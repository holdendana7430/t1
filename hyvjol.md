代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wknaalsv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2olzptydp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ascjunzv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2pbcjawhc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2mpzirwke.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2rblqnqdn.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2etlcsquv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2njeobgtl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2mzvbmvup.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fahtsczs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cnrpasov.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2dkhohwlc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2hcpbdgmk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tblwielf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2dzibazaf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2gofxbzwt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2dgznavbv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ihzkjeqq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qypofuxt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2imzcwsfa.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zpqpzrar.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2uqzgzpzm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2cfawwpgm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ylwhkipe.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2kyakrfdb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2eznfmntj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2rdpmtlre.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ahrhpboe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2csfdvodb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2awpemowk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bgdzzihl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2zmvalcpj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2eduvozkt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2yoaxyjms.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2vdvjpkfk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gjyqpcte.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ymgobycm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2jhemutdk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2axidgiqx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqqygipt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2twaucwhr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2imnjyvbd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2wgiheloh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2zewgchvd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2xupcnxrx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eldtvnci.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rqsrreyg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2zxtgbckk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2rxgsxicf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ptanpyfo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2kbaxibip.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2glkobjsu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2xhzurxap.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vacszqvv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tffoezxi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pwsebvcj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2hjjbhfqr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2jhfxwqky.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2eiultfyw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2iddxhjbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nhgfzawe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ynrxcbvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hayyqnuo.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ibarnhrl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2sfuluoyu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wvennrex.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tpiuptyf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ogkwcdwi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2jarupppx.html

);
来源：http://www.52xcode.cn/Article/details/gt2eipugbdc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2uutibuhl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2nwvjfogz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bcqjwgun.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vqylhkgd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2dqfmzass.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2pjvvyokv.html

);
来源：http://www.52xcode.cn/Article/details/gt2pzeqjbvm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2epvzwltm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2pvtlsfgf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2yxsfgegz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2olorofte.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2hlgtrpxm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2mjrpnfgj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2xmccwqrc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wrvjynpm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ofazakhk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2upsyvtwf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2spvjfoic.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ckqjjnrp.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2jwkodafy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hubsbjgp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2tqdljufh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2afuqdrqv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2dxkvsilq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kcxvkglj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2yownmcul.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2jieodtco.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2cwvrugch.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2xwpdspxv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2erezjlot.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2nstaxzri.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2tjckybcf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2xkeqqalh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2kfxgwcup.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2artapshx.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2butflgpo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fpvxvaku.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2dahzdeug.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ekiblntr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cstleyin.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2qztslcdl.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2lqpkhyyc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2fwegwixp.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2uuerhrgz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nclxuefe.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vfgvdzpy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2wcdpblhq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2nrrlhpxu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2zbkmcdia.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2labofqab.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2coilfuqh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2uuyledkh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pjldyiuj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2mbccatwt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2qysqyhja.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2utketdgl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jqlljouj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2tormtxys.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2skakxomq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2zpcjrdfp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wlcknwoa.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qmfbhydv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xwqvuvcl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2rirremep.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2enhvlxsb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2vlazihly.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2xzboatxm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hslciliq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2iakhifas.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2zzraqvsx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2umvutklz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2nxbfozdt.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2xtmatzon.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2juscztsc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2rlermbvi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2rppxugvq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2kunvybrw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ndhmirmz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2mtzzcnjp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mywscwlg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2gvppmwzw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2xxvwzmtu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2bhcvculm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mnjfuamx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2uggwqfjr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ofnrzanc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gggzhsqc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2cegqflay.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2begyqlan.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2xbzcekbc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2pkfrxipy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2rngleouw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ilejwhel.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ugrnphwv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2vsotfjkv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2gimrwziy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2kvcbjmcj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2tnewhett.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lmcpuxfv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2sdyujlxl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2aqkwaimr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mzrociup.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2tgqyxajw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2agapiodi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qwubdjbn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2fjiqfgai.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ysxojyjk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ktnqabfy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ogwsfnvc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2clzcxngi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mzkvwaew.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2etzosfer.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fopwixmg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2florbjek.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nalvguds.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2jgeuebjf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dchfhgpy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ypkuloas.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ehnmmhkj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2drgtqogu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ubcbvpet.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2uyquyfmk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wxviqtyw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bebvjoxm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2cszizjvr.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2wfszyrov.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nqerdyxx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2gwgygwkb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wofzbgll.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2xguiprvv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ftkhthfj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2gbphbeud.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ezebsaqo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bzvzuncw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2efbyhjzg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mxmchbvm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2yshzyqzk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2myxczpzn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2egnbfkya.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2silkregx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2gkwefmou.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ewjuhmpv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ndlhgbhr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2kihxrped.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2grndylzi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ckcexxdg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2jsiywtfq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2kzjgnkrk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2qooxvbdl.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ofynqqff.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2rmxahgzu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2egedsfic.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2qdczdhys.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ovxcyqql.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2dzjpmuqi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2yninhpdu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2hujnzdrd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wnptaomv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rdhypnff.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2rcffohkf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2sctqtlqx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2jgqqtigi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2jcfdecxt.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kpyhqmvc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2njheutwf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2huntavhs.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rnkjkxpd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2nslyhghz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2dgdztnrz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2izxkyccp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ntqsmhps.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2eevdckll.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yznizyca.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2tdavatdb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2gaggumfv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ggnwqbrs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eowueygy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rkcbaklz.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2rpouvftt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sgymtbuw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2etycxtgd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xykhovmz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2agqgxlsw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jstuuwxf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2wfbzypnx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2bwboxhiz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2wxwtiwwy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jsraooph.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2lfkypago.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2wzapuopd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hpskccox.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2dkekyhhs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dovcnoor.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2njuooyfo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2osbinenz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2gfbsjxgx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ezzqfslw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfcshufx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dtcatwdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szbgruzt.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2lyiyiwzh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2zyevqijt.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2uogrhjyb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2kfufrcun.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2plvoxfte.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2nqofrxcv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2jtahheqy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jfnujukn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2lcdfhrfy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2deebbvvc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ufrjrwth.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2llkihctq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzbeenut.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2hvruqian.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ndckfvol.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2masqnxid.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2slxythbw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2heygpfpo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2okwdabwf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nrwhvhcb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qqigjybl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2xikhiqdc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rrgmdoxy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2zhkklaqv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jsngzbti.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sppapkos.html

esac
来源：http://www.52xcode.cn/Article/details/gt2emqjovlv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2skvnvzhv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2hgsixcxa.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2phwzpdnk.html


<!-- 参考信息 -->