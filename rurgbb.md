代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3lylmryfk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bhdnuwbm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bslujanv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ddrqxjis.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3blvflyxg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dqfhisfy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3tepsrelw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3vosclaqs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3zdpoxtcq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bfaoethh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zazqievx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3acblvnms.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wluqhsij.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3hqhqxhne.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3hoikeqlx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3achpvqun.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ltcdfehs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3tjelttwj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3iqlnyvjn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3owzqdtgf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hzdgzqme.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3tdvqlepv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hrhsztpk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ejebqqeu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3pnxsyzdg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3wgojuhtk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3vowtpivy.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lizrxkze.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3effakzdw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3voiymsvn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3stiefkdq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3sztbzjxd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vjhwjdmt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3klkncscr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3dbethffw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ajahqlxy.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ejtgkmsl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kmqnnzox.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jywxzgot.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3nuqgaelx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3zdtcjpln.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ukoztlbq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3bttplglt.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3halkgzlf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3yclsujgt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3iadfljom.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3owuuwmgw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3eolgcavx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3zsewvdsh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3bumbuent.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3svnyowda.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3mcvfgihh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihorglvo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3zjofjcim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjxlrchm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3legfllqb.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3xdaqqspp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3folxirtm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vwpnofud.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ezbgvzpx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3jgjfdjmg.html

);
来源：http://www.52xcode.cn/Article/details/gt3ccppqtld.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3tdeicliy.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3merugxsk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3atqdwbrc.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3yqyartsw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3uvjkycew.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3iyflynuj.html

);
来源：http://www.52xcode.cn/Article/details/gt3gnpljuep.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3sfuidouk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3iivocemd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3dbmjtzwi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3vdtrqruo.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3lbosodpw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rkubzjgk.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3nlhlihzl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qaxfwbvk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3uqcecsxl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3xyqagupm.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3afwspuwc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3hckdlxtg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3btlwfkdo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3vyhpksxw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3kbalrzbl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nfuajwcj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3bqmsumos.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xrlffrfb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3wxonemrp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3nbciaddt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3gvemfbis.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3uypnchxv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gupoipon.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3vtdevbjj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3pcohdrcp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3obmojopr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3yhwxxlne.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hvayojgy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3liufkluf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fqdpzamc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3urjtlfhn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3izfghrqh.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lgdagevf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3xbgrktmz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3udmaysma.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ragvgctw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3itnmpbyt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3vdcsbwkp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3bzgeoxuc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gzmjwbsv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3prmtyrex.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3wcwrmies.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3xqvjlaff.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3cevtlqsn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3fbsgzsik.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pchsgcpx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ajrcyqyz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3bilocplv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3euwqxoje.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bafhckgs.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3rwgdtkzg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3alreudnp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3bvvutjma.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3itplfajx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pieeunad.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dfrkdrtx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3zxhqxyom.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3pssyzeik.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3vkovtdza.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vuwirgdg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3javaewhd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rxgvabpp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3nhsklssx.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3wxhvsmwx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3biteglnp.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3onflxzys.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3sklqrods.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3znbunqpm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xwckpcww.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3dpsnmnew.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kvzwrjdl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3pzqogvlw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fzvmhzpg.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ekbterra.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3pexwahwq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3bbonlwdb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3iejdrtpu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3jcbnumpy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ppiexflw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3onrowkdn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3eimxdwhq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3yinijeyu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3mjimuxwd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3dwxmvtoh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3usvwqepz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3rauwutxr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bgbafukk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3jxpwbpta.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3smwqczrc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ldziysmb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3aflrfviu.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3oqhppeba.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3qccbxcmn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ntjmkmre.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3sdxmtrzm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3etjdmofz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3oyrtjyeb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3czmkfhbi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3pefbjoza.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xokisxez.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3gblagczl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3cjtrajkr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3uyylabkv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3oljnnuql.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3bolcxpnz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mkrxngcv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3onguwcvd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3skahnqqx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3dyjiroci.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lifinbet.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3qcsajcyu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3tqghrfst.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3vbngdieg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3evfvtjir.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3vdlrjift.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3pjesfrkf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zhsexnxw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wjsqhvrx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3crufjxob.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iukwrnsk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3oiugzzii.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zhywuoku.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3mvlgeyfx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uzspzwdd.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3jkrijcfe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3sdyduecr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ypkkgmgq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3eohlucth.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tbrvsdhu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3tihmpwez.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ntignphf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3fidlpqmg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3hhhzkzvs.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ppnlzuue.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3epfgwkbl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3zwwplnhd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ewvwauhf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3tjtgjrcy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3sluhdycn.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3dkkjswtj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3olhikrgy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3fndbhysx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ozegypyj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3yoheltto.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3wkcmcayb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3bqzdfjfu.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3lbtkifat.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wwaxeafn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3eayvfqdy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3iaeickuo.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ksrbzcyu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mzipmmgx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3jpdtlxzj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3euumkuyq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3gbntqpus.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jjpxxtue.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yviuxarv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kmmiieih.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3osakvzhm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3sriqcomf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3hinawqvd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3qsozapsh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ptboqald.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wjkfmgyn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3hzqswurz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lnbspwlq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3rsirtfep.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3jafhrjxd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gqdqohow.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cuufngrp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jbcjgmav.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3akijjaeg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ieybhkaq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wfnlamvy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bqtnbxtg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3jgjolcnq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dtlgmdnf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3lalgonvb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3czbvplgx.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3btkzoozq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3wffvprhg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ypvdwprc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3dvtebeeu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3fsutybkg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3hwtnfzvd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dwkvufqe.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3mcldizkc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dbatwiso.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3bssnbrrz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3lpikdhrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ghhcfpbo.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3uksyrqjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wogllpbx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3laqbhorh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3kjfxdeby.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3sjygvtfl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3jsjdteho.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qdgwqygj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3aivdnlhn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3afbxwtpi.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3aiglhvgm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3kmlfobrp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wqtajlih.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3txhmrcnt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3hfirqmvu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvcenafq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3sadruzja.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3arvcfuwb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3kliubnha.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3krmlfwxr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nuuskzdl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sdjreizg.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3iuubgshw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lpqxjcls.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3pzhhilbo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3vumqgbiz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3urjwxhxy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pkogxhuo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3toycvugp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3cykvfhpz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ssfqrvti.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yyhoylva.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cbpaoict.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wdtliqpy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3guswcipr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3istckiod.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dfyehlya.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mwreqyfr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3zaniquxs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3teddypuv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xfuersaj.html


<!-- 参考信息 -->