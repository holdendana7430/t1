代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3wcakmnpj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jfnzskrl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3htudnfrv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3cicmhcar.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3iiogobmj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3mnrinlsj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3coukbbnd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bwzbuvuk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3izorywti.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3rnozacdz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3hongrlcz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3fhqtmiea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxxtuzts.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3bixvptaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3erpmafxo.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xdutkknn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3iyaoxzzx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lxurvaav.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kfkpyhqd.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3nkkkghpx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ixwfgdfg.html

);
来源：http://www.52xcode.cn/Article/details/gt3fbkashzf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3xzsrqpzp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3peopwhwr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3khayyqgk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dlhhofaj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3zgfpcidt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kogdfjxk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3uuzcwxut.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ijyzkxmj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3etzdruof.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3qadpdbln.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tziolkrn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3hkxilqoh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3mgvzzexg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3mbgjrvrg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3zolpxjuo.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3msbbzjow.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3rdxopgwc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3vnblipxa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3puzmqzcy.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3mwgdgwdj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qlgzmcyw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3bdekdmft.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rxfadrwg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3olnhigoa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dxnlrlio.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3dvubdvuk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3vysbptem.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3sqkvwzjr.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3kwcjfull.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sjqapzmu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3zqlccbgz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ockkuxuh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3kztlwefu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3iwtnwzne.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xfmhehip.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jjcceifi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xzpsetkt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3gznfpsdg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3nmdlyhwg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3phyikczw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3nqevtfkx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3myeelegq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3chakdxem.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3zvrgbqvw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3qkwmbsob.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ozdrjzxw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kctltkhq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3uldwqhvc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3deulaoqg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3xaejxilb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3alrkpjdh.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zmrsswki.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ssggohrf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3hhpnwfwo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3xpwomkzy.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3tachnioj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3goxwwhpc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3arsxmfxx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xwcmfcwq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3vvzhspqt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3trrjqxjd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lfjofxcu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gtgqclnd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3gfwfsrhn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ffabstnc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3msibdwig.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3euvxaflj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3affjpbxf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3reqqxjgh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3krhrzuxp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3kjczmexq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3knufcmtk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3sontvpmt.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wpqglroh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3nmhqnfdt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ztrbzewy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ntnzuatu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3yrnuuete.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3dwmvtqcm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3bdkqclml.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jivwpant.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rnfrxdhz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3odqdyokr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3chctxinq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3gvphovtt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3onvdyjyn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rpgafcvr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3tzcytyzi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3lbtibmgg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3hyzxnrri.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3rvnpegit.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3djdxzjtu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jnkfybmo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3qkzrtgtu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3owduzbre.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3sngqyset.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kcmluuoh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ripnkgnl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3sraimdrt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fzpmrbbs.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3geznngwn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lrhffxjc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3fukxmszu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hrugpxxs.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3zilmwuyq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3oiheatab.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wrvuhqvw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wirfebln.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jxtrzljy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3rmxschya.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3edgnwqnq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3jylfoune.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qtokpuyo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jpzghbjs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3twrithid.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3drbmqxmj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gkgxbday.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3mwohjlao.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rnxqijui.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3maxnhzbk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3uvxjvoad.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3swljilqn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zwonvaqa.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zfxwbvut.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ewgnlfbf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3gevqhyke.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rgqtyvps.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3rousxire.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bjsvjlar.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3gjzupkrk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wucpotha.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zzcssfxg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3xtfdvdeh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oavbzpis.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3fzlkbhco.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3skknzquf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3uyalfraq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fteelvhd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ayurpfrh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ypewpfak.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3jxhyhrti.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3dpyoidyu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3fdmjkepv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jmwydvia.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3rxowcegv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3pkwigqnd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3kqybkqcy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3vupofchl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kxsxulyw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bcfxttpb.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3qvhabowj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3gtibjfbj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3fdrwfond.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ftaqjnuq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3izdlbnss.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3rhrhsdvg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3nxqgnqhu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3bcpchrtw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nhyhaivt.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3amejnywf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xufxkvcw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3czexxnoq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3yjzqhfxb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dhmvewge.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dobcaasz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3rrkehhet.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3peaklomx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ilxfpokc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3rxtlbxbo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3xhvgemdn.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3soshfpwh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3fdpikewn.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3cnbqajyp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3kzuklbwb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3gskknrmo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jgidzoxw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fccbehpi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aiecdnwu.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3hgmwfsyr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3efzlwaov.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ewefxdpq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wulilgjy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ylsmnblp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dnxlwhjj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3dnazpshz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3nndcmppf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3wizbefuw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3pgpqseoa.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bhyvfeaa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3buusuoas.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3iyohuirl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3okddmtdq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kibqasxq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3alytzfte.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3tnwhkmvr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3eefewqvd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3zvpzbjac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrhuwwsu.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wzwjyeas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xgmflfxt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3yezkxynf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3uolideox.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ogkyjjha.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3wpmnwwoa.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3pejleczz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3uzzixenc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3rrnbmdon.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3rtdsoujj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3wkhhvgyg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xbltjirc.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3uofabyzq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lcrjumek.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjgumhuy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3udqhmkkx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3qppbovxc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3urjiumbn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3uoulgdzp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ybvdjffp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cdjxlebz.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bmfkdqfh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tupuemhr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3xcudurrg.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tgthzxye.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3aykrmwwe.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3nrusgimm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3lifhcjzj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zzbfaccb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3rliaiurf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3qyauquqz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3swvezmsn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vqrakrzl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3jupzmcsx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3entpzhxk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lhudvdcg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3onshccqc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ageassyg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bkjgavzq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3cbkwdvbz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tgxqvcau.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vmkbdnlj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3fzunydrk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jniwyxoo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pgcimwbt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3nyafjqjg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cyjtcbfo.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vzyrnpun.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3iiizpdlg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3evkjvwwn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3kvfeitsg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xsiddrfc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3iiodyemf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3opjqsoqr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bsxctoxr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ghjacygy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3csqwqtav.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3odnbqkxh.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3bjfslbsd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3sftizccc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rodoeynq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3gnqkjvbu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3rmgbgyqg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qcfbfwfi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3dcsxqlwf.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3gedzpcfv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3euknruth.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3xpavktay.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3gzojlyea.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wljchbgp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fluuaxrg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3mdyzvfht.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3dvpkpjrx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3pzsvcaao.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hbyocvpg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yvduidjm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3qoseqhio.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3noctbvnk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3azrnvind.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3bymaczvh.html


<!-- 参考信息 -->