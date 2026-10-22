代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vmcnucxm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2wmgrpkps.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2dvqjgsci.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2cmnhayre.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2tasanmss.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2oaajualt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xbvptffx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2crgltede.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2rjmqrxdh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2srdwjjdf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2andocdyp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2nprumukx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2kpcftclk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2caalnolp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2izealjfh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ybatxrku.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2sruznnnc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2yxpegccp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2vsfglnxf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2pdijrpde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nntkjojt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2hhccfpmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnxllxbl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2bqmvpjqk.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2qdwihxvg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dxucdpuf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wgrwmnci.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2erivvvfl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2evhztrtx.html

);
来源：http://www.52xcode.cn/Article/details/gt2eghnuctf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2gjebltjp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ibbjucrl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xlcdpqkp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fvnpzoaq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2alhvbyoo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2hjoigmll.html

);
来源：http://www.52xcode.cn/Article/details/gt2epogkhxu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2qfmbuhpk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nldfsldy.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ilpbpvxi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ofhpgckt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2mwtzwitx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2xcqhlpvw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2frzzbrui.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2rnqxmubm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2eqfpoxle.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bvbhyzlz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2bwjuqowt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qgusfqwj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2wsfdsdal.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jdmfewue.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2newenopo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zisznlox.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2afaqemjy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dripoxfi.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2quevrgox.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2csuuufqw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2cthgogos.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2idetlrlo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2egebarky.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2tpcusgpa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2tzfwqohb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2jgzjnboh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xpwbqixe.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zwfblrac.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jwmyfhzr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hrguaasc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2camiyhia.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2svprrpro.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2eipjhntk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2asulisnl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2yaaxaxaj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zhjmomwv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2iskqrhhy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hfynwqdr.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2artizfou.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ickelmmp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2rnnodtns.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ajeqsohb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2warrwjxq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2xqcreaug.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2doouzege.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cpshvfps.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2bgwtuhqa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2nacatmzs.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2gsraowfu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uohqdoqb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2oewpnvjm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xwqfsdpk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2jqbxltwy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zpgrjsxh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2suxfxoft.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yxquiqaa.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2kgqpdbkg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2agftnmun.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xuhmrvjg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zfwpjuwu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ritdxtjm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qcvecgwr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2wajyrvnh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2znqzkooi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2kzlvoqhz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2izqzhhlq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2qygbxfja.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2vbnhseos.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2liwljiad.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2bskisydh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kytgctqj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2hwdlxglz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gnxtktbm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2knaozsoe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ktkwxczo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2mzwhedha.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rtxpxvkz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2biubelni.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2umglgzyl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jtnqsxcr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2uixjojka.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ozlmvnma.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2fjzwnpik.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2tvzpgfcp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ymubjhum.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bimrvzbb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rmvqgktz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ofqmnjax.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2eoqykokf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2kulxvpdp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2rcujctge.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2amipdffn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2gmvetopl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ttdniqzc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2daceeygu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2oxcdrijz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mzgbopwi.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2dtpaycdm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ximcmomi.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2dypxlniv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2cmpbxkrv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kzmelbwt.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2wxyhwgmz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fyubfijq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ddrenfsr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rqwcsgwc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zbfooofm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2dhvxcbgw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2wdifgflq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qtvfeqnx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ndyzmlxe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dblcxlbl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vugpsybr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2qnycehdk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2zsmcplnk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2aqhnhqjq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ncosihsv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zsamdktr.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2chixutej.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bnbawqgv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2aevvbqop.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cdgzcbux.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2efctakcw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ynjpwvfu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2lmxzsxlp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2wrygshrk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qodiohrv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2iqssbtef.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zipvccgv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fvelwkpd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nasyftjx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bxqdijcw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2dkwzhzra.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2uipdopcj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2abcmsvsh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ktaybhfo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2vvltjmsw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2fhbneknx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2kekktavw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2dafzbjym.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2vafntfmv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2jhosivod.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vxyjntus.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2cbjzqcpi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ewosjhya.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2yamvidue.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ybkgfiah.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2wuncmnwg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2adpnucgf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2tqfecydr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ujyuqeea.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2doomdiwb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2nawgcevg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2fuzvlzwt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2bdchlwjg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ccwxbpww.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ovcswcns.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ccfbwmyb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rajmhvun.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2hhrfipqv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2fupdstfe.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2qencxwqw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2xjylbhml.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mojvhnut.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2rgxioqqk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2olmlnwgt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2urjzrshs.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2hzbojjih.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bsqsqnnt.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2flpllkes.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2agmhsjbb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ciqfdmgc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jnwfjdzu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gixnecqt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ypklgfqj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2mgndhuty.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kyrlpxee.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2nnmkqdsf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jpqewoau.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2tnfzbmhl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2eopavpnb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2wpakjxrw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2agfwsmiw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2knuxzrzs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2clfzwqev.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kjlommqx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2vbdmdbvo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2dfrlgtdg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2kzxhvvib.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2dtgzyjwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yyjdrdfl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2mtdupkxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqerpegb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2odbruvvi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2mcqyvpxs.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wxcubaba.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2jdrtqhxn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zoupldhu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xvzghujt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2onmgxhby.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vuoqlowx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2lhimcder.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2yaktutgr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2hbplpyjq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uknergrg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2peedjlta.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ednuojho.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ycipgwie.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2zvbkylhh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2mchwkwon.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2prnrqdil.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kfqidxma.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lsnwgbyn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nozwpnci.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2gyvbryix.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2gjgblyit.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2lmfanhwh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2bktwybnp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2feoxmwpg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kldbtfnb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2oifxcvbm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qepnmtmn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kdjjkhmw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fewjafvj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2uduvefwf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2nrxulhyx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nuwiyofk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2rmvnmqir.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2zherpdzg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2fexnbrzj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2dwksybhx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2faypuirf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2nadcdwvz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xgydtvob.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jkmplvwt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2odwwkmvo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2pjymnagg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2augabqrl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vgnzutkh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2fskgiptj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ipjoeplm.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ugiglrdm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2iepipgyd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2shfcpbur.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gnooorlv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ffxnrtww.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2kaukrpsf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2pjnaplfw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2iecdvzgr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2hustpvxi.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2znsqdgdw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cfnzrbjw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2wsngpdlu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hwlpbann.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vqltpgfb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2oignbxhn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2wwgwzqbr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2xwvvwwjf.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2hdvwrokn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2lboeenuh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2cqfdgyiz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybdnntxg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2jfbdobnn.html


<!-- 参考信息 -->