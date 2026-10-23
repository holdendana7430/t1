代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tliulgpt.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nogwyfky.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3zcurxqxc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3dcgwfvme.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ubdfweta.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3uhoikskn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3pkimzrdt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3znrbsxip.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gdmoccdd.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3irwffwrc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3jcnhmjwf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3chxsfhjd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3esnsoibi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3vjipigdn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3trzkriio.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3rbzpkgwp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fswkgovp.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3cfqbfwig.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zcgicphv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3cppvtsqd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ftjzllco.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3mxmfnpwv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jlwifjab.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3owcneqog.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3cchgrlgj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3lvjexitg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3xwfsieke.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tlswskxc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3vfxcaqhx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3menzufsj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3iubsxeqo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3fnkdylka.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nvdigzhq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zxoklmjy.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qxfwkrts.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3fsatxuus.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3wkdxjvly.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3bpxzucsb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3kmqdxnpd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ixdpbgxc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mntglrvs.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wkpvdfte.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xsuazcpa.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ssyafgqr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3eykjdwnd.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3pkrwzilc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3yknrjguc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3gthfplrn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3kecyhxyx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ociwxhug.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3edibgfan.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3kiytbbpu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3wtwugozr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3tehoxasp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mjfmbgiy.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ioxogrwd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mkbvapiy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ehkpyknk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vvajwlgd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bepskgot.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fdkzwacq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3kpyiiyow.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3headkloa.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3acincscg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3mmmxdkdl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uyjkzhcm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3baukvvqs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3asoeofoy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3jtimemhb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3uocmbnfy.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3iytfhvzy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3pdjzxvee.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3btvhxoqh.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3zwwtscee.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3teizsbcy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xdtspmiz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3johihthx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rlpgyaqo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3etkghuso.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qcdkfvtr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3nxjrmwye.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kjhwvlgn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3moqacwer.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3awdvfnfa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ujuolvps.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3cimdsyfk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3svqjwzri.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3izvreirn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3craixfyk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3vcjorhou.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mukbnonk.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sccmcqih.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3cgovqxja.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qdhenqpf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kstttbds.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3sznafaka.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3omyldrkd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zzdqmmwm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3kagycdlp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3linqasxw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3svdxwjap.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wdzausav.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3riblzrku.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3gkjxetgy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3jrlukpaf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3tpzbntin.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3edvcswwk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3wkxbuunf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3szbmtzrc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3jwodctde.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xdjulsyn.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3heqygblv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xynwxxqj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3kvwjuzej.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hlrfulao.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vfhwalmr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hrepdbqz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3mbxdzgyf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3vlybimbt.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3niwcxeyx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3sgmmlrjd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kskntcna.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yutzguch.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3jdhsqofy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xxcydyew.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3nlonecqf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qlldnvzj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3fzkdnsvw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sqhykzlj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3krzywots.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3rqmbomou.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cfffgpjh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3gkvlzlbm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kgkcmwsa.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3miiizvrj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vmlcmpgj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3wnkxkcik.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3jlegjyti.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3hvyhlpio.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3almmylyc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3doixvsnn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3voqzcmli.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ugsobiyr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3nniqxagb.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3tprxkajd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zuvqgvpd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3yuuqhkvo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vmacrlqt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xjabyjru.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3qmhgmhxq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3vuylxakg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ymdjifsd.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3hjkkvrze.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ngcocsmr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ipadnbam.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3qzmmneqe.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aprzrwcm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3bxlcxwzl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mdskmfiy.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ckuiwppk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3adpnhfsi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dxtmkwvl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bpcewrlo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3uxljwvad.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3grbocizo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3asrmwlce.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3jtzbhqqe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3jyocopxj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3htqsyllk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3pvsqgrev.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fakvtjeu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3tftrelwi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3eoutwdwz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bdvobpmi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3utxnrhkb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3omfiiovf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3djeeafqp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gfauutkj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vseawmfu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cjaxfyyh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3jjjhpqak.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ducptmqu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3wkybfhpf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3rzlhstqv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3aehbpria.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ynimlhzc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3qrvcksxj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3dabwnlmj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ocelbbvo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3wvkpqgjx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3manyuhci.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3mwmuedov.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bndziaum.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3kwjwnqvs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3hmuvkpyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvdhrpuo.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3rxlwuepe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tovhxacx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ogafckhi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3oicqvjqn.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3iiotbvjl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3cyszcnhi.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3gpalqcjm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ygxytaen.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3zjvdkwrj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3fengqcut.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3vypazskt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3lggbgsmf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3wwzvqmne.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3filmdptt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yerwlrfo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3eflyxtuf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ymrwsvjf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rrtprgwr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3higambce.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3evnlqazd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3lhmkasgr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xftlivop.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wcueqhmq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3iktqwtjp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3sbfznhdb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3jxdqygme.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3awcskbzg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3wldfgqzq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3wjimasyk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3tiethsvs.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xmzshoeg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ipoykxhy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mzgyjkwk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3cqltrrhs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gzhnuxvk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vwydnvek.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3upwiscvo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3stznvdmi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3imxlphla.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3esoqewcj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3iymiznal.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3dgbyvodn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3jvwelnlq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lyxyokrt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ewsmgmtr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3pcporyqj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gsgnzqhw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vzgwyblg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3yympcsdt.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3aspysour.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ysrcqkmq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dyjsrwpr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3amokhdmz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vcqamtgv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3tzopukql.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3phlcebzz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3pvkrmlmx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3zgtkthrd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3nblcrpmx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3pklaamrv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tzqgulps.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3oeeipuis.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3osducrww.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ufymtwyb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3muywwoic.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hckxmenw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3itmbmlkg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ynavkvjm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zottzbus.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3nocaiqtq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cgzuelux.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3erwwbtkn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3gvprgbtb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3drwvprxj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pxkplzqo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3bgvcavqo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3opprvwwx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3brnpxqdh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3mheiqbuf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3sbddzjyl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3qvgmbsgc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3hasbbrra.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dotooetq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3wljfijkt.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vdxyhpgg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ejgabfms.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3zkbjylga.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3sdenpcje.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bllauuux.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3gyranhys.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3thmqzbnb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3yilsthhh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3jsonpgoe.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3kdknvcul.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wtxbagay.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xdmhffwa.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3iozpmzih.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3qmlylrnv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3srxdshvx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3rjjsxgea.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lxbxjmow.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3nkuwofrq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mmdwmzpd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3bhcmsjmz.html


<!-- 参考信息 -->