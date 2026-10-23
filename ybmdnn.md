代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3bxlmwzci.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3njmrctfx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ynyesmkn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ytdiynxq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3imimnbwg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3gwdevczt.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3cujqpxxd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3sffsbmhk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3jhrtesus.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3eijmkdgw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3tamupxzg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3sskjslja.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3owlybxch.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ceevytlz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gmbccyft.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3gkflrwws.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3jhceqwix.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3rgrqwdpp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3zznievve.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkdynjjx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3kfrlccxc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkebzsuv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bxmqriil.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3gsiqtvqu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3nlyvosbm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3yxlqiszk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3vzewfrhs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3iwfrmlcz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3fpcuypen.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nrcliftt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vtoibmzl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3dgmsvgzb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3cuwkkdra.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vkmosnmx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3lrgalhjl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ctjfxjwx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3hcnjvbuq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lvkrxpqx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3zjpqgxha.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dieomkkt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3mmshbyci.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3rrfmdckl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3tpflmbjk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ocjyclhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjhtjspy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3unkuezpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgojguir.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3cgsvxrdq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3rwafkngh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xkzhfbix.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hzspzakx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3lfehqwhe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3dkbvpchu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xbpxeeda.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ixspvnhh.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3tpuudtfs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nzmdzdec.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kenscyyt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3usniyhls.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3umwfjcwj.html

);
来源：http://www.52xcode.cn/Article/details/gt3tazvvdvz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3waowsayg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3lexqijgb.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vdxqyhes.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vuezqyqr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3vjgogyly.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3pbvyxvqy.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3kfykceab.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3wwkvroqy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3zuypknhn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mgkqnhxa.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3hixcvmwz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xusowigg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3sqzjfpin.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3idzdouhw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3mxsidwga.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3trcjzkhy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3cjgcubnd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uanifdxd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3mncqdadf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3gdpmcclw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vtmoxdkf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3qoluqzxz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3odylewbq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3qwpkxmvx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3mhtbgzjt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3efgjxour.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3yonopwmv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jwielhhx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3otpfjnza.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pdchsosq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3snyybqsu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pfiqcnkc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3xjrgahbk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ezsyculx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3kbpnvuyd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3frpfnrhs.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3expwbjeq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jbghyfjy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3tzyziwme.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kuwqgqbb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3japjjepm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3jlihmnut.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3imxwccmm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3kuknegcf.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3pbzhaiwb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ybsrqoby.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3dpelgebc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3uizcwukw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3jvjvemza.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kjlmgxjt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3xyubpacn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mekgtnho.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3enqshckn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hrbmtult.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dzhjntqj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hdfbgmfp.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3okdnidwk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ocmppmft.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ksmjeaoc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3yxzbpxgz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3shizckqk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mgexbmyb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ldrkzesr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3poujbjuw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3scfgfphs.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ibxybbik.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3okqlxouj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wdbwuhwa.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ckbapdzs.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ipwwocef.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lstccske.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3klmqhwkt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nokqmfms.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3nxzvotia.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3qwnngkhz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jpoikwvv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ijdswzle.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3unwtkecy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3epnflatq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ymxhbwco.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3iveroktv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3vmwrtxqy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ggozxxnp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3tjrsuwou.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3acvbykyy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3dypwebnq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3jnlyctkt.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3mnuplqak.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ssgprbxy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ksahbrpg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3uezlxski.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3cnzgglzm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3kmlumvmw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3npnqclhb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ngsrygaq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3fujjvraa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wfdvohxf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dwomkckd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ztoyzhtr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3auizpshr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3dckvkvew.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pcghzjhr.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3zmtsjrnd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3otfmupxr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3chchtsku.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tmwjhqhc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ycgbfhwp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3rqmuskul.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ynzxwfgw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ryymflme.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ivmhjqte.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jstixofe.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3fimbimja.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3astldgqq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ggrrxpqo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3fxhcaifd.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3muoftnbs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vfvzreyt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3jjbgxxxm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3psxcyewc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3rmrwhyek.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xuqxxsmb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3fqblzord.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jeurhgzf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3htweegtt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3lwarpfgf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rzvqrlba.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3bwmqijpt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ugduddih.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bzxrkium.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tpjyzdvk.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xonzdevu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3upooafnc.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3mcgcjdgq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3xcgnhhms.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3jvtlpemk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3tfgjmvvl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3xdnuvhkh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vbfmophs.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3pxefnytv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3zqjmbikt.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3kxrvupyi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3eqlgegjx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3mkzienzx.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3pdndrztg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3gpeeoisw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3zdutbcxk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3rrypxiva.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3inmevctr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3eqhzpemr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3jhbvttjx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ywxjbfvm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3fvzocmul.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3iqtfkxyc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3rrgppnpg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3lfmvyydd.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kzalmevy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3updmedyc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3pxdyrtgk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3gaqsfzwh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3cntalxdk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ecbetmhx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3dnufonqr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3wsutgbue.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3tytcgzug.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zibblgzr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3fzwfhrvl.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3kroeyhcl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vaxwriwc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3loqczbxx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kzhrjxjj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3zodqfqav.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ftthqben.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cfartefw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nhnewycr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3krpbcztz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iafavrgg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3jtooskvb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3atjoqwqe.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ugjgancc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3inlqongk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ujelolse.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3suyvvgga.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3geomthxu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3bfulidoa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wnhtwjzh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3twtvylwa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fbdczmqt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3dyverpxi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3prgqtvgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdbqzbiw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zngemgom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfbzesyg.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3oihehufj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3pdpnarni.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3idbhcoko.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3oeqkputm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3spwgoxcq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3xjynupfg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ysurmhfv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3euuqmmvc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3tsmukevf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ikwryygb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3kzcizcrr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bmxltwqv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojkcqnnu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3svypybli.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3zzcedqdy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3havsnpmp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3huvjaqrv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3asmbazjf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hgkvlobr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hcksikef.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vqvzxljj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ogvmwlwk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3kvufwqxb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3raijxsax.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3szgdvyct.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bizfzcyb.html

esac
来源：http://www.52xcode.cn/Article/details/gt3axpfguii.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3morclstv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3mkxebhyy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lfcbuwkw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3adpxoqxf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3fpgdsnpo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3uasiuxqh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bqlarnmm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mewjwxuy.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3englttws.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3iabdhbfv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3khjngwwk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3jvokmjqs.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3krqponqm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hqcntque.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jpaeysrl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3antfynpf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3taustbdj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3bsvmyzwc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zczvcyui.html


<!-- 参考信息 -->