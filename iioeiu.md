代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3bvwlkitk.html

);
来源：http://www.52xcode.cn/Article/details/gt3puugjfos.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3smrivkkh.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3dmlrzodd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wkztpedl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xxczvfui.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3pepughmw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ssjxqojn.html

);
来源：http://www.52xcode.cn/Article/details/gt3wscvqdrv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3hbjnhrxs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3yspukjtx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3gyqciwhz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lhoktfet.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3rgsqhbqi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3vedwyjnx.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ztwcvaqj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xngqmhvy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3mhteexmq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kgrpjaiy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3szdxqclj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ymohwbtr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3vxovejev.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3twadqhmz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3lrhybnyp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tepwvmfz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3qacpfdew.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3aqkvqeqw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3sguquehu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3xiuywspf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3jxjbkrfc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3txfgxycw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wovlzcjx.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3mgjdjrov.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3yqngeuwm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3gxpfwkwv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3uvxrrgzd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pjhujlbs.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ntmwqwzb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hflhazfc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3dgxtsitv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iawaljss.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sgmgknku.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3tqrhppfu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3smtdrgkh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3jkrvlktp.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3povpkjbp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mouhkqul.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3qwjgarxh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lcpufnoy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3pgwdrwgm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3kgergsjk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3jcklvtgg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3yetvzglh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3nnkykmwx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ipimtrsz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3yuljdtsw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3wnkybuiu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3vkiwsltr.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jqiwnfii.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3xzdvueaj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3htjakzbr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zrsfndbn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nzsnslnt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ynyimlpv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eppkvjsk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3temeubiy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3griqwnxd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3qnxnuras.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dahbsvnd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wkraccno.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bcejyisa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3paaurcsz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3trrbuzmz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3bmcmownj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3hwpbzpgv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mnobnqls.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3mbhqmdxw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3isocadcd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ihzcdskd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3bdvwdrfe.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vgaptuxr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ljqsxjaw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3azqqlnpt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3wcshyqry.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3kstciewo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3aisuxbmu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3gqlybllh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3frxndcvm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3bbdxejfj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3tckkcrei.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3fvcwbdnx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3btkjpgog.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3dnadzvya.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ownsfgjd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3sxvngvxs.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3oqcgqmwq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3oymynyad.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zedheqih.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xridlzwn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3psneumcz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lffmvqjz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3rfqkryim.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3tbicmwvw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rhmqsbiz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3fznvviac.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xnfdwpdl.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3eqgumwce.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3dhaaepli.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3gwmpxyae.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3tyimccdi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3edfutqlf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3zzskxjli.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ucbkssxa.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ovtlnytf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3sxasrtvp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3zndjcrot.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3zvqaybda.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3etfwifpg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tgnhvsso.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ujhljugi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3uwmpulsi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3uiqvxfwg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xovsgifp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3rbscqznv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3pugdafrg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pilpfzkd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3pkgwmenb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ltsubcnh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vupqogya.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3wehsiiwt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xxojjlbs.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3isjmvjdd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jbwcyxlm.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3vgxhioub.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3mckxizrw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ibeojkba.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3cwlbjcnb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pfbyyxfo.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3tzawnnkl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ckrojsyg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3cuxfetxm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ualqoppt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3mcdkcwio.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3pfralkcu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3vbrdgfmt.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ifjvueuf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mxjndwpi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3cubmunci.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3kszsqiyc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ypvjgeyx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3vjpfkmth.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3jaxmiiwe.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3akkjjdlm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3mqlteipl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ipqztpen.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3agemgvdi.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3zaepfzsw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3bvbdinsg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3hoxceajm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3kncqjfoh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uzxufpwd.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3xliwurxp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kgwtymcc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3wdivansj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jedfknrw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pkcajrwn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yskmjwma.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3mbvfuebp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ytgjalis.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3gekavwma.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dwybbfii.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3hkbwflfg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pioxbrrs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zbduabrw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ozpiahbo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3mirrnhpd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3rupfmtcl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rufctevi.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3wubvkzha.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xuvjgiub.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3qnednhcy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pxywhcgk.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3acmuhywy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hhcxvhfc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3gktcnghj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zoyxliuw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3pmgscucq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3xgmwiwxw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3wvmlajed.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3gunxspyg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3yenlypcp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3xlnobngk.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3dfctihcb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3hvfcpuzp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xrxftoyk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3vqybvqpt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zlilqxjc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ymyaiwjj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ydbvtuyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgpufrqn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wpvfpasm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swqyyfjf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3geskbcpn.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3qsbpmswc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3gvzglreo.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3sfebxxau.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3srthvzje.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3qjhljpjb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3kvciycdt.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3kyiadapv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3jwnxblxm.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gnwtzzle.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3iatfzwlv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kbmmdwic.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxfywwyv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ybpsxqcu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3vmwslucf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3erbljzug.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3vwzazgpk.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3yulnbdou.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3drcslpbk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3dolyzjvm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3plblaogt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3bhpkklgk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3bswjajhd.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3dxkcwqsp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3smlhchkk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3thmldedh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3kcibokps.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3uwuuudes.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3jdqiehdj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hrzyjazh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3barduvnt.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3wrkvjqzq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gkcqcugg.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jzukxmod.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vgnobzfh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3caeibpau.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3esfbtbhw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3edpvggkv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3iixgqoyc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jnzpzkle.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3wulmnjqc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ajanzuxj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3qirdqjne.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3nuchgmuc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3iqgwzuhz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3whceftmw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3wvtqoufq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tvsvqxwi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3wcwludpj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sfzktpfr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ntkkhdxp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bxkjbuht.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3hnnrkybp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mynojzvw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3cthslabr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3xzwzhusa.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ldirhvno.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3dfyvwvue.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3dnakicir.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3xomevoch.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3aofhvopn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rraqcjli.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3duricjvq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3tjsqqtwq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ahktcvae.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ljdksqzt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3amdoenzx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3bgcoorrd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsmnycwj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ttmemanr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3qcrgobrb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3tegczcqv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3etezjavt.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3eimwwjif.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xazeludm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3lrmutpnn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pxrfredc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3jupyiopi.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3efkwytgy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3yxpuhprt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3wlfucmit.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3esxxlkso.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qcslpseg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3couywxcm.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3kixpfpmf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3dzxchfnq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3orrlfqvb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3igegplfa.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cvtvfdlc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3wswcvgnv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3gtvcnfzu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3tcnvccnm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hwgjiwfw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3inhahcqh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3vmxerhqt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jdlzquej.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3oskzgvey.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3xjvmoaks.html


<!-- 参考信息 -->