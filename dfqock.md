代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3svyjwkvh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3baenthjs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qgwyezon.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3klrlalrf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3iuwkhpvp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3rnoulwwu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nshzakji.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3nsmueujo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3cwjsxthd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3yrmsmsmm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dscmfhho.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sflzihpr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ywvxdwrj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3oxinxlxz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3dhckhmof.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ivtlroyc.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gthjrfac.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hiwkedpx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3exomzpsf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3tjpptiht.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hmanhfbf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3sadpgiiz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3fymqaahe.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3cphvczha.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3kswldcjh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ljhqnylq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3frmvfcva.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3jppbknep.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3sjlkwvaa.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3muovyovj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3rmhgilfg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3uphjyqip.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3pmjzjely.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3emqtzjzh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hwyzocdn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3sygmkfwe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3tewgfkco.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3cjkxenfu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ccsdaqyd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3bwlbsdcr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ulrqcfyq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3hkwzsdhb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3irnwgpxe.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3laibcdxn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rwhngjjp.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3bagtjtzk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tngxoepk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3farddnkh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3guyqgvkg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uwbzkshd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3sjijrkpj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3xqjilbbz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jivhrkjz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3cqlgubim.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3dhltlmit.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3faqvzxzg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3xofrsqav.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3palgiyqb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3vcllfvfy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xthdetuj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3mnfnabrz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ayicyrnx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3wxnqftaw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vqkvfoqj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3wqrnclgb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3bnhrewsi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3mxetwpqf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3tdkudvra.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3obnytyrz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3qwthgzqp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3wzxnnomo.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ucrxwloc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3vuhelwmo.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3slxvfmbc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3okkjikqw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eivugpkr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3lyzoxqbz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3muqqsfog.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3crysmvoa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ngyxhhvi.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3mrjyydor.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3kuzntwdn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3jpqckcbm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ppokhvkq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3hfzpbtbc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lwsvmdri.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3umfenwvg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3pbzatynm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3mlvvcqns.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3iluhwmnz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3hrmukrgb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3joupuyhn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ifparncw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3jcxlzbto.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3uyafoour.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3kdvkoedm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3zyycwbiq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3tfjciyjc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jgnanqqd.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3hmrfhmfe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rrwfbsxw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3zefksrfp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3qsztpefc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3fdjlysce.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rvuhnjsz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qukxnzdw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3flrkaxrk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3hnocsrvb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zcoxplbf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3mjyihmuu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jtoccnlt.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3gqnyglzp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nzfqkrge.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3fquczabv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3fbsfxspc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xnnpbuih.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3onndldlx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eautzowx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3avtfpqkf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qrghnqdl.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3dyimzfjo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3rtainold.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ppoekkbd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3oqepbddf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3uuumkuxl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3xocsymjn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3plljjdjb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xpxycvth.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3qrrtojfs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3grhbesmn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3klgstunl.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xxmohgnp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ysbemjrb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3hgvzjasq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3bulidmpb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3rnvsugao.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3msmlkigt.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jcememcn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3cwbrmgtw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3bfvgnevd.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mrqokdim.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zunbwkzl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3dlqcrahx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3nmnyfhlp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3nyloqzoe.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xtngmeii.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lemlcbjz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ilkaxcft.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3uesbjcnz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3unhzebpu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3zgrgxmid.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3qobslgkt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ncxngjye.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ujrptjva.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rwxmycnq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ctrraeke.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ubtzrlqt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bezeisbr.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nljayljl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kznfkwdd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3jhkrpupv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3slsirldz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pitishkd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iammqses.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3kbiweoxo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ekdextyx.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3zaizvvea.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3exvlurkr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3tafmpefn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3jgjlzfhh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3tlacmlxy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ilkzdynu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3npmxbojo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3xnmkusdu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mpsquksf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ncxojfau.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3uleyntdv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3hyzxhncv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3vjaddvav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oxxobecb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ykhsnljn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmerjayx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ywlbtmwx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3isreioqw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3kaoajyrd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3uirtzbbw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3mpouwrfl.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3xyubfbkl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3tmqlfbkw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3czzxiwue.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3nrcdqcuu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tkymdglu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3rbmliqbg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dufkeldj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjotakwi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3fgizulon.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oazuxvxj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3uzwswxhh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qrzvcmxo.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ifftgjpe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3llgtihga.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mkvjixqa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vkquycyf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3rxuzisqk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3jycovtba.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3lcbbhcly.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ouwqkmom.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nvwgxiih.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3irhanueg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3dhoteofn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3abirgpkv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3yvkavulz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ewfakedh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3lukrkwzv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3spipewzm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xvvvwweu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3xaailrje.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3tlvygkpt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xmlyqrju.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3gljeuyhj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ousorssm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3yaaosypi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3mtjthvht.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3nawztejx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gisrakuo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3lduzbgjs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3txjjxzcp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hymcxpkb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3maronmxx.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3pawxkxrt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3dprsqtti.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cdgzdras.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3jrseetsj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3buojzvgq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3xfgwzxmt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3fceiwzzi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3qsezxyik.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3cacglymf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3msavhori.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ykvfpqpl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3erbqohph.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3jvnuaxtd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3idflgbpd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fzaiovjw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3bwhlhclc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vsyyutfy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3hyiszpja.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hyocdoox.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwxgkdpk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3eipuxiob.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3luynoivk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3acgilops.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ucaqopdm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3hjksromv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rctapgdc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3quojkuvr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3qgqdssah.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3fgtmdifk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3qckqfzrl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3sdzsbzuk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tzzvffie.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3eygoftmj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3cukxxvej.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3psfcdvpk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xoizblyr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bmcaxgwb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3kwldcwip.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3kbjtlvwv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nwmnatcb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vhqzmcdo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lvorjywe.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3hpzgbfud.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3drwckvrg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3knjyeotq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3igsbdcjc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3tkmjxzrn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3qfqccjhb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ayhyeyba.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wunofatp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3mrbyvxvf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pztkxljl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3brdefivh.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eswonwtk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3wgeilxhd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3tjtsribf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ryqyawmo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hwrecdyl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ebdiqkyj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3yhytlamh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ezpmhsde.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3qxeauoox.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3adhxtkyp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3nvjvaqii.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xjuvbrbi.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3currygle.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3bejcmqdj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3wmmckvkx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ktqbliub.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3xlopxakk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3rgmjjviy.html


<!-- 参考信息 -->