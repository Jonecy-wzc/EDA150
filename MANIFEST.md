# EDA_150 导师汇报材料交接清单

本包仅复制现有材料，并编制本清单；没有运行分析、测试、仓库查询或改写任何原代码/原产物，也没有外部请求。压缩包路径以EDA_150为根：原`EDA_150/README.md`在包内为`README.md`，`report/`和`code/README.md`保持原相对位置。

**汇报取舍**：以`report/02_full_report.md`与`report/03_advisor_summary.md`为当前解释，`02a_corrections.md`说明更正。`01_preliminary_findings.md`及P1旧图保留历史原文；混合分层回应、旧钱包活动、未校正规模的旧解释不能当最新发现。没有为打包修订历史报告。

大小口径：2 MB = 2,000,000字节；25 MB = 25,000,000字节。CSV按原始文件大小筛选，超限原表不切片、不重算；行数用CSV逻辑记录计数，不含表头。PNG均为原文件原尺寸复制，未重绘、缩放或转换。

报告中指向SVG、未列入的代码/模块说明或超限大表的原链接可能在包内无目标，按本次要求未擅自补入。CSV里的来源/缓存路径仅为原表内容，不代表这些文件已收入本包。

## 一、导师摘要8张图对照

图注逐段原样摘自`report/03_advisor_summary.md`，不是单独图注文件的替代文本。n列逐张读取图面标注，区分起始人数、逐月有效人数和配对数。

|序号|advisor_figures复制文件 / 原图|对应CSV|摘要中的图注原文|图面样本量n|设计标识|
|---|---|---|---|---|---|
|01|`advisor_figures/01_M1_active_trajectory.png`<br>原图：`report/figures/M1_active_trajectory.png`|`report/tables/M1_active_trajectory.csv`（已打包）|前12个月活跃月数的中位数，甲四层依次是3、3、7、7；乙低于和乙超出分别是2和10，每组25个账号。组别按回应表现选取，这些差异只能描述样本，不能说明某种行为导致了成功。|标题：每组起始 n=25；逐月实际分母未逐点标出。|非设计变量（活跃）；首期受至少3帖资格约束，后期与Y2选样相关。|
|02|`advisor_figures/02_P2a_M2_within_early30.png`<br>原图：`report/figures/P2a_M2_within_early30.png`|`report/tables/P2a_M2_within_early30.csv`（已打包）|只在甲三个非零人数层内部看，30天获回应率与后续活跃月数的相关依次为-0.633、-0.121、-0.348，各层25人。回应人数、获回应帖子比例和首帖至首次回应时间不是一回事；同层内发帖更多也会改变获回应比例的分母。这些结果不能解释为“回应有害”。|六个面板均标 n=25：甲_1-3、甲_4-24、甲_>=25 各25人。|非设计变量（回应率、首回应时间、后续活跃）；仅甲设计层内。|
|03|`advisor_figures/03_P2b_M4_trajectories_first365.png`<br>原图：`report/figures/P2b_M4_trajectories_first365.png`|`report/tables/P2b_M4_trajectories_first365.csv`（已打包）|首365天对端范围在第12个月有132个账号可以计算小图结构，最大连通块占比的中位数为99.5%。节点或边过多的账号没有硬建图；固定对端集合还可能包含后来才接触的人，因此这是回顾性圈子描述。|标题：各月完整观察样本 n≤25（每组上限；未逐点标实际 n）。|非设计变量（网络指标）；组别只是设计标签。|
|04|`advisor_figures/04_P2b_M4_overlap_distribution_first365.png`<br>原图：`report/figures/P2b_M4_overlap_distribution_first365.png`|`report/tables/P2b_M4_overlap_distribution_first365.csv`（超2MB，未打包；见排除清单）|首365天范围共有11,175对不同账号，其中86.0%至少共享一个对端；共同对端占两者对端并集的比例，中位数约为1.1%。同一账号会出现在许多配对中，不能把这些配对当成11,175个独立样本，共享对端也不表示两者互相认识。|标题：配对 n=11,175；指无序账号配对，不是11,175个人。|非设计变量（共同对端/重叠）；配对并非独立样本。|
|05|`advisor_figures/05_P2b_M5_calendar.png`<br>原图：`report/figures/P2b_M5_calendar.png`|`report/tables/P2b_M5_calendar.csv`（已打包）|2024Q1可观察的早批有40个FID、84个用户月，中批只有1个FID、1个用户月，晚批没有样本。图中最高发帖峰在2024-04，中批当月也只有1个账号，不能当成群体热潮。竖线是本地最早保留合约事件，不能当上线日期，也不能直接把变化归因于打赏热潮。|图例：早批逐月面板 n=3–100，中批 n=1–50；2024-04中批峰值标当月 n=1。|混合：原批次为设计变量；日历行为与本地协议时点为非设计变量。|
|06|`advisor_figures/06_P2b_M6_activity_synchrony.png`<br>原图：`report/figures/P2b_M6_activity_synchrony.png`|`report/tables/P2b_M6_activity_synchrony.csv`（已打包）|只看两种状态都可观察的完整月份，在至少一方活跃的月份中，两者同月活跃比例的个人中位数为33.3%，可计算145个账号。链上只计非共享关联地址主动发出的普通交易尝试，并排除已识别的身份合约操作。同月出现或未出现都不说明谁导致了谁，状态未知和分母为0时留空。|组序均为甲_0、甲_1-3、甲_4-24、甲_>=25、乙低于、乙超出。左面板 n=25/25/23/23/24/25；中面板均25；右φ面板 n=18/16/20/19/18/19。|非设计变量（社交/主动链上月同步）；组别为设计标签。|
|07|`advisor_figures/07_P2b_M7_client_history_by_group.png`<br>原图：`report/figures/P2b_M7_client_history_by_group.png`|`report/tables/P2b_M7_client_history_by_group.csv`（已打包）|本地保留的76,424条合格发帖消息中，75,745条能对应到一个客户端，占99.1%。观察到多种客户端或相邻消息变化，只代表已经看到的使用证据；未知映射不能当成没有使用或没有更换。|四个面板的六组均标 n=25（FID点数，不是被映射消息条数）。|非设计变量（客户端及fname计数）；组别为设计标签。|
|08|`advisor_figures/08_P2b_M9_active_axis_sensitivity.png`<br>原图：`report/figures/P2b_M9_active_axis_sensitivity.png`|`report/tables/P2b_M9_active_axis_sensitivity.csv`（已打包）|把起点从首帖改为近似注册时间后，150人中有129人的前12个月活跃月数不变。这个样本本来要求近似注册到首帖不超过30天，而且真实注册时间均未核实，所以不能把变化较小当成时间轴完全可靠。|标题：配对完整观察 n=150；没有逐组 n。|图示活跃月数为非设计变量；注册proxy至首帖间隔参与资格/模型，图脚另标其为设计变量。|

