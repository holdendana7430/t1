代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3nmkqwsuw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3xmuphlgi.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3oogicoqz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fcxjboxw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3hswunvmv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3mccfvytg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3tnfwjzhn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3vedtctrh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jxdnhlrx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qodirkcn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xcjpmusm.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3kvdqgyke.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xfbmyooj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3scwectmi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ynzcltcu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3muyrkgis.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3agcejjux.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ztpknpna.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xfsgmbnd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3qxrziloe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3sjiygdcd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ptcloopq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ndidolwl.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3zvznkwvp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ebodvjht.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ucceajuv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vlkurslu.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3knudrcnc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3veshpekx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3efujjwzo.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3epvoxcrf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3sikbtleo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fdewhkzb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3knvtcyof.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gtpeyncc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jdttqsik.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3akyqicve.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3szpgxlmk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bntficzx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ttupvcik.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3aysftfgh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hiqicesm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3taoigddq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ehjlsmyo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3qkhofdgf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3numbrvfc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ybkbtjdc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3xfyfvaog.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3sttlvshx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3uazqxyra.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xovqaohi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ipbtnond.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ypmifyfp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3faacfpxs.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3wgapnvsm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kxkflomy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3fxzzbpqs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3wdvumkgt.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3mmohhmwh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3dfrxlbei.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3icdohybj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ybwugsim.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3haoqeccz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3wxcweyqc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3mvkkulhp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ydieurbw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ofqvebcc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3nbcbsefd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3xlwmcghc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bpnfypkc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3gskcvpkb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3sanoksrd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3fhzzxjth.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3fcbwgecz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ggqmmwxe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fcgvpmho.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3fdgphive.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ryksypio.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yzxpgsiz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3foysvzqb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3urpmchsr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3dsyxrlfu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jdlnkwdr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3agjsbtvs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ivkxulhy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3vaaxeznl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3pbitbfwe.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3xvfbnmdg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3qtgkfkav.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3firtqzwc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qospdotx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3wwktfrlp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ciqxlezp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3inpzbtke.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3vtybhggl.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3lgbjmqru.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3trpamlup.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pqfazzdj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3nqkuhork.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3zsafeatz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fcmegtkr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ejnbvdyw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3egwtnbrs.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3pnzcwyko.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ceimghkj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3dknornxk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3bfygmmzx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dwkobive.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3gaigyyzk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gwzonjtj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3rjfpuirh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wrrktzhn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3nnokctxm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3xmrcagmn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hyamokux.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3flgnbugc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3csdkvsvl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3xyjbwrsf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3plewugny.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3sbclvale.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3clougrrg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3kepgfpbh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3vzzziwwr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3aqpawzlb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bwiybbzq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3zvsvligf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3wooohjsj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3izntqrjb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ablwnpke.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3xwoeubbg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3esdryvfr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3hnexsfgx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rarkaioy.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3yzvkjgao.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ewhkwrni.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ymwvewir.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3akumfhbe.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hrsynkzd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eqzpgpan.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3vaapweje.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3fkfvyrab.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3raxqqmzp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3haaavptg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3cslahohv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3kamlthqm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3iyhdcoya.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vfvqduzl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3xmmyzlmc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3fddmnmxw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jchazptj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rnwzaaqn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ojzfldhb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jftepimx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ezvpyngx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fcdqyxwl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vpetllkm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3kxrdcooe.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zukwbfhl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3wkajycwu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3qmyjtafz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3xvzbksdt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3fygmbrnf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3lukbiggc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3enmrladf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3idqzhadb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3rscotlxh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gnmibawl.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xmizsrzl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3czbnzaxr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3anmeubwy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ydburfth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ammfwyxj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xpyqcskv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xytvdirf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3pwecegbt.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3svtkdsjb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wwesaxsd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3xqxnrmhg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3sphaxcsk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3vgxlilbr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ialumpto.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3qqtbxqqi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3spizqlug.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yzyvalax.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3bhgrrnps.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3sukrntvp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qucbynmp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3edmhfslw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3glkhyehg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3acztclou.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3eghvppyi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ewwtrrtg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nplzwvhp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3yfloxwzm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jcneezgh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3dlnuajhz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3jvhjxjsw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3shixohbs.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3xneazccq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mdrhnihj.html

esac
来源：http://www.52xcode.cn/Article/details/gt3uvwmrriv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ptrjadir.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3pbqudajr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3naczplfo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ufmnulyc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3wyhgqkap.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mqjgcijl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ftqifvli.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qzsnpwdr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3fylwfbrv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3skzuojuq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3yyefrdgx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zdyzfpaq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3mknbmhjl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3zgxjtycs.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jfbnsahl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kiwowtsh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3bkdhqybm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3gjbgllez.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qwrawbtf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3alaoyorl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qrmjoulj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3acvhuuad.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3quohcakb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3etdyznmb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zhlwnuwg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nmddxkxi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3zthzfiey.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3fbqgfwpt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3wsafvwkc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3urgzrzvx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3vhdrwwya.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zfivqqxz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bfxykvuz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3xoassyce.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fodndvxk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3kwmxanym.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3iqcjhfyo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3mgzvitwv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3iakdpons.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpvuqvio.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3owmoemok.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvklsjes.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ffaqiqeu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3klkjwhpx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zgzpsvmw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3iavbyfsm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3axcqynnj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3acxljcwf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3zbbkfzyu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3xrpncabp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3bradhtmn.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yejdmawl.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3gkctterd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3dfxrrekq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3vccbgnsk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qmdqsqtv.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3opeghuvd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ycqsszih.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3rtdlokux.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rvkjyusl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ukgfchnq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3enresmmk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3shgykyhp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3rfaadzax.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3dasqdrix.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hoekgecq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3pdbhcjvk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3eotyhxxm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3pnattfwu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3qvhihdnt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3gkypawov.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kbogkoec.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jigyhpwa.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ccssiuyc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3falpcujp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ubrotabn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wtthuwlv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nemmkosk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3wlztnkht.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3wrtseamh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ndgxcftl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3taikkznw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3weexwrma.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3dwxqgnzt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3oveirihj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3zbroxqgd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ohcpblii.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3pydcssgh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yhmxvhob.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3cnwtetgo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ftyeoyrf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3vaxkiykw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wmrckzxz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3rpzmpunf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3bkxqkovl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3hztazkyz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qokmqbbt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3uiygcmjs.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3glaekjmt.html


<!-- 参考信息 -->