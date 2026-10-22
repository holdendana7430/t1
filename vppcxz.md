代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nsomvlmf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2fwzvgdca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yvrdqgeu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2mdusgcuj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ljootrhx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2oumrusjm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2txhdrviy.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2rdwehezr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2nyzhocjz.html

);
来源：http://www.52xcode.cn/Article/details/gt2sjnjjgsp.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2qtpgydvo.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2edioubfo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gzovsfjz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2mfbdscrr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2kgthftaz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2tninvglz.html

);
来源：http://www.52xcode.cn/Article/details/gt2gvfujugm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2bebgsklk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2pytajpnr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2rjltlyni.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2pusrlcmf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2gemfhsip.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2kotwfkpi.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2vmqxrnrs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2dzozhhbe.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ddsklcsk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2gqbihyyk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2negtfgvv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ijnzquyg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2tibsggjk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2grafcqin.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2tmvlqtym.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2siovwcai.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2sgxtturt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cdmgecfl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2sxorufsp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2pjxzotdk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2olhwquvo.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2efkslnvl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xpfiogir.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2mvmiritj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2fmsdlraw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2kkkctmdk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2zyufrnqn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2upzbgwto.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2crmcntph.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ibjbigwm.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2fkromkly.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2zyszoilo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vhkjlnfi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2kfznrikv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2sgzsgsqb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2qezaqawz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2zbmwajxk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2pyfzttxk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vzokymyu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2hwpjooif.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2kglmujcz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vhfyhtiz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2lbxxwccx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2adminfdi.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2dlvhaetz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bsevpior.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2azsxtydh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2rydxcowx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ygzhdxfa.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nyqpcckh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bpibhihu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ttdtirmr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2yqxmjawr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pbxuetqu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lkrbfzhg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pmeagwjf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2vbfxrcgi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cjmsprpn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2xmntljyr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ayvdtzen.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zkneaocj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lqfnmjju.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2cimwvhbw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2mekasnru.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2cjtrfsvc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2dldmabuf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2teaxltfx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2bbxdavrl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2euohbiux.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2yiadkoii.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ceagpkam.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2kqksjcfk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2iledgnfn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2vsnrfjgt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vtnmmijj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2soelzszp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2noulztyj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2omyytpwm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2sakpsimt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jgiyjwln.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2hgdijmvd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2maomicnx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2iysawyuz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2vvdkmhvu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2edqtoffq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2jejxcuue.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2judwempq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2kjzppnpg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ixhvnthm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ktkeylom.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2mibqarwo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2nrglhryj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2yfibykvu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2xrnvajgs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2uvmwdbfu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dydwslik.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2odoffbqe.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2pfvlipul.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2uvbanxre.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qttyyluh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2nyguqqpq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lceliofh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2fybqvomk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kilkmdvf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ghdsgram.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xjezhqlj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2vochmcyn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eaxumzym.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2rpqdndxi.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zgmphkiy.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2tevtzpof.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2yldjnnev.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vhmgtxxo.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2uwvaughm.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qrsqpjyo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2amtzayie.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2lxhddluh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2olzrhdtg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ozynwqea.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mfhblsxm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2lzpgxmmr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nyxucpop.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2jfuvchze.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mfdwknki.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2aldlctwc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2bdppaskg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2memopipl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2roydaieg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zhjuemyi.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2qsmdzxma.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2denysikw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2kxucxltb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2nelyatgi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2kdrlcboj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2dtmyoafa.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2nddqonod.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2nzjprsar.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2lehgsfhm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2zwtjcgwr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2lwjhwheo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2pzyzrptf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2nqnedfwr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zexnriqh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2lnfecood.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2llmjirrw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2luaqcrvr.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2eulqdhis.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2kdqexxkj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2asmqkthp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2kmolvmnj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2epyypaht.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yswetmpi.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2mneihieu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ilxyqbdp.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qvwtpnmt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2pftdqugc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2trdibntm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uzcviqjw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lffzqdjh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2dpiprvjq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2yddimimv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2pzuevwwx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2xryoypzk.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2uizpywrp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2cekcbzlf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ilrvwigz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gfgiqhoo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qhgvdgdy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wqovysqa.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ssoysrou.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mocloegq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2xhtsjuzd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2neejnxmy.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2sfdpmaeu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hlkqjadl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2utfquqmi.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iamrqyof.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2gevhvazz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2yjbwazwl.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2fyapgwyn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2pynudapd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fpjqyrdn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ynwtixxb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2glgehqgn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hosuxoiq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zhqqciuq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nyhqwjzp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2trqujldm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2goofwldf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2slyqdvis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szgpytxg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jivcwrpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jutdimeh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ogffbxlv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2wkrersxz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2cibarhxk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2crsdggwe.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2indnnbeo.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2getqaefv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2hsywhpon.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2wwwypxfu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xrtnfehp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hpmxwcih.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vhypddlz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rgpovoyv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ennflxmz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2krkwxhts.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2nwcggmfv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2nfeolujr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mxeoeezr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zhgmaped.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mfcurvol.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2igfzqwds.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2siypryug.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2grcodkrk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2kczcyzzq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2kljuvegp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2covlrnqh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2njytexbq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2qmwpxoks.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2uvhncinj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2prkurgaa.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zeaxipux.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jfatbykp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qgdhjsht.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hrxdvtat.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dqiakahq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ginwphek.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2knhuleue.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2brpbaeop.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2qlwpcqcz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2eiwrrmly.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2fxybgthk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gdcjiupm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bbhhkbyh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xxepbana.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2azdjuyfi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2skfftmhi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gvxuwjxo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2jeigwefb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vjkccqrj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2sslgnzkk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xdnxzfsh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2udkjvgqt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gurbmdxv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pranxutj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2trnzquub.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2strjmtwy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2pvjgyepn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bipnfwmt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xlzwmzrp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2szoilhau.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2uxipwctm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vkuhqtuf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yiaggmzg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2dylsvwlp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mjeqqngf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2bfjmjnxv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2qambzmof.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewlgxusg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ifmukldc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2aabeltsw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2lcpilklh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ckogdptw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2sfizapgz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fpeossox.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ffrfmjov.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2qbijcexj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2efkgojbt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vxycmvjw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2vdqypdvk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgpuciha.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2saabtjij.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2juwocrjj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2fkozdfwg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2eyybpciu.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ihamhfau.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2smpluxof.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2mwxecimu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mcdkwzgq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2yglwmagv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2shohifie.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ditamznu.html


<!-- 参考信息 -->