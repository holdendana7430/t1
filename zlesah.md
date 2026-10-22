代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2uhogrkpa.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2otrqnjxd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2qugaltjl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2vtilfebx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2yejnueop.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ymvwrvkf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pfqryell.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrlrazee.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2qfhhssnn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2dejgccse.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2bdudfaet.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2psdpawxh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2zhmooqnn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2niisvdcd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2zyscmnio.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzlyjiyy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2qhgmstdi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2mwirznnf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2lycczuys.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ectwkjjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsgjoryr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2uabjcgtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aboixxit.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2qzcnmlcy.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2bvurrlcq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nwcbecnm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nmucbwey.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2bgknokgv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2gcqqxlsq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dogbwjzm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2trhjyqgg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2khvollbs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lnmbnmtd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dfhfthug.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2iphyedfh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2scfjnwaw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xvzynfcv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2dujfhuwj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dqxpzzri.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ofrajhca.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2zscmjedl.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2augordyf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2yfsksdli.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2dtmprpwy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2oboplymy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2qongltri.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2gsgsahsq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2hbktajcu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wbgztsyk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2prncbxys.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rzsicrlw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2yjbcahmc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cldbesic.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2bliholxs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nliigxkb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2iduigdvj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2rduwchgd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2paltmiag.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2sbzwyvhl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tpfyobbd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2nzsdpeai.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ebntwvrb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2snhjpahz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2quvkjzpa.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2doypaepi.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2eqpxfsro.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vausaitl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qywtzajp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nqfintzr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2fqoyfely.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2hshgdybr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2owatghhl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2alrojnci.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2qwujzqht.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ecgoztwd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2xrwxbimk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2thkpzlzs.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2mmazkefj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2omvksawd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2mjjxgskl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2igjuvmat.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rjcbgamg.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ncpefofm.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zdwascdr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ktromhjq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2aukfnvmg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2btzxteqs.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2itlycnpf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bzvjqsij.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2uztoagrs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hngeywqt.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2howuabus.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tklgyrkv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2oovveycq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2miuveljh.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bflfbfyx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jikaaeqx.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2emvxlepe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hnldtmhi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2skraphmd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2zdcpuuxp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2wptgnide.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2rixaxqhy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2fegtjttr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2mngmvhai.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2vgleexlp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2vucncxri.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2frskjfsc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2lcsfpulp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oqwiaezp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qvxojtlp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2pihtipps.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2cetqjzwp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2rzplfpmh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2nmhzszsv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vwdmxyjf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uhmgfdjr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2jbazeiyo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2weboljhe.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2tmpsakfw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2rfatnbjt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2mdedvdpv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2mfwtldhr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nbnuldys.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2rnpefmfm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2mtgppgwi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rppovxts.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2dqjsntpw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2nzewmmhg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2fdntgauu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2hzlubysr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mfitkhyk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2jycixyqg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hzghbxhf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hxcwvcok.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ohhuoeic.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uqzuwkvs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2mhxiwjac.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bhuedjhh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2fuonvptp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tbxrjhtg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2sfwqapth.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zhkjcntb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2mvdqmzst.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ftkkxygp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2fkqwrrjm.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2yqoqyprs.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2hznrlgyj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2uaxiutxr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2dnfczwzv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2lmwksezc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2buabwmdu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jamxmoxz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zqrbkvvx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hnmnhzmh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2konszrbo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oesfbomr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2hwerwulf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sdezxcsk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2qhkxxitf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2drrdkyju.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2mavqmskn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ldxavnnt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2palkhjck.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2btlfrcrc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ofeoqffc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2eyxtqqom.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dphdwbjh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2dfadgzgc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2gjvxnbma.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2gkonnnsg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2cegxcidv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2iyrxytus.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2okvcgakf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2giyzxswm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2xkipzpzt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2lptxeuxt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2wawjjgft.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2nvohghei.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vkvibcxk.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2qjpoflgj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2lgpwzlhe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2qntksxrv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2lzosbxmj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2kzijzhsd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2xgckyxgg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ogbifvkd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2cxypmrmd.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2utjdxzeg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2xvcodenk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uyxuudzs.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2cnzqxeze.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2gzrfuyrr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cttvkrfx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kyqybnkb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ziepphhb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ofiefllc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2vwtpxtqf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2bgdmjiyn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ncbhjsvg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2zjywibvw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2kxqsieue.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2oxwlumgy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2wjffuayu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2aqddxcrj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bzoaxylr.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zokrhihj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cywclwuw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2soqgfdbl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vokkqqer.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2oftqptug.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kwyppnoe.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2uxzzfjgm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sdatyptl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2lrnfmrvv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2uvfbxjxc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rvybrrvw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2afmovziy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2zyttgcfo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2dldxwodd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ykwhuume.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2mlxpsqvl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ioetbpox.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2cfxqszoh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rjykfeik.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ozsrizmy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2qtybtnos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqiknlcs.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2tpbmtopk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wlpkghhy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2qzliygwv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2dyjrklwe.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2trttsmsj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2xqfriovc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2falzxxah.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2gplfcygf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zpgofdix.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2yysrwloa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2tonzqahd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2dfumogvf.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2iczbylrm.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ypljcjub.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ijrlipyh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2eowxjdol.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sqzclkee.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2nilidbqr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ocicncah.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2liuljzgh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2yfdtubhw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2nyunuqts.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2swnhuazi.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2inwqxpuv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2skwmpjiw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dgoyjivd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dxiarpwp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2blwfvney.html

esac
来源：http://www.52xcode.cn/Article/details/gt2wltxqmdr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2yzdsdaxs.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2rcbytmpk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pjhsedou.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wrkjjzwt.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2shepvpat.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2seythhqg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nuvqcaww.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2hfwfldhu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2durwkngq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2yanbbycx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2oguvmppq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2doqyqvtv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2iudnbavk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2zpazsmhn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hranjwtc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xqstqzoc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2svgoojnx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2rcjwvvxw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qtrsmtzo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2mwqibruq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zxieowdd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2lfapuaiz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gszyweag.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2jfmdoclu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pddrxkow.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2uololtzm.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2laazaaml.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2nulzirna.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ftxqeegb.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2vuyrbonc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2kewpogez.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xooklafe.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2yrpmlgiv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2phwvzpwq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gxdkgfxi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2nhouhpeg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eadhgkhk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2htuaziox.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2csxopwba.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2aolmqqbw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2knhroasz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2arhgzimk.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ykisvqjh.html


<!-- 参考信息 -->