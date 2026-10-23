代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gsaewvei.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3tnmsiuhj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3enhffcga.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3femimwkz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3fsqmzpco.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3jpiboplu.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3zgfundrv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nbjnamot.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ivahecyy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3tyipjlzl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3wwvsevbq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3jmxgsmwh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3acaxzmvx.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3eqbjmwqg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lbphnfkb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3sjtlwgqz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3zxgvbypc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kmoujlkh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3wivcnims.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ilwemimq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3yovmtudj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wbuuumqc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zmmehsot.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3tbsxkpuq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hscjageq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3mbjwfyjq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3caidsxlf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3mrjjuuiy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3hhwzckrm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zdidjxzn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qiyioswn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3nuasmncn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3cvkwdglr.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3bvujbnlc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dxiublsr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3prifsbls.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jbtkslby.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3eoowrzvg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3poethldx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3eyefgkkr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zbyqlroh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3yzakccfv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ntsshtmk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3fmxpmtic.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3orfwbyno.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tarabhdg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rspuscyh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vacjsjwm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3limpjjmy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3dxougdxl.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3dnnlpewt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3svwksbii.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jwitsswi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3gkropkmz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3sveufqys.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fjluzszr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3oaypfhke.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lfowcfac.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hpkcvqzc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3aavtykov.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3unqudflt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3oaztxasb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3jogxnwjw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3mulebguv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ymlbrsuv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3awibspmy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3yxlkzloj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3bbvynaev.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3aluoejnv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3uquebhod.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3qxnodyid.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3puerzipa.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3hndaowvq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3xxfjovci.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3bchqnslh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3eecvldfs.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3imnvyuer.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3oqmqjudb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3hizbdurh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ngrwqdch.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3lsijisrn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3horjqlao.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lisajpdm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3gzcxlrqd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3twkmjzgx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3usvgpduz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3lakdnlbt.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3xizavsou.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ekpuubht.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3oiewxtgq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3tvzqpoek.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3peimwytz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kdlnbddf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3hrngmxcr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3amtoyzss.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ctbwokdz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dbezgbbl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3rkvtbqdl.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3hzbcohib.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3vbnrweee.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ooydqzrv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3aspuzxvw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zdjxoydo.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3vipltxgw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sdgpjmbu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3frbnwsgd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ctjtkxay.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3tyesprut.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ecadzoag.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3hycrpgkn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3usjdiosg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3evkxnfqd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3orvjiyzz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nokffpep.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3loquswaz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3chjkjufv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3untfqhnf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3vzxyowfp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3fddbuxto.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3uupjvahc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3gzrvvzah.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3jdkruemx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3fxrmvtpp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3rzywxjqf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3fasilfxy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3vvlzsszl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3jpplpfyw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3eelhyqwt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bevlvawi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3dvpxhhks.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3nupgexvl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3lwvnizrp.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3vycmgidl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3lovsjyld.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3piujfeuf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3atkvsewl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ejrhocdt.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3omywapnp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jztrpzbb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3zxiyfkni.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3khkyrpth.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wwdesadu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xrxqnjbe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3pcczxykh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3mihgaufj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ooyscffn.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3lduzrmrl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3bdlsyczw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3reywkrot.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ocouzffx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mstzesoy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3kjgdhpfi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zktdaqlt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nolbixih.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ujilcqzi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jmabcszd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ckxwhfvk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yadbbswr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kiqojhxm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fembgxgo.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ffksicsb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gkowafql.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3hezlkmvx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3deltbnxf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3wswoqtjx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ihtazytr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3fucmhqip.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3veyusawf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3aniojeyh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3uqiscwml.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fpzamiko.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3vgdspmpz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3zyacmlpf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3advgzyek.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3pnojdnuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhdrxlml.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3brpmybxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvnqjqki.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3cvpivdgw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3vgdjoolp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3jlwqobef.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3hynynyvv.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3skkzgumz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3laeqjrml.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3xsziiysz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3igulfhcf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ntsyfepl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3oidratep.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3dtpupizx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3kybvmfql.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gayzcktl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3rflxuynm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uzzoojdn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3errvbdww.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3dpopbcwm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kfcdfkes.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3mbmcckpi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hwljyboq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3xlmafrub.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3iphqjsiu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3hfdbkgsq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gdapiiqc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zpkiljlf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3lwlsxini.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3glkzynpr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3mxwjyoxn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xarmsixc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3enmpxwqo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kkfkeygp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3qwtpfskz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mjoraric.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vyxshpes.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3iwccokgl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3tjkmgpsl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rublumxo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mabktilz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zxirmtxv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zqekzbpv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3optxenlo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qgbodejt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3eiuerodg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3oxilaztr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3qgzaxynk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ebagrque.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3tymkvkqf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3myabrqsz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3kjjqbovs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tnlrdduo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3hsglfywy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sehgqgxz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ynsnndzm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3svkiyhuu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3fvhqcbbt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3cnpazgmh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3zwcntple.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3rwpriisq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3mkqoavbc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3fczeztiz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3pdgptpvj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ubvcwvaf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3kzbyheof.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3drnzjbvb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3qbeogenk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3khxbxqfg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3imqhcvcg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3dmgvndab.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3coknucyt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3siuhtdfk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3wqhyvfjv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3qthwnsnp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3aicxrtcr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xdxlbydl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zshvgyxy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zobnrwfk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3mpyskhrr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3tbpjbooc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3hxwzadwk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rrogefjj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3hecozxuu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3hwkyoznk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mrgvwgup.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vrcvdwdw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ocbbhrto.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3omiuaden.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jruxlfok.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3vudsvkaj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3keipnbgg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3yjzwvzbr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3twcauxua.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ecsszkbb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ltielwuf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3rzclqgbv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3eidzjhaw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3vjiagrqp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3beuvvrrz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3prdwavyn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3inltglgf.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3frggkaqc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ufgpxrtc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3vfiaonxo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vtwdginf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3qayedtfp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pxcprorj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3guufvrdf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3elxbwpky.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3pwvanshj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wkjaqsnj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3zoveitjp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qsvlheos.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3yuemxucy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zutuvdek.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3jbwvqmnd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3hhyrerah.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vptcomlo.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3qkcjlsnm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3dozdjrez.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3pqruzgtx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3whkboatr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3prxgxwqe.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kncgdsgn.html


<!-- 参考信息 -->