## 二、其余全部图对照

其余64张；不重复上表8张原图。出处列为原报告实际图像引用所在章节；图像所在报告中的阶段性限制一并保留。

|图文件名（原相对路径）|对应CSV|出自报告及章节|
|---|---|---|
|`report/figures/M0_group_cohort.png`|`report/tables/M0_group_cohort.csv`（已打包）|`report/01_preliminary_findings.md` § 各模块图与图注 / M0|
|`report/figures/M0_representativeness.png`|`report/tables/M0_representativeness.csv`（已打包）|`report/01_preliminary_findings.md` § 各模块图与图注 / M0|
|`report/figures/M0_time_distributions.png`|`report/tables/M0_time_distributions.csv`（已打包）|`report/01_preliminary_findings.md` § 各模块图与图注 / M0|
|`report/figures/M1_broad_activity.png`|`report/tables/M1_broad_activity.csv`（已打包）|`report/01_preliminary_findings.md` § 各模块图与图注 / M1|
|`report/figures/M1_cast_trajectory.png`|`report/tables/M1_cast_trajectory.csv`（已打包）|`report/01_preliminary_findings.md` § 各模块图与图注 / M1|
|`report/figures/M1_cluster_groups.png`|`report/tables/M1_cluster_groups.csv`（已打包）|`report/01_preliminary_findings.md` § 各模块图与图注 / M1|
|`report/figures/M1_cluster_trajectories.png`|`report/tables/M1_cluster_trajectories.csv`（已打包）|`report/01_preliminary_findings.md` § 各模块图与图注 / M1|
|`report/figures/M1_retention_cohorts.png`|`report/tables/M1_retention_cohorts.csv`（已打包）|`report/01_preliminary_findings.md` § 各模块图与图注 / M1|
|`report/figures/M1_retention_groups.png`|`report/tables/M1_retention_groups.csv`（已打包）|`report/01_preliminary_findings.md` § 各模块图与图注 / M1|
|`report/figures/M2_early_response_by_group.png`|`report/tables/M2_early_response_by_group.csv`（已打包）|`report/01_preliminary_findings.md` § 比较计数与限制|
|`report/figures/M2_first_response_time_by_group.png`|`report/tables/M2_first_response_time_by_group.csv`（已打包）|`report/01_preliminary_findings.md` § 比较计数与限制|
|`report/figures/M2_followup_activity_by_response.png`|`report/tables/M2_followup_activity_by_response.csv`（已打包）|`report/01_preliminary_findings.md` § 比较计数与限制|
|`report/figures/M2_post_response_delay_by_group.png`|`report/tables/M2_post_response_delay_by_group.csv`（已打包）|`report/01_preliminary_findings.md` § 比较计数与限制|
|`report/figures/M2_responder_profile_by_group.png`|`report/tables/M2_responder_profile_by_group.csv`（已打包）|`report/01_preliminary_findings.md` § 比较计数与限制|
|`report/figures/M2_retention_by_response.png`|`report/tables/M2_retention_by_response.csv`（已打包）|`report/01_preliminary_findings.md` § 比较计数与限制|
|`report/figures/M3_early_followers.png`|`report/tables/M3_early_followers.csv`（已打包）|`report/01_preliminary_findings.md` § 比较计数与限制 / M3|
|`report/figures/M3_followers_trajectory.png`|`report/tables/M3_followers_trajectory.csv`（已打包）|`report/01_preliminary_findings.md` § 比较计数与限制 / M3|
|`report/figures/M3_following_trajectory.png`|`report/tables/M3_following_trajectory.csv`（已打包）|`report/01_preliminary_findings.md` § 比较计数与限制 / M3|
|`report/figures/M3_reciprocal_delay.png`|`report/tables/M3_reciprocal_delay.csv`（超2MB，未打包；见排除清单）|`report/01_preliminary_findings.md` § 比较计数与限制 / M3|
|`report/figures/M3_reciprocity.png`|`report/tables/M3_reciprocity.csv`（已打包）|`report/01_preliminary_findings.md` § 比较计数与限制 / M3|
|`report/figures/M4_alter_activity_monthly.png`|`report/tables/M4_alter_activity_monthly.csv`（已打包）|`report/01_preliminary_findings.md` § 计算边界与图表|
|`report/figures/M4_alter_counts_groups.png`|`report/tables/M4_alter_counts_groups.csv`（已打包）|`report/01_preliminary_findings.md` § 计算边界与图表|
|`report/figures/M4_follow_density_groups.png`|`report/tables/M4_follow_density_groups.csv`（已打包）|`report/01_preliminary_findings.md` § 计算边界与图表|
|`report/figures/M4_interaction_counts_groups.png`|`report/tables/M4_interaction_counts_groups.csv`（已打包）|`report/01_preliminary_findings.md` § 计算边界与图表|
|`report/figures/M4_scatter_M1_active_months.png`|`report/tables/M4_scatter_M1_active_months.csv`（已打包）|`report/01_preliminary_findings.md` § 计算边界与图表|
|`report/figures/M4_scatter_M3_followers_month12.png`|`report/tables/M4_scatter_M3_followers_month12.csv`（已打包）|`report/01_preliminary_findings.md` § 计算边界与图表|
|`report/figures/M4_scatter_interaction_M1_active_months.png`|`report/tables/M4_scatter_interaction_M1_active_months.csv`（已打包）|`report/01_preliminary_findings.md` § 计算边界与图表|
|`report/figures/M4_scatter_interaction_M3_followers_month12.png`|`report/tables/M4_scatter_interaction_M3_followers_month12.csv`（已打包）|`report/01_preliminary_findings.md` § 计算边界与图表|
|`report/figures/M6_address_activity_scope.png`|`report/tables/M6_address_activity_scope.csv`（已打包）|`report/01_preliminary_findings.md` § 计算边界与图表 / M6 / M6 钱包与链上概况：口径说明|
|`report/figures/M6_first_activity_gap.png`|`report/tables/M6_first_activity_gap.csv`（已打包）|`report/01_preliminary_findings.md` § 计算边界与图表 / M6 / M6 钱包与链上概况：口径说明|
|`report/figures/M6_first_activity_timing_status.png`|`report/tables/M6_first_activity_timing_status.csv`（已打包）|`report/01_preliminary_findings.md` § 计算边界与图表 / M6 / M6 钱包与链上概况：口径说明|
|`report/figures/M6_person_chain_activity_status.png`|`report/tables/M6_person_chain_activity_status.csv`（已打包）|`report/01_preliminary_findings.md` § 计算边界与图表 / M6 / M6 钱包与链上概况：口径说明|
|`report/figures/M8_core_comparison_1.png`|`report/tables/M8_core_comparison_1.csv`（已打包）|`report/01_preliminary_findings.md` § 计算边界与图表 / M8|
|`report/figures/M8_core_comparison_2.png`|`report/tables/M8_core_comparison_2.csv`（已打包）|`report/01_preliminary_findings.md` § 计算边界与图表 / M8|
|`report/figures/M8_core_comparison_3.png`|`report/tables/M8_core_comparison_3.csv`（已打包）|`report/01_preliminary_findings.md` § 计算边界与图表 / M8|
|`report/figures/P2a_M2_count_and_rate_separate.png`|`report/tables/P2a_M2_count_and_rate_separate.csv`（已打包）|`report/02a_corrections.md` § 5. 图表、比较次数和复现 / P2a_M2_count_and_rate_separate|
|`report/figures/P2a_M2_within_first10.png`|`report/tables/P2a_M2_within_first10.csv`（已打包）|`report/02a_corrections.md` § 5. 图表、比较次数和复现 / P2a_M2_within_first10|
|`report/figures/P2a_M4_associations_all_time.png`|`report/tables/P2a_M4_associations_all_time.csv`（已打包）|`report/02a_corrections.md` § 5. 图表、比较次数和复现 / P2a_M4_associations_all_time|
|`report/figures/P2a_M4_associations_first365.png`|`report/tables/P2a_M4_associations_first365.csv`（已打包）|`report/02a_corrections.md` § 5. 图表、比较次数和复现 / P2a_M4_associations_first365|
|`report/figures/P2a_M6_ETH_definition_funnel.png`|`report/tables/P2a_M6_ETH_definition_funnel.csv`（已打包）|`report/02a_corrections.md` § 5. 图表、比较次数和复现 / P2a_M6_ETH_definition_funnel|
|`report/figures/P2a_M6_activity_by_group.png`|`report/tables/P2a_M6_activity_by_group.csv`（已打包）|`report/02a_corrections.md` § 5. 图表、比较次数和复现 / P2a_M6_activity_by_group|
|`report/figures/P2a_M6_first_active_gap.png`|`report/tables/P2a_M6_first_active_gap.csv`（已打包）|`report/02a_corrections.md` § 5. 图表、比较次数和复现 / P2a_M6_first_active_gap|
|`report/figures/P2b_M4_overlap_distribution_all_time.png`|`report/tables/P2b_M4_overlap_distribution_all_time.csv`（超2MB，未打包；见排除清单）|`report/02_full_report.md` § 各模块图和图注 / P2b_M4_overlap_distribution_all_time|
|`report/figures/P2b_M4_trajectories_all_time.png`|`report/tables/P2b_M4_trajectories_all_time.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M4_trajectories_all_time|
|`report/figures/P2b_M5_DEGEN_inflows_by_group.png`|`report/tables/P2b_M5_DEGEN_inflows_by_group.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M5_DEGEN_inflows_by_group|
|`report/figures/P2b_M5_DEGEN_social_monthly_comparison.png`|`report/tables/P2b_M5_DEGEN_social_monthly_comparison.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M5_DEGEN_social_monthly_comparison|
|`report/figures/P2b_M5_pre_during_post.png`|`report/tables/P2b_M5_pre_during_post.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M5_pre_during_post|
|`report/figures/P2b_M6_balance_distribution_Base.png`|`report/tables/P2b_M6_balance_distribution_Base.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M6_balance_distribution_Base|
|`report/figures/P2b_M6_balance_distribution_ETH.png`|`report/tables/P2b_M6_balance_distribution_ETH.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M6_balance_distribution_ETH|
|`report/figures/P2b_M6_balance_distribution_OP.png`|`report/tables/P2b_M6_balance_distribution_OP.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M6_balance_distribution_OP|
|`report/figures/P2b_M6_contract_event_timing.png`|`report/tables/P2b_M6_contract_event_timing.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M6_contract_event_timing|
|`report/figures/P2b_M6_contract_participation_by_group_chart.png`|`report/tables/P2b_M6_contract_participation_by_group_chart.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M6_contract_participation_by_group_chart|
|`report/figures/P2b_M6_node_balance_trend_Base.png`|`report/tables/P2b_M6_node_balance_trend_Base.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M6_node_balance_trend_Base|
|`report/figures/P2b_M6_node_balance_trend_ETH.png`|`report/tables/P2b_M6_node_balance_trend_ETH.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M6_node_balance_trend_ETH|
|`report/figures/P2b_M6_node_balance_trend_OP.png`|`report/tables/P2b_M6_node_balance_trend_OP.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M6_node_balance_trend_OP|
|`report/figures/P2b_M7_current_verified_addresses.png`|`report/tables/P2b_M7_current_verified_addresses.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M7_current_verified_addresses|
|`report/figures/P2b_M7_storage_capacity_by_group.png`|`report/tables/P2b_M7_storage_capacity_by_group.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M7_storage_capacity_by_group|
|`report/figures/P2b_M8_case_13769.png`|`report/tables/P2b_M8_case_13769.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M8_case_13769|
|`report/figures/P2b_M8_case_250719.png`|`report/tables/P2b_M8_case_250719.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M8_case_250719|
|`report/figures/P2b_M8_case_487270.png`|`report/tables/P2b_M8_case_487270.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M8_case_487270|
|`report/figures/P2b_M8_case_508970.png`|`report/tables/P2b_M8_case_508970.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M8_case_508970|
|`report/figures/P2b_M8_case_539273.png`|`report/tables/P2b_M8_case_539273.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M8_case_539273|
|`report/figures/P2b_M8_case_785986.png`|`report/tables/P2b_M8_case_785986.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M8_case_785986|
|`report/figures/P2b_M9_early60_by_stratum.png`|`report/tables/P2b_M9_early60_by_stratum.csv`（已打包）|`report/02_full_report.md` § 各模块图和图注 / P2b_M9_early60_by_stratum|

