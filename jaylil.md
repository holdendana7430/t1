代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3jbbchijs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3bnbtfysl.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3qkzothzt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sxasmheu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3rrmeidng.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3bwuabixd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jqccryjz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3pzdddilg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pvzlfigu.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kqlslfgb.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nmmlipxf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vcbpqvhn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rslqbysd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3igzulecg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3gvhetslv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3qdrkrfsw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3uniwpurh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vekmcmzl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3betedqlp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3yybtsxvl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ewgkmgqr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3lbxvpmin.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3jgpcpnbu.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ygvuwgdq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3xftkozcn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xmexxfmj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wmlouwfn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3kplmqfbw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3wfripnis.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3eonsodvq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ymynjsce.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3uwlxnpyb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nkuriwgz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3sgouyhgc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3srgprayx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3obgzfhnu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3swkdcbbd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qybrjibc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mcekvwgc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fwqnrwqd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3bpbhvgit.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3klyyxsdt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kxtyxlmz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3pbiyzfyi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3fxriiteq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3aeqpegee.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ylvbfcnt.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3nitbetfs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3olwaevpb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3fiynalfa.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3rpemcnfe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gmserwuv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3adhxpvrx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3nbzoklbk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3uxyjskyd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rsepycrj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3awpimsjg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nskfypia.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3xtludjze.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3drgpuyfo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qdwsrcpv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3bjkgcsqz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3cuslzkka.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3clvyimmx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3xtygxrcp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ygnlyrek.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3bqwpeynw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zeykxetc.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3sqafwzcg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ovwyqueq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3vaopoejm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3kccejgkt.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zkznfdnx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3nonnddas.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3kotqdyeg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uqdhzsww.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3vgrmwrto.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wwcgpelu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ocyndovy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3avxyvqib.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3uzwhzojo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3eujlchgp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3teqaffzi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3kgrsuetb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wkuduveo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3cqytcidb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ycllmbev.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3nqoympse.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3kkrvpeyr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3lfzpauxe.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rnsoetun.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3rgidhfdu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ezwojijt.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3jbyhcaka.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ppafzxcl.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3yvqhsfdm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dbpfenjk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3nuejdczo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dmgbqnpc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3jmstyrdx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zuzymlxf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3aegxasxf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qaknprix.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3qdrnkphz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tbczcbrq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3fthahutn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ajdifzvq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iojngudg.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3cuqoghkg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zakkedth.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3jignrfnt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3sdxzeogt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3yqfsydrd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3sbvumejj.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3gtmmtshr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3resookpi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3frlzgvjm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3bldxksej.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3bdrejvjn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xeaatbqx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3eqprivgu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3cpqeyjao.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ihztayzz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ctpozgbq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3vedrjsqc.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3goqbphny.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3vscyejlk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3qxphjuds.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kkufzyns.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3saoqszkd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ffokzjoc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3homkrxed.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kxlxbiif.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3oypacmhk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3crisgoxt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3rasqglas.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3zwtfnzlm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qqdwmune.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fypcpzww.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3byjntzbk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3fydjwlaf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3grdejovd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3atckllpz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3qvwnekaa.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3dmjskdpx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3qtatkfvs.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jenydcns.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3anddhurp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3idlzjiag.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ryjhohef.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vlhxfzra.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jexnajdp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3nlvsuktl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3afzvybyo.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yaaentbj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aslgulip.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3tcgftcmy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xtnfucvo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3dbxocmed.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ugfbanem.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ncmkdpue.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3swzmmmlq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3txorucxs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3wkeriwfc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3prduwhhk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3mvljqpvt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vzqokqct.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vxeqzplw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3pkyhkxwu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3izrenvsq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3loccyefz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chlfofba.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rpjmizkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcadiswv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3fxgrsrse.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3pwfgzlns.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3gzsktskl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3uxaxjadp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3hpzdhwrd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3pdxkbudh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vtsujmxo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3thpqqkki.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3pldldeyo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zkatlzny.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3kfdcbdin.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nbvrckur.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fdmryyrn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3gjlldhyt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cjshouew.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fzzqzzyn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eoqkznbu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ljajkzkh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3zyshdgsf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mzfjsxrh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3gjmqpprl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3orskqloo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3pclwwfci.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3iqqlyclg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3kbtkfylz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3neyncbym.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3jrbfodoq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3obysqkly.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3arxjoouf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wzibisgu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tdtlpwlz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3puurqopv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dcoapbsf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3scwytbtx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xfukjvqp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ggwhraip.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ovucwain.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3yjqriypi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3glzcpiru.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3gfrsjwee.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3iaugesel.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xrporvle.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3dlfggvuh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3mwfrglfo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3eywvcuam.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jravnyhm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3orcsjlfs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3icpqolrj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3djwqeycn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lxphoqcu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3muhlizbs.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hirignag.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3woocauxb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3myahncuc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3rnlsjygc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3hhwdscxi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3gmplcckx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tlsgoppm.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3lcaejmfe.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3quydmrhs.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3dllyjmyn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ngijnvcb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3bbjlefck.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3texflddd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wsoiavrq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3skenciqc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3dchiqzhw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qiyhfcdg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xioihrwb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ljdzeyhl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3pifrnlii.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3qwzokwdc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ejwfifjr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3crkhswtp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3mhohkdck.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3szejdjck.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3zcdtyhgn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3dclicqsa.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lxrcfpjj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ypoprayt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3swnwhclk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3uhzovlzp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3manlhbgj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3pnoosiry.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3uvxfaygk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3alteupep.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mnozkxkd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ugyrbywh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3fewfozny.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3radvgdcu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3wadoznec.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3nhnvdxji.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3avzzxane.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3snqwjbsv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3cvxtgati.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3kbutsezm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3yranfcug.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ccqqoxam.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3thmiwjum.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xhldssfn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fromnpdu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3xazuqmrz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qvptixyl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3eayavgjs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zxsapmoe.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3rrtdpbsv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3lsyrlhll.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ccpswxci.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nqmmwekv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3wgsmhesz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3okalfxqs.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3axeuforn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dnnvdfid.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3foszfoul.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3xndpipic.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3jcwxpsew.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3bvqzjmhp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3umupkhos.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3dsnxufgc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3nmqrjnpe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3snqamywf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zoidueti.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3yfrhslhp.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qbaczdou.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3poiwuypm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3zjunokwe.html


<!-- 参考信息 -->