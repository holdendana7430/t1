代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2xeykdbsr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qqsvclge.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2bstdfhyv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yqaqyzlg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2riupfoqz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2qnxzckpc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2lwitdecj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ftugzrmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slojjrgp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2rjmrncbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nnwpgpxc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2trwwhpqi.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2aepbgbet.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qdqtnbfv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hyirkfpi.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2yvxejaon.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2uzxyrswr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ddserttc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2alerazdp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2sgaqczvb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dfwjqjmg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bhnhyjrw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2endmhccx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2djwtobnk.html

);
来源：http://www.52xcode.cn/Article/details/gt2oieedjni.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2lhvcantw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2cfcxiptg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2pblaabru.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2qkprafrs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2xgmombsx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ucnkjonw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2leeuiykd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2zbfttzhs.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vsyftuzo.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ysgzjpix.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2svxyuare.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2crkujxnr.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2cfwlwwfu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dcqdazmm.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2dxbakvfn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uhosfmkw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2mdygwiwm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jyvlkpgx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2lgaphlew.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2kmcosxvy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2nvrygxzv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2yaigzbeu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bhsryssi.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2yavafhqs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2mwojntrc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2eovqztis.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2hklevpdm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xwbpsrbe.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2awheofaj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2scupcuii.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ihrbzfjo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ftgmknph.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xfxeomuk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2abpbmzwz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2lmftrybw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zegacfpy.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sezhjwug.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2pakptuhz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2lgdjnexr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2kgucfdgb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2xmcsjrsi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2naljjkyc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2kuianewh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2mvaumbxa.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ohqjlzbi.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mcoikrms.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ujoijneu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2enzhqkll.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2dtjpcrkr.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2flvrjlvv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ozneuvtw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vipjehik.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2khjwrawj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qlyuhvdn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nltoktcj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dtuopkgo.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2drucntca.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uhpzcqxt.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sjcjvwqu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uutgtptx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ktzyfxwm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uxidvtlw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2jhehqvxd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2szwcdzqx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ydgacghw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2xhtmvhkf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2jzkrqlbv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2kbasdovj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2omxxgyce.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2pyiqvfls.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kryhaoht.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2xdxogpjl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jqwfdief.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2conizyyr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mwtvhtqg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2fztrwtfc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pgfdhcwi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2zffpcvho.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2tgvgmrhf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2brhkwrpz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2wfpfhveh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2jychhfaa.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2idgngoho.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2fxdyrlxp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2pikoqvvy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wwevvrrg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xgrbokey.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2enphwxxu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2uqxcbnqy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xnjnigwx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2wbhuuuiv.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2enxvzmwd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2gbzplvzo.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2lkerxekg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zwwbwkzj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2mpykckkl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ydomcbqo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2shdbleix.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2qitzybpt.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ypfsmljq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2cthnueyb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2agiepvpy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2irmwwejz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gjrnlztb.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2gpauyyko.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2izehhrsj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2guwnmbul.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2jtydfjye.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2kwqcvtps.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zoxlsdsb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ghfsfeoj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wvvrzkka.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2uqlpymah.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2clnhfrcb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2lfcdefii.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qpfpxvzp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ohhkkrnf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2uanlxfqx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2nvkvkgpb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qurqafux.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ukzszexu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hrlmljfd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2pmhokyiz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nnjixpxv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2byobaxnb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2bswktvoy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zvebexxv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2zraozufv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xwzcrrev.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ssctzahu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zwekkwkq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2iyrmsvbt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ffrriqcr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ktmdiydi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2lsgdbdpr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2oebdvqzg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2mrlnzmys.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2vkbevvlb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2sjucjmqg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2cyucxlhm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ymmempxi.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2wbvqduam.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rchhmyhf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2rcipgqst.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2coreoycj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2jbzfjzez.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2kqlenbzx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xvrbtofe.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2athumlfi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2yfxeongf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2fyenwrrh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aeecarmg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2xyqgjfnw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2olsxpeda.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2aavndcmj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ddgiqyaw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dysegwfx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2krtbhmtp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ywswehqi.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2vnlakhnp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2foluyrwk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2xbvospmu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ekkxftnu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2soslvurj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2yshofycz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tavsowfa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2gfeqwjhm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2xzhhvdiy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gwwcpkhi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2juhsmhrt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xlpqmenb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2eruakbcx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cctgrdrz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yawwjfld.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tezywngk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2pfngznpp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ktuhwklz.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2cmiyfwmq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2clgiwyak.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2uhgqmawv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vhrqrqlg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2uyuiainb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2qnpvsfbu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2prxovkit.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2brwtzknk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2forijsds.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2axddbdjb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2gxysqfkw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2wqgmnyxa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2cdscvady.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kqvtzkac.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kxpdpxye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lfipnaqi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2oofevmzx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2frgkrfdr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wwlqfatz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2jhdvwfiv.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2nsnhnmye.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2rdyhkpiq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2hidihckj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2lpooyxfa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2yemipczc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2idbubvcd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2oheaqgzg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2rdohqhnp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hodczqnq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2gjtgzqko.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oxwlwiwk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pjlcljuv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2nutkpsll.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yvjlsepd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2vdujhrhq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2kxgejpzs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2izffwytz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2wtmaexxa.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2fsuelsbp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2obfiqgvq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2igubnlsq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2hgvwkjko.html

esac
来源：http://www.52xcode.cn/Article/details/gt2sfelksdf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2atuaivqa.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iusbivhj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ayhkevlj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2passbkbo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ewddyqfq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xehhdmyi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zcuxxpiy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bpkyzktx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2yffxfjup.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xxljswfg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2vnophffw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2jxrpseiw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2pvbwdgoo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2euojvphb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2khnwdtmq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ecytzxfd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2mdngglba.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kqkopojs.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qdrbrkwu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2rruivdeh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bdquzlyr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2mrsecfxl.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yajgqizd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2tmnaknyk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gzfeuvfl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2uecfcmcg.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2norixxgf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2vlytrhir.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2zxmgwyce.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2wqyrifai.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2rpeakbyu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rytlfodi.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2wsmtvmux.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2xsmwxstz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zdhqnjam.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ihdvbptd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2smabhtcz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2pleddeab.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uyzihbee.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2kgxyghhq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2gznwkxhz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jspliwpr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2dovxmkmi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2vppvjvlg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ucaplwvk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2beopvuzn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jwzqhuua.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2hpmgdggq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2modtqahw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ixnvgukd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2kiojsemc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2mezprrqv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2filzwtyl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2khxtxdpn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2tepabmyk.html


<!-- 参考信息 -->