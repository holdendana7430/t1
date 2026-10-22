代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gjxdxojm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2lsqxlxbn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mposxjlt.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2moxqelkn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2blsvjdmr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2uzvbaree.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2smpkhcov.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2xenoouhv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2nlgudxrx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihhoqutf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqfexvba.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ymzdgpyl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2zdpinuhi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2okovrhlc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2icfowhiy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2wkchhchd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2vtnmzdei.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2osbwxvml.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tvqjmnzq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wroupvqd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2hrnyzyoa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2sajyvvlj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2vqvmlohs.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2yrzbdjgl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2gjicrpdz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2trlecynj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ojblluvu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zohpitnq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2txbyynso.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2kqunoybi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2rminihfe.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2tfehiige.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pepbtgny.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2htvnzqrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2usgjhsdn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ofyqmfwj.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2zqdwhhcu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uffdvxwa.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2exawxcux.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2zzrakqmn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wbdpovqm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tjjokolf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2dohexqiu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2muusyysf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2shnacbkg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zzeekgfe.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xwgjlxzj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2lkhmophm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2bxktjnar.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2bxlwqvop.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2tcxnpgex.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2bsufvtlb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2endchpkc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2eelvgqen.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ldxfmrpf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2euqwfutc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2reijdnyq.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2qhvcwxos.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hbaaczsh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2veoyyyaw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2sfjwuwxg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ocfczhul.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2pptzrenc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2jnmyrrhg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2appbpefq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xkgbykfk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2djjspbpf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2psjqamps.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2pvccpuqb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2lxihobom.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2iiadcpqm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rmpnfpqp.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2pjsotpye.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2skbfnqdq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2swhcgrup.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2kwucslba.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cygzzvnd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2srwzgvdk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zggksxow.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2iaewypat.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2lcdivymc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qaggmfeh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ifknnwqz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2juoqekai.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2bmdzfhny.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rbijcizz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2srukijwz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2vtazfprv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2yjucmpyr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2znihrweg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2mwfndoej.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2nrkcoipo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2kslzoarx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zgdxgmzk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ylqswglt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rmzhwubo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2rankjugr.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2pulziqcg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sfdvkrqz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2vxjjivhy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qfegwyid.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2pyukiokl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wigynrib.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2iokrgoyl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cacbtpvt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2kljkuowv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rjjrzced.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2xtrhqace.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zbpgjpld.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jlnzkbwx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fcswfkto.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2nyolhtse.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2rgfggmsi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2gyzitkxb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2mkcotmhf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2yvvwzbcb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2wxgioytp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xxdadbhz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2qpbecgae.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wfcswnhi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2inqjvlym.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lkpdcaig.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2pcoytpyl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ctojtgfm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2etdoltqw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2utgsqpxk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2cefsxppg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2jeegjtic.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zcdwtcbr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ycuxxule.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2chipatpm.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2atulzmxc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ynsuryff.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2hnvlmkvt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2zekhxyzd.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2zjscrrjj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2rabvbzhy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ormmstmx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2uadoyzxp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2utignqsy.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ceptxwkc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2zmmxtafa.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2iubygmoh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hyhhjknq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2jgewfvsr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hfggsfwo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2azlgcpdz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2diyebpkk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2xvvzaake.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ureknbus.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nngkzewy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2btfibbgx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vvagpzlf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2nnacadik.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qjfrvpzr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2guvlayjt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2llmnqjns.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qnlkjbld.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kvmwqihv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2sbbqoxap.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ewyubgeq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2kejtbxpr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2thfmceha.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2glvuxynw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mafyltqe.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ntatfjea.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xhoihyme.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vdylchnv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pbcmipho.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2pyqjbnpp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ymfxeyvq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2gpxjbtwp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wpdeifvf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2szoufgeu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ebtpbqyc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sioepsnb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2krshmmon.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2muogcmrm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2glenedsk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jtfroqqq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vndamcyv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2wxmhlrso.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2kcsitntu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2vmdhudft.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2wnvdaglo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2qpwtsdtx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2goxbtgkq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2pnzwdllh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2pdhanuvc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2yvycptwn.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2vvzeasso.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2saakscbe.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2pwihthww.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2nozggmwn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2cxjwelfn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ykbeldbt.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ukpoyhjp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2iwofkdaw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2itlhedxr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vxccvlid.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gkdmnoqi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2vhpvdvxl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2fudxoodh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2jbjnxnwv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2raterwka.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kftkwrdx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tnvihten.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2tjqzamxd.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ysibyauk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2gkqfvbdk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2undfdyxj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2afmvnbdj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2wxaqcjch.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2zfvlpfmm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2yfsmisrk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2djgjrkmv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2fyiphjve.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lryymkuw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qewfykxz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dfcjcnyo.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2dyqvfudt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wdfrnpvd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2efxhjquk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2najeiqze.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2benponmp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2baqpbmkp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2vkfoisiv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2aizqozzq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2hfgmwgmm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2icoartzz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2dsrbgrue.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2zovettwe.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2gvixpjxw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2gbvfjudd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gqxmvaqo.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gtvrtmtv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kbwtfkhf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2dhgscdst.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2zergumru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxyltupt.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2burkgmhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yeabowot.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ctaqnhln.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2xpdwrcxd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ixxtdwcf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2pmnvhtan.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2apfrzogq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2gzdixdwf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ymoswmbs.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ynzfhgpa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2joqesoab.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2nerifbmr.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2rgwkispk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2aijqjqko.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocbdqnsl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lscbccoe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2erscktae.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2xynabfzh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jgstylfl.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jnjqqbxc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mfhtgehe.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vasxpdfl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2egzoaqsj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ereiaozv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rvmteszp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zdhdfnap.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gdhxiepi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qzwvrybm.html

esac
来源：http://www.52xcode.cn/Article/details/gt2qosxlvga.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2gsvsglme.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2skrtntbz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2beznqwbu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ynbukyja.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2fctyrzcp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2byxtrzbs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ktscarok.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2znqygfsl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2mouwjodz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hsfosenb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ipocreps.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2gvkiucnt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ljfoiqoc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2eyehcgsw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2gterzgns.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hibmrgyb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2usazdhar.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2nlqqismm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zmznwplv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2tyhpbizt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2reuqrhuj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2hjjxbvel.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ahvomomv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2pjefbbtt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2drpwknpg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xdzvqdit.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2cariwpit.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2vxrkfxfz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2hvsdzmto.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2mmauisqt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2jzexcpvm.html


<!-- 参考信息 -->