## 三、五项补充的现有完成情况

**仅审计既有文件，不补做分析。前四项未发现指定补充的独立完成结果；第五项已完成。相关已有图表不等于所要求的补充已做，未运行的检查也不标成“通过”或“失败”。**

|补充项|完成状态|现有图 / 专门结果图|现有表|报告章节|缺口、原因或选取规则|
|---|---|---|---|---|---|
|早期回应控制发帖数|未做该控制分析|无独立完成图。相关已有图：`report/figures/P2a_M2_within_early30.png`、`P2a_M2_within_first10.png`。|`report/tables/P2a_M2_within_associations.csv`、`P2a_M2_count_and_rate_separate.csv`；P2b相关表为`P2b_M9_sensitivity_associations.csv`及`P2b_M9_disjoint_sensitivity_associations.csv`。|`report/02a_corrections.md` § 1. 抽样设计：精确定义与标签；`report/02_full_report.md` § P1经P2a核对后保留的描述、M9：时间轴、60天、广义活跃与设计权重。|现有结果为甲层内未调整Spearman；以发帖数作回应率分母、或在回应人数层内分析，均不等于把发帖数作为协变量控制。未找到调整回归/偏相关或控制后效应表。当前只读打包，不补算。|
|首次链上活动 ±90天与 >365天|未做指定分窗/分档补充|无±90天或>365天专门图。相关全分布图：`report/figures/P2a_M6_first_active_gap.png`。|`report/tables/P2a_M6_first_active_gap.csv`、`P2a_M6_first_active_gap_by_group.csv`、`P2b_M6_first_active_time_chain_audit.csv`。|`report/02a_corrections.md` § 2. 链上活动：主动、协议、角色、共享；`report/02_full_report.md` § M6：节点余额、月活跃同步与历史合约参与。|现有产物只给连续时间差、首帖前后计数和首次链标签核对，未输出这两个指定时间窗/阈值的独立结果。本次不根据逐人表新计算这些分档。|
|第3个月网络对照后续结果|第3个月网络描述已做；独立后续结果对照未做|已有时间轨迹图：`report/figures/P2b_M4_trajectories_all_time.png`、`P2b_M4_trajectories_first365.png`；没有第3个月网络暴露对照后续结果的专门图。|`report/tables/P2b_M4_time_metrics.csv`（含90天时点）、`P2b_M4_time_group_summary.csv`、两份`P2b_M4_trajectories_*.csv`。相关旧关联表`P2a_M4_associations.csv`不是第3个月滞后对照。|`report/02_full_report.md` § M4：时间变化、小图结构与共同对端；`report/02a_corrections.md` § 3. 网络：分别画scope并调整规模。|已有3/6/12/24个30天区间末的状态；后续关联仍用首年汇总暴露，未形成“第90天网络→其后结果”的独立分析。不能把M9第3–12月的早期回应关联当成网络补充。|
|迁移后注册事件单调性检查|未做单调性检验，不能记作通过|未找到独立单调性结果图；现有注册检查以表为主。|`report/tables/P2a_registration_coverage.csv`、`P2a_registration_person_status.csv`、`P2a_registration_register_batches.csv`、`P2a_registration_alter_summary.csv`（超限未打包）。|`report/02a_corrections.md` § 4. 注册：事件时间不等于真实创号；`report/02_full_report.md` § 研究口径与设计边界、M9：时间轴、60天、广义活跃与设计权重。|原有检查统计部署版本、首末区块和同FID跨版本先后登记，没有定义并检验迁移后注册序列的单调性。报告说明显式IdRegistry Migrated事件为0、调用入口未还原、迁移与普通登记仍可能混淆；这些证据不能替代单调性通过结果。|
|个案选取规则|已完成且规则明确|六图：`report/figures/P2b_M8_case_13769.png`、`P2b_M8_case_487270.png`、`P2b_M8_case_250719.png`、`P2b_M8_case_539273.png`、`P2b_M8_case_785986.png`、`P2b_M8_case_508970.png`。|`report/tables/P2b_M8_case_selection.csv`、`P2b_M8_case_timelines.csv`、`P2b_M8_response_reconciliation.csv`及六张同名个案CSV。|`report/02_full_report.md` § M8：按规则选取的六个匿名个案；§ 各模块图和图注 / 对应六个P2b_M8_case_*小节。|乙超出按residual_Y2_log降序、乙低于按升序，各取3个FID；并列按FID升序。已列组内极端序位，六人的Y2与冻结变量核对一致。规则本身及选案残差属于设计变量；不能把个案差异当独立验证。|

