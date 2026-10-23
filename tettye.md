代发 wailian999

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3nsygqwtk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3dowubkcd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3rjsmgjrm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sxumktbx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qfrpbhpo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3hwgxrkag.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3gukexnlj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3fgzisvvz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3dxuwtxyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjuwpnzf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3qhiwuqpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flyldqfc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mjnibwee.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3raqhhufe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3mdehwpxf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pwmjtttp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dnhiiwsi.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dsphimpc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ixgrgiwe.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pkefankb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3lzskgdvy.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3rzthmpeh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3gxlazepn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3czusufci.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3smpeuaoq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3arkoniko.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wixzakcf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qxursvrn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yyhjjxlv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3qslqgdlr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ueyirwut.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3tuebikjs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3voedajxm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mrrscmjr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fifilack.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3dmhzwati.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3njtgndus.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ftvewest.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3tgfscftm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ofbnqhne.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ojdlcoea.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iwxjbzks.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hoclnfqi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3reqqkpdc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vlenkmdf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ydglqqhk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3nmjvcbrq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bbtsrzqk.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3unqixjst.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3zcfitief.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3izbxxhrw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3iaurycse.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3iytjlqwu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3heibswjf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3btpxbtpx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3mbchguyt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3pbfgucoc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3zxhtzprz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3qnipopuy.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dpxhomst.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3pmwebrvl.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3pyixkhml.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cezvqfns.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmcluhfb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3dfpafsng.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nglxcofj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3pmhsrpfa.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3wjfvskjg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3snaytlcn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fadvjans.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3amcidabo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3wdcphmwk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3idektdkw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jojizuor.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3iawbfjlg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3uvbadwoa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ncvxtdmg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ricqnjsn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3iqpjydzg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yjewmeod.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ysroyuzk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3rzyvwarj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3rigcbgyr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3nxpiaytl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izelufyg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3qoyemdkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ciwieheq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3wmlamyip.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3kxvvhooy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3szwkxygj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lyvgzijj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3rdbvubif.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3clwzcxxp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vwawkzga.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3amrgdioc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3svcleqqy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jfhultwb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zufjsfvd.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3dibtoejx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3pfkxespc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3twlalswy.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3cdbhtksh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3axuczvxp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ivpflzle.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kjhpwmhn.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3lugowtgd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3amqixcnb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3nsmmpifm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3olufetmx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3tufsqdem.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3pdsyusgu.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3gcugunbm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xodgacfz.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3wdigpdjz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3euimcxbd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3npczwwnp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fgoxiden.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3tqucnyxg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jigqkfkl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3cwdtjdjt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3oqbmnmif.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ikgumcfb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3mcmpaoht.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nrpbueft.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3nksbvdit.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3syqwsxyb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3mrqlejme.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ewmoohjj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3prbfwcih.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lhstqiga.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tuoppwuv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3sutphvoy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3rvvmdazl.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hsborppp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3cthnwvds.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ctyscjfr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3gddyutuj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3yxlvxhml.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qggixjew.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3qwosmwsh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3tkbkmkvk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3pdogpzgg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3kgivqyma.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3bfobjreu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3plcihkbi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ikfwpbqm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3reqyrtil.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3xsuxottk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3xdiftatm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ptpsuduk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rpxgkupw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3icmqtcwa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hgjvuxxo.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3dzrckxgf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ysvfqbmd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qmrrnftx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lgexddsa.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3wrbylkfx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kepstmku.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cmajlgsb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mmknfwni.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tlsneord.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3znsuvqkx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3xjkbdhgr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ylvmbxjb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3doyuhadn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3jxscyudz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3djqbjwdx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3yzxgbfoa.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ukmkciqz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3fctwzjxm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3awwkrhyo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3fgtocmau.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xxuftvxn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3auiusgua.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3flgbtrfq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3fnpvrvyz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ferunnjb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3yycolfvc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3adyzspjx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3befeozfa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3mbctfzir.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hjumhecc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ywuskasd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3scebieph.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3uopudhhr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ctauttwo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3eyuacczl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qasamauy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3tvqopwya.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lkekhnuz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ayyfkmbn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lragcxwt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3foepbkxo.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3fdlutrdp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fkcoenyu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3jnxudcbf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rjqragvq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ldpzlqmb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3kxzpwkqk.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pkoyhner.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3rueqyapt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3sulgmufs.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3eyuixvwr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mjvqgxeh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3typkfiho.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tckxvfjc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3oytuzysu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ygbwtvvi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3fegrulyy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3llpyovva.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3axlnnxke.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bmfjsepz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3liciakuj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3oahmqbem.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bbfrocmg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xxmrxboj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bzzxcuso.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hyttxexq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3mswmjkuw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cuewrmwy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ncnvlaxd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3miqacwnw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3gjjzjgfd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3skupukaa.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zxdajuio.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ioqbchmu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qyqbwcgg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3xurdzgdy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vdccjybj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3oydhtsnq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ruvpijwn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3zxytqwnt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3wslcwbav.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3vxdqbuzn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3fooxglhy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3mlnoavij.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3gbzjtivr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3upapuexy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3iuvhuvds.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3qshyochn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3zrqwwetm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kxedkqoj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zlrkawcj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3yxssxdfo.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3bqvbxxqv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3iyzbtliu.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3mxyrmiya.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3fmnfnbcl.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3mftraltf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3npyyqeut.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3sorvxjul.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eeibfyko.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3wpewrkfc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3povrxxdc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3rtrnibjj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3desfjnhc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3giljncxn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fgkwqkkb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3agzwbume.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zyhbwmck.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ibigoyom.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3wvtiuymd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3fkijkaph.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3aglednnq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3wcditwrl.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vkjxnnfo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3odtuhkcp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3djeuguzr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zbnlwvqn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nhdutvel.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xxafrjru.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jzziauid.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pnxmvodq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ozobuuyq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rrlhbmyb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3bpbzqglz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yfutgoze.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3uklofqbd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3uchvghpc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3wfrmvdyo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3lbfxwurl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3htqzyrsu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3izxwapic.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3wmcssepz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3lwjvlfyx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3efrxwzmm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3gcgrqdwd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3mfalexqu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3qwyrslqd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3byddgmsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wbtvsjem.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3qkewimip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bgabuemv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ixazgymj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ugerwgyu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3eiegnegd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3muxxccze.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3fouiqwgo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3zmirouxt.html


<!-- 参考信息 -->