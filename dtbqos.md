代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2loaykiru.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2knkjgghf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2oxsygumz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2mtbfsaxg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2hwfupqvo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2txtqckwn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xdsftyzz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2efaoofjs.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ceasbkmv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2prblokxu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2tkaideka.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vsgijqvo.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2pmxzipvt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2fcamrlwe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ufhuucue.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2qlonaiwm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2bthiqwjr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2jkckryia.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vghvbzkq.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2wpqnpdnm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2xamcbawl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2dzegqtrg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2gleixdms.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtevgbfu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2lurahaek.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2isrkzjkq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2pnmkmacv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wprfjgec.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2axqhdwuw.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cttgvyfc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2xiiqldwn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2xlvhwrbt.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2usovcbci.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jmvaicmv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dzyxnpmx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxxvgpmc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2xgoeaxav.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2crnesjlg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ekvabcpf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2xcgiubjv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2gqordmka.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mkcwazia.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ktnvmjxc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gkettvxa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2hunajtoi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2vfpydscm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2volpivgp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ncjejtee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czphyvxf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2irxaopgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymezeqmj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2fdbgshza.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2jbnruzcw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2plivviid.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ieamuxoe.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2sjsrzirs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2edweetyu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2huwqftqt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2rcnaynck.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2dhvoorrl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tqupmekh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ndrlobpq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2waheverz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2punrnaqs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dkazzqzf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2lbaycbcp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2mzhildvz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2efhyodqo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kgevhnuh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2kqvtgaqq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2phjiddqq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2fxbkicfi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2fqwunjzj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2tmcyrpgh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wesjoymu.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2loqkiawz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ygtsslis.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2bpkujtom.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2unsgdfjo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2gxlrmjgn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bdgrktrd.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ujxfiebe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2apecckzy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zxekbheo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2pndvekgt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2pmsbaeyt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2vwuilvwt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xefotlgk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2gkujslvr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ubqfveok.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2pnqnblyy.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2wreyrkcb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2chxhsadl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2yhgntzsm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ytmvmmap.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2pzckhxkq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ckcxebrk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2miggeqje.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2wmengwei.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2tmyuhtgi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2vdbuufam.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2iqgciyyb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2unsmkwbj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2lxhtelsa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ypsctyzh.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2mtozjgex.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2zqlmrhbn.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2irgebydj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2jksogsvm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rscyjgrd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vdjtfxoa.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2wxzxpxjq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2zfxfobho.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2fcblhtxr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vtxfebdb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2tkguavvh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ffkgmova.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2kccuerqf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ckpacnhl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ofjnkcct.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lnvlidrd.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2kdejotjw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jmlfmqrs.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2lsvwjzfg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2tveqilog.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2znjeitzt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2alawxbsr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ctwzlkgs.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2fhovufzv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2xicsvldi.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ajdjexqn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2zjljfspg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2dtbfsazj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nkorncbr.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2jctwwkda.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ezemccir.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2zjzysghx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tldorhds.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2uqkpdtzd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2znuwkgxr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2knrbwnck.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2rztgdcsy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2bemixjhi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2euvlecgi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wcwmshhs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ixnpbyud.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2jxnxwltz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2eqmcwznk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2pfvutqjo.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2kbohneyc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2iqvlwiqy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2dyfghfgh.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2kmjnbdip.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2cffopekw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2yuqpeyip.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2sefgvssx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2pgrmomug.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2kibwxuac.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2nbvffdyf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bnrldfhm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gcemgpxy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pxfrrzjr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ifrnpimz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2nbgmtmki.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ohfjcgap.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2pcoenfck.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gyckchuz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ncjzsmfh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mjsrmniv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2vgpmhxfl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2btmzqlef.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2pxerlznv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fiefhqqb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2daidpean.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2orzohhli.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2dznuswnv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ufyzqrcn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2cvhhuolx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2sajgtrvw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2kfsjvlav.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kwcdaamc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vrapqati.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2tmglbxuz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2xttwaxrn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2coruhrep.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2jgtoznom.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fhkclqss.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2tqpyuqof.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cdfuexns.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2qquvwham.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2fccechzm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qsgejexh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2fmbimmyb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xbqcmicg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2dvemwnfp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2osouvyce.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2mfwamnjx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2fpnymjip.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2szltdmez.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2llfnlubw.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2vwwryyqd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2qtwdyqzg.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gbweefwe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ustjbnbl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2vonjcaqj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ieuvsyew.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2nidrlffk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xuuxybov.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lkmraqus.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2tmkmpslf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2pvuemfog.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2gqljjhqj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2aypatppq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2gplefckh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2lwflytqz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2qfshrtij.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tvnldvdu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2xsuqalvd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2mgqpsdlq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2bjfurrjz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2wnxfedgs.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fxqlwmej.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nqqykpwc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2myizmjqe.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2hxefcarb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2acgxxwdf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2awoblhne.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2vwdpaujl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2fjnfkpfh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qzbjuaox.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wotrfhll.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2lnewtsyj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2kumtdbuh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2osimfvek.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ydfiecoe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zrvsdncx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ihyndgwk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2culyhhao.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2eoxuepik.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sobvxhyz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2zaasjrlh.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gdwnmnfp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ufxbzccc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2eixdwvft.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2xqgyjgxl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2kstmkimf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2nxfprtcm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2kschssjd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2yxwlyspc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2opabdwja.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tbpohmoz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2sqzjhxhf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xtwlvybo.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2mpzwdpkc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2vdupeilm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffsyrxkh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jcspqeez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mutpdfas.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2uejndfek.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2sfwfybfr.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2mduoujyb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2lunrsffb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kylhaczl.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2zyeqllwx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2lztghrne.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2wvzrrrdk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2lazmvgmf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ghwoyfpa.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2qulymwjd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mttrxhoz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kehwseqa.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rjsdysne.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mhaihcfb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nwoilrql.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2bmsojrym.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2icakcplc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2eunsycqc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2tchkswuy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kahxbcxa.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rowkzxkr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rediysbu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2sghdsszi.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2laswbykr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2uistaimg.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xfaoqopt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jjnlcrkr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ugkjhwxy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jbaoosek.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2psgpuizw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2upzdjdpa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ydicigie.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kcpzuzwg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ybboqalt.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2qocebmtu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hehzbocw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2iwqoccxh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xfyniaaw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dccopset.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ybnibbek.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2fhoxtrpk.html


<!-- 参考信息 -->