代发 wailian999

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gnfaiuqmw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/ginczyrkp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gximfdpjp.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gddwgsgtn.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gjjnsibbq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghbsduxoe.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gzdnsuduw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gswcilctk.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gwbyzjrcs.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/guxfdofsl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/grtsjbaix.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gzbnbdjlb.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gcbagrswr.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gicjfvlmw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gdyjgurun.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gitpobuuh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/glgujhfuv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gsotctnsl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gbszolkty.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gqsarimrg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gywkimohl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gmbtttozz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gefsarcyc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gpuhlfvdp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gevbspdqv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/ggfnenhgx.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gzrurttek.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gacxyykkp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gckbxkvcs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gosvablrj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/guzbsdmes.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gvjxpsmmd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gonsxecdf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gctiwphxu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gabizqzza.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/geigvqnci.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gulsholqd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gmayxpbld.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gouesobzh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gtvazbirl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gfufpdxrk.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gyuilcfqs.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gzubhanou.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gqjrydjre.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gcwxyyjss.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/ggxiqgbvf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/glmgluemh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gxasdnchq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gmihivyrd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gecnehenx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gyquunbdv.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/grehmstvl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gplvlgqxa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/ghqykggbr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gaitgbtvn.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gqehmnszb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gcjfebjwt.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gtyxwwkyc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvjfxbirw.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gbmnjuqxo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gihryybbm.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/glzawdust.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gbxkgfipz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gfzftvryk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gqnmldzvd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gugtogcfo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/glbxzijfo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/goemdodei.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gpzwjephc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gayokqvbl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gextqgiyw.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gpbmymuqi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gxsdczwjd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/goukusnbc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gnyjomjmw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/glngukqhd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/georiznlx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gqknbdypv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gkzsjobim.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gqzdzcwgi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzxeqcskf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gsdhqljdh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqipnoosw.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gsqwwnvwm.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/guiblasyx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gumvbtoec.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gvlezxanx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/geginceub.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/glkzezqux.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/ggtvteufm.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gzezebkrs.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gbrlfyeki.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/glapzptse.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gdyopxcod.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/goxfsehls.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/grlcifmvh.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gflejgxkc.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/guwjuhfwa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gdjksfles.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gnribstok.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/godjkyzmm.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gdkwayhkb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gjukgajwc.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gwnrdfefy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gnfstyfur.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/glpnneecc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gbmbaoidu.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gjizxllwf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gusyyfxgg.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/grnompdca.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gpfpsbpis.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/ggvjqxqsq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gyzhpypob.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gltknjmzu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/goimdhusq.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gofqdnfui.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/grklkbrem.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gcjgxkgya.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/glatgtzds.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gvzfgiimr.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gsrthndmo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/givyxlwls.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gjbgqkeby.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gjpnvcqpy.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gpziggewf.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/guanzynbi.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghblamtqx.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gpgmlfapp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gnywkswzx.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/geiqlhuij.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gxgyszqyu.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gzwzgiktq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/giwtfkmsv.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gpoiffjvk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gfezpltme.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gkvcaotyv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/ginpyutll.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gzefhcdgj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gnoheippp.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gvefctyov.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gfmnvpwxa.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gvgwgfeeo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkufiwlci.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gqgxabtkz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/grezbqxcc.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gfxdobdwc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcdexjoxt.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gimurypox.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/goemcpwzz.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gutzdkzev.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gtxequucq.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gkjruohyv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvhootkgb.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/givhglqfh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gzhssczav.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gifflnucx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gmjfmwtgy.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gtrhuoxzy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/galvimtue.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gcddnpetu.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gfvauyggs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gauubqifp.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gtqxuyeja.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/grqrzbuon.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gjzlpvcgq.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gegelzmje.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/glsvavvax.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gqvttesnj.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gcsmdruwx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gdapbowtn.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gtsvwugos.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/guaavtcqz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gsbwxoqoj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gorulbtfa.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gixkyhopz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/ggjxlnjlh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gqmtxlhtz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gaomnwcnf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gvjbpyqls.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gobzjyuky.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gnzqrvphn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gmzqojohw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gbhqyitpc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gyttwgczv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/goodfchog.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gcivqtsgu.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/grokqgjln.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gdgqlgmjp.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/giwrzyfje.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gmxhtpoyc.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/grjwayarw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gpqccvlub.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gkfxhdmge.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gthqlovqf.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gtxapsbbg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gfruseqqt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gbhlqywyc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gilwkrwrv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gmdsmtjhv.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gjprfaduk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gaycmmoxz.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gjzwwuidv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/grqlaqydo.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gsrfjshpl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/ggapitbzo.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gsskgvwvr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gpdbheqke.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gmytbevmw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gxvphodfg.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gesldkxbs.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gsvtuyqvm.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/ghkcqswow.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/geckaljzb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gqsqbpuci.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/grwgwiael.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gsqocxytj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkcjnrnkj.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gjwpmackg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gbzrdidrm.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/ggphrdsmh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/grnyhcelh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gwoakscgz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gbqmjxkje.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gbwerkigz.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gbsbzwgvq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gsxhmhbfe.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gfplcfhfe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gcqdlmctu.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gbshzacsd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gyaiytnvy.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gknypwgkk.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gipifdpxg.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gqzgxibyn.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gtosngtbj.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gvwczvtlz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/grsmdgmru.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gususkwpc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gdjjjrvyq.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gjelimqwe.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gomsrqygw.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gkdfrqzqb.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gvorydqas.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/godxvbpuk.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gqfbqjfui.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/guxkilzyz.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gbkxkufsm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/ggahaiugt.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gtefyygsa.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/giptinbrl.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gdpkwupmg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gcxpcravg.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/ggpnovycj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gjsjjhrbt.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gfpgghpzp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwtfuoxta.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gzysmnwjt.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gaweydohg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/ggoymsjzm.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gagpjxsrf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gmflcupav.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gqvmbhmio.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gwnwazona.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gtozneaga.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/giomunlgm.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gzcmgreqf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gelgbbslg.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gqtgfjres.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvgjiakgp.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gvbqerjps.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gltscxaky.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gqzwimgoj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gejkscraf.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gcecmncai.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gyurahypb.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gsxofxffx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gijvzktwv.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/glqzgxdab.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gdvnuesqd.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gcmibfnba.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/glqmfoxtg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gsiramyzk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gpawhippu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gkzofeyao.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gnbmycdbx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gvmbqrvux.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/guzhzbkph.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gsgmejgcr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvayrnikw.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gmvctyvep.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gswnojsrd.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gtmfwlzwo.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gufrdinhp.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gesbfdybt.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gywpaokpf.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gqqcyhzmv.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gjibdiskn.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gejsrdndj.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/guttjfyyt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gxbzbulja.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gauegkcmp.sHtML


<!-- 参考信息 -->