## 四、超过2MB而未打包的CSV

|原文件名|字节|MB（十进制）|数据行数（不含表头）|
|---|---:|---:|---:|
|report/tables/M2_responders.csv|2883356|2.883356|14432|
|report/tables/M3_follow_reciprocity_pairs.csv|9344280|9.344280|115906|
|report/tables/M3_reciprocal_delay.csv|10419715|10.419715|115906|
|report/tables/P2a_registration_alter_summary.csv|39180834|39.180834|91725|
|report/tables/P2b_M4_overlap.csv|5262400|5.262400|22350|
|report/tables/P2b_M4_overlap_distribution_all_time.csv|2658017|2.658017|11175|
|report/tables/P2b_M4_overlap_distribution_first365.csv|2604533|2.604533|11175|
|report/tables/P2b_M6_node_balance_person_month.csv|8667008|8.667008|51832|
|report/tables/P2b_M6_node_balances.csv|56550798|56.550798|110664|

排除9份CSV。特别是导师第04图的同名CSV超限未打包；其PNG仍完整收入包中。其他CSV均逐文件原样复制，没有把大表改成小表。

## 五、压缩包内文件数与总大小

- 报告与说明：8份（5份报告、2份README、1份run_metrics.json）。
- 原路径PNG：72张；导师顺序复制PNG：8张。
- CSV：189份（原有198份，超限排除9份）。
- 本清单：1份。
- **包内合计：278个普通文件，31,864,983字节（31.864983 MB，解压后内容大小，包含MANIFEST.md本身）。**

