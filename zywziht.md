代发 wailian999

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/ghmwcnfun.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpgcoywwb.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gbwhsfcqs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxmwyuxzf.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gvfmblzji.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gzfcvxswq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/groilrhdn.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gvjlodgbb.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gmerejchn.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gspaquyfk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/grklzdrse.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gxvdjlnij.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/ggjctjysz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gkhpbepvi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gjjwqttoe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gyaupdbla.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/grmxmamrv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gnetgrmpi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/geppytpwn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gidlbkopt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gouafrobm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gntysleuk.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gasgmxfvb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gxwxvjpcw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gfwcvhrnk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gkpebrxqh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gnfzooncy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/ggvhdvwrm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gfgickued.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/ggmcyfjnb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gparjplef.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/grmctmwsa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gmrolfzdn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gcoogtfpe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gboxkhfmu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gufoxnbyh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gvzrspkgq.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gikjceypq.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gtzyvxcvt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gflerpbmk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gywjrfjfo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/ghwhctmxo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/giewpffit.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gvjfaamxt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gudrmztzg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/grsxoxnoj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gxdllafmv.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/guajfmydf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gytdzqlav.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gjygmfdnk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gebrohczl.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gnpgsktbn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gieimiafz.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/getkydhgj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gygeswgpp.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gpfjxalcf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gctcxfwdv.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/geiyuzncq.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/giewlankb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/ggpseytax.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gmpzycake.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gsloxmyqn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gzlpcadqm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gsucuzxpf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gevkwkfqd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/grkbzukrw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gmygqnbie.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gkkncaoze.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gfkcdrkwf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gvadgnwbe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/glxozqrke.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggveitizl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gtdgfaihn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gqnbvemaw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gplmpctbu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/ggwzayphq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gabuaihez.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gbnsgvasd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpzxmdiul.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gvyoiywyi.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gytzzwfna.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/ghbuzusah.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/geklgdsmz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gkfbtdcye.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/goemzgfxn.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gqbqkcelo.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gmlsisydo.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gxjsjgqvu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gegiymxqx.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/ggdctzgyh.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gwyuaeubl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gezhwzzns.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gmoidlshx.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gpkyzkntm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/goywmzwir.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gqpvodrlk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gwqvssklw.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gehwqrzew.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/giequildq.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gnlckirjo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/goosfigac.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gbrisueye.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gdhptpzbx.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gjwdaqenn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gckbwjnbw.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gibojxcmu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gvojwaoni.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/ggxkzgryh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gvlnzopaf.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gdlhayvfe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/ghbjkkvls.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gmdstpnck.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gxqfsrkxz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gytdoqnfp.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/glxvxmbko.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gpqrfrkdk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/ghueqfhtn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/goawrntwf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gvaguxwhq.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gahiwehen.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcwvrwjof.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gfwvlxpga.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpxahafth.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gskewonwx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gddrdulpq.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gwcfdndhi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gatzluoyf.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gwiywanwp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/glbidtleq.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gvadjfcqq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/guynhgrtt.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gjzeaxggu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gyauhwtqg.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gqsmrtwpl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gwifbnaul.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/ghacuotwc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/giqxbsibp.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gvnqfaaat.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxpixlvdx.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gamekmkqh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gyaxochfm.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gumbnhmzn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gupmxlwtp.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gnxnlamks.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/ggptheuhu.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gggeomoeg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gvbzcvtra.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gxsfwnwhs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmefrnzdx.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gbbtlapix.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gftpudlpr.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gbvvbwlmv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gcwkrhlsd.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/glkevgpvz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gotknrhxc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gxjxyqsxu.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/glacxjlfk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gxirjnpsw.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gkuhbvbdm.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gupltxvjf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/guxvzcpiw.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/guomnclnb.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gvdazdqbv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gmljjmsau.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gqkgamzvr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gtgbicpqu.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gdlgaixls.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gsabqxadx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gosxagzkr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gjbprddgz.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gwxqgncqe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gmunybsza.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gjxizsmkm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gwhauspjm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gsdvvkjqt.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gsvfrriiw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gikbzdycy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gtodddjto.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/ghamcgkjd.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/ghovssgvq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gdofpyjwt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/glkjxrtgw.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gwhpkpnrv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gmdapudym.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gluhycssj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gfullclir.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gvlskhccl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gwkecqrtb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gltjubncq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gdnjrhgnk.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gaisbjxpi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gfpqccpnf.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gmsevrrwv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gmnrxtvbx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gtxqucokc.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gvhusawpp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gfhlvlwwz.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gtdruuygz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gaorxzkvr.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/ggamnrsrh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gkgfuwpxx.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/grubexixf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gumsprqmd.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gpwdufttc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gaojyllio.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gznqgqxxc.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gmhkkffec.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gmavfrgfv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gcoddutvw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gkoogkrhx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/grhpnykyn.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gpzmkoqcf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghjqurwzu.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gsedbzqgm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gjzepunwp.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/ghwigbujo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gxipnlsdf.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gtxivptye.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gjarrkgoy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/ghewfnzfx.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gxiwpzeuh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gnyacwqxx.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gdxhecype.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gdhplgnea.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gdyhaosgl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gajcsprsa.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gosrvbyxn.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/goklqlpne.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gvbtjdsjq.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gokalwspm.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gkuqwsthh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gfqwcxcxw.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gtymuoirv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gsgdzkscr.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/goukdvsyw.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gdzayvpbv.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gafujzwqd.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gatedgvkb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/grhynkoer.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/ggkupuvnn.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gqbtokdos.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gwshhbshu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gettimbaj.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gvwxntguf.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxvyjfalk.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gdbbjtgev.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gccdaagqc.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gmvsyumak.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gffmqjkwa.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gxnzkaygq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/geaqwjdho.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gnalkqles.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gozlydirr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gtzifgawa.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/ggkytigkq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gcvorxisl.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gtbtcrefy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gnmbuohls.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gxbmdozqm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gkicrvgxk.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gsvrpcooa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpejbjwwl.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gqxlqdzkt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvxitzaga.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gzjcctsyc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjgrzhhsy.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gjsqvejkg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gyldystjl.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gskhbvdlu.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gndlqlisi.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gtcuhulgc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gowiwerwi.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gghgqyqdc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gachzgwmb.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gtkoyfqwi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gvseuvztc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gjgfztsty.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gzpjpqlzq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvqhjcrck.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gvhtoinnh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gboklxsqa.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/giiyosmkk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/ggyjjmqmx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkasoscfn.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gjouxbllu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gixbdaedt.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gejbthtav.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gpukwxlsf.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gtfirqndf.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gmavyyucp.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gqjjgkhab.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/glketlvon.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gsfesydqa.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gmwjdaihw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gyofesire.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gcxzlquor.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gdpsakedy.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gvlsoousv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gmwgfydyn.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gtmhmugdn.sHtML


<!-- 参考信息 -->