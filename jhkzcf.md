代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2lgupkkui.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ijtwrwtj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jbamzmdw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2yidylobm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2rgwyfncs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kercozri.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2nevhnwxe.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2cltknulu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2mhowqicu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qinoybxc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ylufnrin.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ivceelry.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2bsssxrfg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2neobxfay.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2muexyhay.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2yppatuuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjfgnpbd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2pvljvbjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kfhxrdxs.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2jtvdkcri.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2njsdcgwj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2heteoubk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2yovigyta.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2dlnjgbkh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2hdstkqha.html

);
来源：http://www.52xcode.cn/Article/details/gt2jtfpfjcn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2oterblei.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2girfpqmc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kyiyvlsl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wazflltq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2bxzlhwgv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ipxxocil.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mqqmejki.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2kdnlqujy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wymkacxh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2xosiwbzm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2wtamocgf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2hkvhadpe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2vvkrcdrp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2jfsvwuuv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2vcncjhaj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2heoufokg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mwiaehhn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2vscjrypi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ktyzuiix.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2hrajkvvo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2tpmahkoy.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zwegimks.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jyenwjjf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2uosixwyf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wxjelpiz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2tlmtjich.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2fhkrmalq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2buwvzdzt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mfnvjqsa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dwmxmzdf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2xrkrdbyo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2bcufogpx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2dxletxqs.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2kpywjjba.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nhgwrvll.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2nblxzsft.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gzyzqydo.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xnwflpky.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2azgqvgec.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2icjdiexh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2khlvlxcw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2nakgjvrn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2rpvwrghe.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2aogbijgu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hxupcxse.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2oipyplvg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gayfykxl.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2mpmyecqm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2zrsxztes.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2kwdevxwk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2bygovcae.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pvatkkql.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ikitzawt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2hxpfherw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2swvdzkdg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2azlpmxzr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tuzslecf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2krectdsf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kkprlbei.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2yotmaaer.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2slggufkg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rqywgzko.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2svzdofwo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2fypdaelc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pmnpghmn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2uxtvzvwu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qthcjnsc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ikfvaqem.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nhtnkwib.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2jnyezxnm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2rqbnehew.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2eegjqhjb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2npbfnmzy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2gyabgsbx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2fctolgfd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2aewyrvah.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2trlxpvvs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fycxfrtq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2inqwsagw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kgknzimp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ojmvdcyi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zaftfaoo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2yrsrqblh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ktmyrfqs.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2wkgwaeqk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2iykkwcmd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gimclgtt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2awqrzlcr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2uyflxrki.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2kevapnao.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2zhyrcyir.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2imwemhpu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2uhycciib.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2isckqimd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2kdntloqr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2gylweqpm.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gzlfhxac.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2dyyojivq.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2lcdxfjmp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2acaapxni.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2dqgzvoeb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2rmrbkmcr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gzjrahnc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nfqkjyua.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ipkwcmcc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2umqfnnis.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2miasdxhp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2zgtbnfik.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2frwmckok.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2braleqdp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zdspsbho.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2zejijlea.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2uhrtuvwl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xfjhmvdp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2vbbksjwr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ugmymklo.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fwcyoctd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2dznpmipx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pysdqbtp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zaggfanz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2tysndcyh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2rrpoolit.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2syzkrxto.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rgwotooe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xfojohzo.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qqrcgigb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wmmxpggr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zejvqfnf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2emwssubf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2qhfiqziy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nngsyygr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2rfxzjoom.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ztjnunni.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ruluxmxg.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xddippyq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qltiwkiu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2sxeeiqjg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fnnjanay.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ojwqslna.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2kwqvbrhh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2srtowwrj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2gogtumeu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2dnykyezo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2npluebuv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ccusxqpg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2wvmpzuzw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2uynmvxwa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2fzgumtfr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2kkvpxodn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ixtohcps.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mkabjova.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2htooslbd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2hutyxxay.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2qkkvaggw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2njkqhfeh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2zpgoacvh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2wwadknuv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2tkgjtrqy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bzrzsjin.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2nifjgzaq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2phydqsmo.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2jddegnfw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2oitbwvin.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ppdljkzx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uujwvnyh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wpeysrpi.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ycvagnbt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2sbzrvrxy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2yzgodeen.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2lnnfasxc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jhaddaqk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qkgbhrwr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cfgsqfqm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2uwrrcdkp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2zdbshpym.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2razwcnik.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2btcycmrd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2boartsbz.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2knqlnhns.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uzehxyjn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qertszjf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cmlhtauh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2wicvpjup.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ukxpherg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2myhdngdz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ilhjnchn.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2npgoufbc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2iykvplgp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2yjbkeynj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2endwbmpj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2bmqudyoo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2dxnrrdim.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dawuhvjq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2yrsqmgdj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2eawaeaip.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2yyzjkdqo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2dnvqisat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2witvupfr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jyldtqgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jgkpjsrd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2nnkheicu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2lcnuwseq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2gbqxlaou.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2cbbsskgd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2mocuikhx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2hqdzepbk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2sphgzbhq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jptlglot.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2gjzpihut.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2iypyemvl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2eczqbznc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ynfkmzby.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wlfspzyg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2praqehpg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2qphstdkq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bbhyvvkm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2mbiwswgh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kkflbhzv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2hxnijupy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2aiwxysya.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sofcmuxg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2vqjddiuk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2auqkijnh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2vbxxsuha.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2akrqazfg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2hwoxpouh.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xxogonro.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ufqsfako.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aoqvryxa.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2myezezjo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ukqesjkc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2eirtpbev.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iwkyjoou.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qusqiifd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2enysagvd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2vpevtpwy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rdlckkch.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2iqqziaos.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zbnhdbkm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2sbrjnrrx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ofjozdwr.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kudxmpoz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mkibmxlr.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2mwjlsrkh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2wnvcrnrm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yzdxeshq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2swhmreen.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2skgdwnkk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2paqjnhrx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2bmmenohx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2kmfquick.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rgvquovn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2sjliyvnz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ksvkgyqg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2jlneaedx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xaagcabt.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2zclshkrb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2lgwktbfa.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2lixalovo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2iqxfkxcr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2otvoiupo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2oydcokiy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2npbtowpw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xwockllk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2qsetxskb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ienukgjo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oshzzday.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2xkmmtvvl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fliyytxb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2cdoinxrv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2vpofwrzn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2qxgwxujg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2pbzsewtn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2cbtpnyda.html


<!-- 参考信息 -->