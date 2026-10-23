代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3yvsprjpe.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3xvezbnwe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pfpqkpdq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3nubgkeue.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3bpjgamct.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3etggibju.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3qgtjurhf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3nwddeurs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3badekgiw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3apihcysu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3acfcajdv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3bgeyzmgb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3vusfrqkq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3vigdglhk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3foqbjcvr.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3dcherenf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kxeslpkv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3qgfqmgpb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aflsmenf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ddglorgk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3egbajvhk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3zdtlikut.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zzlzdwyi.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gvwlguyz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ymrfqhbp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ecyecqla.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3woocwfxe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3bhzllocy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3fgwsijao.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3zvosargi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3wxgqkysz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3rhgbvnkn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3soikeebz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hbcvhivt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3cyogbnjj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gyhudrgz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vbxigkdz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hdgyahxq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3pkylaboj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zvwklexy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3rbzkndvc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3oahhmiyg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3xxxjwagb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3frdasong.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3odnpydhq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3dhuhrydz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3rfbanuhz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3irprqlkl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3dvxmyoow.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3cotbcxrd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sycmfbmi.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hwdjukgr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3uiubsxjz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3mavdajiv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3uwpyiawc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3gryozsjj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ojngstek.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kqychixa.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3kngewllu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wbnetldw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3dfevjdkh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cptobmhi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xiwkxmou.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3aojhwioc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3daizorwi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ltpumeqt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kmtdxbjg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3wcbxeouo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gqxssajc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3kwxuxwhb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3opqgmsac.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3fmllcnls.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xgrtauep.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3bwmalycw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3judvpfcl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3oqzvbqkg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gxqqrxpw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3mmnowtba.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3cqaaackh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gxizhkza.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3bxchgyzm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3nnyjllcy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3raahslsq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3nsguqcgc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xpiswezm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3lkzvpaki.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iezxctmx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ygxbjcvx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mtlgjntc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3qitvslmy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3wjkavspr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pbawvhoc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3jdtdhxnl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kswpawtm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zvmypkhj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3olcbzzvt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3isknfzch.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3yrkwkopn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3cxpcybhr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3lgrtrbog.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3wbcestfi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3flnrccze.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ukubstqe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3gexmrvvh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ialsigwb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ivwicnzu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3oiunagzt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3nehwdsex.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ogdtmnqw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3atqvwtlu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3tiqxztij.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3rhcitftm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3zkivnizf.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3pbqklquv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3xtnbasxi.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3dihyfgmb.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vwpekocd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ikhwxxlu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3gybbytsk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ayjsszyx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3qdxiyxrf.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zroxfvkf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uyopeybj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3fmuhnjox.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3acxipvsp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3atlksnju.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3gggidier.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3cftrmjrj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3zzyfcpum.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ztuiskfd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pdwknyxe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3vcppcese.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3fuipwydr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ylpbjzca.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3psjeoisx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lwkyyvxm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qihzrjrd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ebzvhjfz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xqbqbxnl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aulhtkkf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3txrqpwqr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3djtbiuzd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3wacwfxwn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ssgjwjjn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3knpghhkd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3rbdvtcbl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3crkgavnn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3agkirsgc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3npoaqyjx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3omcgojkn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zdjyfgvp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xzmbmyeh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ackkshbf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3qqgbxuae.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ooxyqlpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3giyvqsdj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ieqqxwyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehbxmvjx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ufewprsq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3emivmljr.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3rdyzaxlx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3iyscftwj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ydiozzvr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3lbybhfjj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3sapftmmj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3nhwnwkym.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3tnqmqsme.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bxpcfcit.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3hxfrzpxq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3bnonuehv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fgjyyjqk.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3aygxasjx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rejbqgab.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3shxqvhbs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ochwnafv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3inqwpnnw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3dctpbyvp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3mmlrwiac.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ivdatvnd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3lgrybzvm.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3eirpwawo.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3grpmcxdy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kjjjocrk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jgkdrkev.html

esac
来源：http://www.52xcode.cn/Article/details/gt3vzdsczuh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3azljteis.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3tozzwyzr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3srtoujgl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oyugthof.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3qhqknmqg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3songsyja.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wupswcsg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3toorvjuu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3fgdstxnj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xafjcskg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3mcfzxsov.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xkxjqtcf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3wevhoxau.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3eerkqjix.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dqynqgtd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kadtwbln.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3tmanluuu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3hpbpyryp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hqppfbpr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3duzdovnh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3refjkrqv.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3clexijjv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3benfvdlx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3mjmyuuei.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lfggovak.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3kheyhuby.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3edgipvmu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3kksrhyrn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ymflctnz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3aavgzcbi.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zkzbzrqi.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jimoeiaw.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3gqausfip.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3nuoennmd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vpcukqxb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3wemhyxtb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3nukgdvgw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3zylrdojp.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wqsiuhuz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3enhyqmzx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ewfvgjuy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nlhflljq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3xqjbefdm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3hwsptzks.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3gxauiclv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rtphfeej.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3lskgbclk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3mmgimujs.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3kkigtzzj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3aoyzubsj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3nyhlufuu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3brbelfhz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3avoktgwp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3uztjacxa.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3desdehea.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jxlfcgsn.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3bltfrexo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3zzijbaoz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3lltfebwj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3murzffck.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3whnmbhce.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3vcsxjpmo.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ojglpwku.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3pkdagenw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3oncqybkm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vaoyayus.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3aszutvhe.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ijpcxthx.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3rldstczk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3jrktpzfg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3uiulywky.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vqtmbyiy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3sxmgemkb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ggsjjwhv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3oovlmric.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3mkjfppiw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wqbeglwj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3volqdrdv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3yeytmwxk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3lvloorvp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3onwqylhn.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sioubbdn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jvgswwze.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3atwpcsyf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3swbnpkgu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bvfsxjys.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3cbujfudi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ybkxcjdb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3jjpjwfux.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ywipegmp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3trbyzjwt.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3lkcfafro.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3zcjnbpgw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3vqhpbqkv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rnofnecv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ricdvvvn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qeuncpgh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3mfibvkyt.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3uizwqvwo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3bkmpjzfh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3lbrposes.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3fabdarzg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3sqoorpbc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3fkghbxer.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3zebjatic.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3bvolhmff.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3mdlwnkke.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3sjsxfgkm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3oiipbvll.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3rvjhpman.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3xarfnkmc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3oamzntyo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3dcetfhkp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3gabibckz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ipcvjhzo.html


<!-- 参考信息 -->