以下大小为压缩包内文件内容合计，不是ZIP文件自身大小；ZIP实际大小在交付回复列出。ZIP本身不嵌套入自身，也不计入上述文件数。

|压缩包|文件数|包内内容字节（含其清单）|
|---|---:|---:|
|EDA_150_handoff.zip|278|31864983|

单包压缩后未超过25MB，无需分包。

## 六、包内文件索引

|相对路径|字节|
|---|---:|
|MANIFEST.md|39827|
|README.md|3388|
|advisor_figures/01_M1_active_trajectory.png|242052|
|advisor_figures/02_P2a_M2_within_early30.png|240155|
|advisor_figures/03_P2b_M4_trajectories_first365.png|414563|
|advisor_figures/04_P2b_M4_overlap_distribution_first365.png|78228|
|advisor_figures/05_P2b_M5_calendar.png|294358|
|advisor_figures/06_P2b_M6_activity_synchrony.png|280436|
|advisor_figures/07_P2b_M7_client_history_by_group.png|282736|
|advisor_figures/08_P2b_M9_active_axis_sensitivity.png|173670|
|code/README.md|7739|
|report/00_data_inventory.md|13442|
|report/01_preliminary_findings.md|48097|
|report/02_full_report.md|65349|
|report/02a_corrections.md|26216|
|report/03_advisor_summary.md|5058|
|report/figures/M0_group_cohort.png|68742|
|report/figures/M0_representativeness.png|174536|
|report/figures/M0_time_distributions.png|133028|
|report/figures/M1_active_trajectory.png|242052|
|report/figures/M1_broad_activity.png|273786|
|report/figures/M1_cast_trajectory.png|239726|
|report/figures/M1_cluster_groups.png|58940|
|report/figures/M1_cluster_trajectories.png|167961|
|report/figures/M1_retention_cohorts.png|84392|
|report/figures/M1_retention_groups.png|102563|
|report/figures/M2_early_response_by_group.png|156228|
|report/figures/M2_first_response_time_by_group.png|157992|
|report/figures/M2_followup_activity_by_response.png|161326|
|report/figures/M2_post_response_delay_by_group.png|153545|
|report/figures/M2_responder_profile_by_group.png|258246|
|report/figures/M2_retention_by_response.png|141330|
|report/figures/M3_early_followers.png|206670|
|report/figures/M3_followers_trajectory.png|182893|
|report/figures/M3_following_trajectory.png|154884|
|report/figures/M3_reciprocal_delay.png|173872|
|report/figures/M3_reciprocity.png|163427|
|report/figures/M4_alter_activity_monthly.png|342879|
|report/figures/M4_alter_counts_groups.png|181782|
|report/figures/M4_follow_density_groups.png|174290|
|report/figures/M4_interaction_counts_groups.png|197548|
|report/figures/M4_scatter_M1_active_months.png|166087|
|report/figures/M4_scatter_M3_followers_month12.png|179094|
|report/figures/M4_scatter_interaction_M1_active_months.png|152565|
|report/figures/M4_scatter_interaction_M3_followers_month12.png|163551|
|report/figures/M6_address_activity_scope.png|81529|
|report/figures/M6_first_activity_gap.png|145095|
|report/figures/M6_first_activity_timing_status.png|110743|
|report/figures/M6_person_chain_activity_status.png|138775|
|report/figures/M8_core_comparison_1.png|280987|
|report/figures/M8_core_comparison_2.png|264412|
|report/figures/M8_core_comparison_3.png|360454|
|report/figures/P2a_M2_count_and_rate_separate.png|230813|
|report/figures/P2a_M2_within_early30.png|240155|
|report/figures/P2a_M2_within_first10.png|238529|
|report/figures/P2a_M4_associations_all_time.png|781743|
|report/figures/P2a_M4_associations_first365.png|779110|
|report/figures/P2a_M6_ETH_definition_funnel.png|126665|
|report/figures/P2a_M6_activity_by_group.png|199090|
|report/figures/P2a_M6_first_active_gap.png|114773|
|report/figures/P2b_M4_overlap_distribution_all_time.png|76667|
|report/figures/P2b_M4_overlap_distribution_first365.png|78228|
|report/figures/P2b_M4_trajectories_all_time.png|430498|
|report/figures/P2b_M4_trajectories_first365.png|414563|
|report/figures/P2b_M5_DEGEN_inflows_by_group.png|264605|
|report/figures/P2b_M5_DEGEN_social_monthly_comparison.png|706101|
|report/figures/P2b_M5_calendar.png|294358|
|report/figures/P2b_M5_pre_during_post.png|123244|
|report/figures/P2b_M6_activity_synchrony.png|280436|
|report/figures/P2b_M6_balance_distribution_Base.png|385456|
|report/figures/P2b_M6_balance_distribution_ETH.png|274412|
|report/figures/P2b_M6_balance_distribution_OP.png|353489|
|report/figures/P2b_M6_contract_event_timing.png|152926|
|report/figures/P2b_M6_contract_participation_by_group_chart.png|192732|
|report/figures/P2b_M6_node_balance_trend_Base.png|342581|
|report/figures/P2b_M6_node_balance_trend_ETH.png|297030|
|report/figures/P2b_M6_node_balance_trend_OP.png|305844|
|report/figures/P2b_M7_client_history_by_group.png|282736|
|report/figures/P2b_M7_current_verified_addresses.png|111140|
|report/figures/P2b_M7_storage_capacity_by_group.png|226248|
|report/figures/P2b_M8_case_13769.png|329356|
|report/figures/P2b_M8_case_250719.png|311670|
|report/figures/P2b_M8_case_487270.png|282170|
|report/figures/P2b_M8_case_508970.png|266418|
|report/figures/P2b_M8_case_539273.png|257335|
|report/figures/P2b_M8_case_785986.png|259514|
|report/figures/P2b_M9_active_axis_sensitivity.png|173670|
|report/figures/P2b_M9_early60_by_stratum.png|271448|
|report/run_metrics.json|16707|
|report/tables/M0_age_and_sampling.csv|520|
|report/tables/M0_cutoff_boundaries.csv|330|
|report/tables/M0_group_cohort.csv|331|
|report/tables/M0_known_limitations.csv|5162|
|report/tables/M0_representativeness.csv|146487|
|report/tables/M0_representativeness_summary.csv|740|
|report/tables/M0_sample.csv|21883|
|report/tables/M0_time_distributions.csv|1070|
|report/tables/M0_used_fields_dictionary.csv|91295|
|report/tables/M1_active_trajectory.csv|6767|
|report/tables/M1_broad_activity.csv|4956|
|report/tables/M1_cast_trajectory.csv|6767|
|report/tables/M1_cluster_assignments.csv|2679|
|report/tables/M1_cluster_candidates.csv|106|
|report/tables/M1_cluster_groups.csv|127|
|report/tables/M1_cluster_trajectories.csv|971|
|report/tables/M1_monthly_panel.csv|129373|
|report/tables/M1_person_metrics.csv|14885|
|report/tables/M1_retention_cohorts.csv|2204|
|report/tables/M1_retention_groups.csv|3745|
|report/tables/M2_early_response_by_group.csv|85123|
|report/tables/M2_first_response_time_by_group.csv|85123|
|report/tables/M2_followup_activity_by_response.csv|170603|
|report/tables/M2_group_summary.csv|1399|
|report/tables/M2_person_metrics.csv|85123|
|report/tables/M2_post_response_delay_by_group.csv|85123|
|report/tables/M2_responder_profile_by_group.csv|85123|
|report/tables/M2_retention_by_response.csv|15527|
|report/tables/M3_cutoff_quality.csv|125|
|report/tables/M3_early_followers.csv|28332|
|report/tables/M3_first10_followers.csv|135612|
|report/tables/M3_follow_quality.csv|317|
|report/tables/M3_followers_trajectory.csv|5219|
|report/tables/M3_following_trajectory.csv|5479|
|report/tables/M3_monthly_follow_counts.csv|121738|
|report/tables/M3_person_metrics.csv|28332|
|report/tables/M3_reciprocity.csv|23255|
|report/tables/M4_alter_activity_monthly.csv|13006|
|report/tables/M4_alter_counts_groups.csv|137851|
|report/tables/M4_follow_density_groups.csv|137851|
|report/tables/M4_interaction_counts_groups.csv|137851|
|report/tables/M4_network_degradation.csv|28088|
|report/tables/M4_person_metrics.csv|137851|
|report/tables/M4_scatter_M1_active_months.csv|138873|
|report/tables/M4_scatter_M3_followers_month12.csv|138873|
|report/tables/M4_scatter_interaction_M1_active_months.csv|138873|
|report/tables/M4_scatter_interaction_M3_followers_month12.csv|138873|
|report/tables/M6_address_activity_scope.csv|754|
|report/tables/M6_first_activity_gap.csv|17580|
|report/tables/M6_first_activity_gap_by_group.csv|342|
|report/tables/M6_first_activity_timing_status.csv|1385|
|report/tables/M6_person_chain_activity_overall.csv|702|
|report/tables/M6_person_chain_activity_status.csv|3332|
|report/tables/M6_person_metrics.csv|17580|
|report/tables/M8_core_comparison_1.csv|18101|
|report/tables/M8_core_comparison_2.csv|20076|
|report/tables/M8_core_comparison_3.csv|21779|
|report/tables/M8_core_metrics.csv|17889|
|report/tables/M8_effect_sizes.csv|26011|
|report/tables/M8_group_medians.csv|3787|
|report/tables/P1_beta_effects.csv|4521|
|report/tables/P1_group_summary.csv|811|
|report/tables/P1_network_associations.csv|2960|
|report/tables/P1_responder_summary.csv|357|
|report/tables/P1_response_associations.csv|1141|
|report/tables/P2a_M2_count_and_rate_separate.csv|84895|
|report/tables/P2a_M2_window_timing.csv|244|
|report/tables/P2a_M2_within_associations.csv|3605|
|report/tables/P2a_M2_within_early30.csv|49262|
|report/tables/P2a_M2_within_first10.csv|49262|
|report/tables/P2a_M2_within_stratum_person.csv|49262|
|report/tables/P2a_M4_associations.csv|8707|
|report/tables/P2a_M4_associations_all_time.csv|104597|
|report/tables/P2a_M4_associations_first365.csv|104513|
|report/tables/P2a_M4_partial_rank.csv|1866|
|report/tables/P2a_M4_person_metrics.csv|208190|
|report/tables/P2a_M4_raw_adjusted_summary.csv|620|
|report/tables/P2a_M4_regression_diagnostics.csv|1291|
|report/tables/P2a_M6_ETH_account_evidence.csv|41492|
|report/tables/P2a_M6_ETH_changed_first_activity_evidence.csv|3377|
|report/tables/P2a_M6_ETH_definition_funnel.csv|874|
|report/tables/P2a_M6_ETH_group_funnel.csv|874|
|report/tables/P2a_M6_T1_cutoff_quality.csv|423|
|report/tables/P2a_M6_activity_by_group.csv|12302|
|report/tables/P2a_M6_definition_comparison.csv|169986|
|report/tables/P2a_M6_effect_sizes.csv|2758|
|report/tables/P2a_M6_first_active_gap.csv|124191|
|report/tables/P2a_M6_first_active_gap_by_group.csv|335|
|report/tables/P2a_M6_null_recipient_audit.csv|137|
|report/tables/P2a_M6_overall_comparison.csv|318|
|report/tables/P2a_M6_person_metrics.csv|124191|
|report/tables/P2a_M6_protocol_contracts.csv|421|
|report/tables/P2a_M6_protocol_operations.csv|5070|
|report/tables/P2a_M6_role_activity_by_group.csv|3958|
|report/tables/P2a_M6_role_eligibility_audit.csv|26414|
|report/tables/P2a_M6_role_overall.csv|388|
|report/tables/P2a_M6_shared_address_chain_activity.csv|301|
|report/tables/P2a_M6_shared_address_summary.csv|115|
|report/tables/P2a_M6_wallet_role_evidence.csv|464070|
|report/tables/P2a_M6_wallet_role_summary.csv|837|
|report/tables/P2a_design_variable_registry.csv|3439|
|report/tables/P2a_figure_design_annotations.csv|9611|
|report/tables/P2a_output_manifest.csv|54228|
|report/tables/P2a_registration_coverage.csv|4453|
|report/tables/P2a_registration_person_status.csv|88617|
|report/tables/P2a_registration_register_batches.csv|379896|
|report/tables/P2a_registration_sources.csv|608|
|report/tables/P2a_sampling_audit_person.csv|15501|
|report/tables/P2a_sampling_design_group_summary.csv|779|
|report/tables/P2a_sampling_model_inputs.csv|1175|
|report/tables/P2a_sampling_sources.csv|808|
|report/tables/P2b_M4_independent_graph_crosscheck.csv|6976|
|report/tables/P2b_M4_overlap_report_summary.csv|344|
|report/tables/P2b_M4_report_summary.csv|972|
|report/tables/P2b_M4_time_group_summary.csv|15459|
|report/tables/P2b_M4_time_metrics.csv|1016821|
|report/tables/P2b_M4_trajectories_all_time.csv|7962|
|report/tables/P2b_M4_trajectories_first365.csv|7856|
|report/tables/P2b_M5_DEGEN_bridge_diagnostic.csv|174|
|report/tables/P2b_M5_DEGEN_contract_evidence.csv|378|
|report/tables/P2b_M5_DEGEN_inflows.csv|1213106|
|report/tables/P2b_M5_DEGEN_inflows_by_group.csv|1245956|
|report/tables/P2b_M5_DEGEN_monthly_inflows.csv|16231|
|report/tables/P2b_M5_DEGEN_report_summary.csv|506|
|report/tables/P2b_M5_DEGEN_social_matched_months.csv|42980|
|report/tables/P2b_M5_DEGEN_social_monthly_comparison.csv|42980|
|report/tables/P2b_M5_DEGEN_source_status_diagnostic.csv|145|
|report/tables/P2b_M5_calendar.csv|10727|
|report/tables/P2b_M5_calendar_by_design_group.csv|64604|
|report/tables/P2b_M5_local_base_contract_first_events.csv|1702|
|report/tables/P2b_M5_pre_during_post.csv|1123|
|report/tables/P2b_M5_pre_during_post_by_cohort.csv|1123|
|report/tables/P2b_M6_Base_contract_cutoff_audit.csv|1250|
|report/tables/P2b_M6_activity_synchrony.csv|29134|
|report/tables/P2b_M6_balance_asset_identity_crosscheck.csv|1799|
|report/tables/P2b_M6_balance_coverage_report.csv|824|
|report/tables/P2b_M6_balance_distribution_Base.csv|333996|
|report/tables/P2b_M6_balance_distribution_ETH.csv|155099|
|report/tables/P2b_M6_balance_distribution_OP.csv|300537|
|report/tables/P2b_M6_collectible_recipient_by_fid.csv|251|
|report/tables/P2b_M6_collectible_recipient_events.csv|1275|
|report/tables/P2b_M6_contract_event_timing.csv|7220|
|report/tables/P2b_M6_contract_participation.csv|8041|
|report/tables/P2b_M6_contract_participation_by_fid.csv|1952|
|report/tables/P2b_M6_contract_participation_by_group.csv|652|
|report/tables/P2b_M6_contract_participation_by_group_chart.csv|652|
|report/tables/P2b_M6_contract_report_summary.csv|747|
|report/tables/P2b_M6_contract_social_alignment.csv|7220|
|report/tables/P2b_M6_first_active_time_chain_audit.csv|20591|
|report/tables/P2b_M6_latest_balance_distribution.csv|277522|
|report/tables/P2b_M6_node_balance_trend_Base.csv|107798|
|report/tables/P2b_M6_node_balance_trend_ETH.csv|173100|
|report/tables/P2b_M6_node_balance_trend_OP.csv|143223|
|report/tables/P2b_M6_node_balance_trends.csv|423717|
|report/tables/P2b_M6_person_month_activity.csv|819642|
|report/tables/P2b_M6_social_chain_sync.csv|51195|
|report/tables/P2b_M6_stable_address_balance_changes.csv|388186|
|report/tables/P2b_M6_sync_correlations.csv|29134|
|report/tables/P2b_M7_active_correlations.csv|2516|
|report/tables/P2b_M7_client_app_summary.csv|1474|
|report/tables/P2b_M7_client_history_by_group.csv|56418|
|report/tables/P2b_M7_client_mapping_status.csv|86|
|report/tables/P2b_M7_client_transitions.csv|3051|
|report/tables/P2b_M7_current_verified_addresses.csv|56418|
|report/tables/P2b_M7_person_metrics.csv|56418|
|report/tables/P2b_M7_storage_capacity_by_group.csv|56418|
|report/tables/P2b_M8_case_13769.csv|5792|
|report/tables/P2b_M8_case_250719.csv|4620|
|report/tables/P2b_M8_case_487270.csv|4041|
|report/tables/P2b_M8_case_508970.csv|4057|
|report/tables/P2b_M8_case_539273.csv|3930|
|report/tables/P2b_M8_case_785986.csv|3757|
|report/tables/P2b_M8_case_selection.csv|444|
|report/tables/P2b_M8_case_timelines.csv|24912|
|report/tables/P2b_M8_response_reconciliation.csv|164|
|report/tables/P2b_M9_active_axis_sensitivity.csv|73162|
|report/tables/P2b_M9_comparison_accounting.csv|643|
|report/tables/P2b_M9_disjoint_sensitivity_associations.csv|7238|
|report/tables/P2b_M9_early60_by_stratum.csv|40025|
|report/tables/P2b_M9_sensitivity.csv|73162|
|report/tables/P2b_M9_sensitivity_associations.csv|6045|
|report/tables/P2b_M9_weighted_summary.csv|5650|
|report/tables/P2b_advisor_figure_selection.csv|1411|
|report/tables/P2b_figure_design_annotations.csv|16078|
|report/tables/P2b_output_manifest.csv|135785|
|report/tables/P2b_semantic_sources.csv|737|
|report/tables/P2b_used_fields_dictionary.csv|182341|
|report/tables/P2b_used_tables.csv|19525|
|report/tables/output_manifest.csv|34769|

## 七、完整性与排除项

打包前后核对EDA_150原文件的大小与mtime未变；收入包的源文件额外核对SHA-256，复制文件及ZIP内字节与源文件一致。8份advisor_figures为原PNG字节复制。

压缩使用`zip -X -9`。ZIP成员中不包含data/、cache/、.duckdb_tmp/、Parquet、日志、SVG、pycache、._*或__MACOSX；只包含上面逐项列出的Markdown、JSON、PNG和CSV。
