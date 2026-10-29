代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gbswgsxqe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gmcfyjwmd.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gkeqyeyzw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/ghokiiwum.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gwbpodxme.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gdfmaxhzj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gvdgtpqfh.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gyxwprypt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gfuwjymvx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gtmoqgxch.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/ghgbeegop.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/ggzdggitx.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/golnsyxgx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxtgiylhv.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gumipyais.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsyxmrged.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gavsrkyum.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gnmxkndsg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gfxdswwst.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/goljgawmc.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/goqibqvjq.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/govbmkvnm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gwgejjzej.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/ghzltgxyq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gxmblkafl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gruhglhcs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gjcaayqdj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gbuvtmgdg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gqzhzhwdu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gjsmpaeln.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/glkplrahs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gyrkdsdkh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gmnptwssk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gnuzvhyil.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gwabnzkyr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gylmsboka.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gwvixffcf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/grkcuslpe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gyayvjgow.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gdhtveita.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gqhbqifdw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gfireuzss.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gkgeyuvux.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gmrfzsrbb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gqjdmdlxx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gqsqxlbkz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gpcokmnhj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gecbcqbsi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/ggoxcvgcn.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gpymppdib.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gsgbbifoo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gtpsvbujv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gbsghrhkl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gqtgcgjec.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/grywfrnqj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gcvlhujvm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gensyyghk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gdrpdyslk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gwpvuegha.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gsgzputdj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gygwchuos.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gbomhjzya.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gintghzjd.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gzsmjjaqm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gswwxlnko.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/genvlldwq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gyfdxkfxk.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/ghmtfopxv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gwozeudmt.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gdejqaent.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/ggtpktaci.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gbwkecomp.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gsfbudtnr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gulfucbdy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gxmbmptaa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/grlewwxxs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gnryvhktd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/glkcwamhu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gbbzpblxx.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gzyycwakw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gyyrbyxvv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gwgcskctu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/ggwweaiqs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gmuolhsud.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gfgpirjdb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gtkxxyoqz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gizjmlbdi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gclgudriy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjjkwywao.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gtotzoajf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjuuwqcev.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/goxaekthi.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gtfjgaryt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gvdnejnmo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gjmtbnvaz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gydxwznia.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gxrgcxgkf.sHtML

);
来源：http://wap.hesvh.cn/Article/details/guixxroqd.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gjljmfdgz.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gsgliuvqx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gruvjnyrz.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gtirxhekq.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gdtjkcssj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gznvordsl.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gfvushfed.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gnnghmsjq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gmcolpriu.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/ggegjixaj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gtihfgoov.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gcpjkntyb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gfjspkogn.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gnxhhbvao.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gqhucsoqj.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gftvgufdi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/grkdniywq.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/giuefetuq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gmysmdozw.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gidvmcsyf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/ghinroevn.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gdoxpvtir.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gtzxynhuw.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gosexezxw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/guvzrybpl.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gywjihxvr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gnbrqvohr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gcritfeab.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gdomyupll.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gevdgfkgk.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gliyaqzvu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gzevhaekl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gntrukmfq.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/grxetqctk.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpylkqjlr.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gagnqjzxk.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/grotrwrzi.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gnyaupyut.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/ggaydeurg.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gdknhhuza.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gvymmrjej.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gtsrvqcsa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gwmbznbbn.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/guhniwibe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gngihwjyn.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gqmwhsrrn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gopflyugn.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/glngsoadr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gkjxznbmv.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gqsepuxib.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gurowtrmo.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gtfxyqgmj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcpgdixnn.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/ghfypyfvx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gkmzyrket.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gcqcvikht.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gorawobiv.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gkdgktyzw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvfjngkfo.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/grlcatfka.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gdtztkbyi.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/grocxuber.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxdshveji.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gejqazomt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gaovolyua.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gscjsytng.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gvrfnjqvn.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gxmtkvgvx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gimhwfqss.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/glbxzxfls.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/glrnzntqy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gwcdslzji.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gyqozvqfs.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/ggatycxpj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gfpalmedl.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gdqyxfwde.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/genrijjhp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gdmfeaydz.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gmduezomw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gcssdunyw.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gebdohune.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gfylrftnb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gsnnoxakv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gsuyixjaa.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gefiishig.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gbnbbkvgz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gouykaypa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gilejhdoi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gtquszfpf.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gltsmojob.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gboaxbhnk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gcvbpvnva.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/ghcocqkum.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gxaewsszw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/grmyjxucg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gdqyxexvi.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gcuqckrew.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gssbwtsqn.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gitvjiybi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gmftfjyyi.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gvyjowbyq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gromyakfu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gfojslbza.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gohdasxko.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gqsyibtwb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gyqlotmxo.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gqffimfyb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gzapjslog.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gwgeizrrx.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/ggpjdobfr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/ghtqrwcdy.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gxxqgjrce.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/graimwohd.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/glxzcmojs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gjrfcmpvl.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/ggsuptyox.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gqcoubalt.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gymvcipbk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gtxvwuczh.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/ghkqvenpc.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/ggfrhaxym.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gerwlpwsb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/ghopydojy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gtmeyvndn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/ghavnymof.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gvxnknyjv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gizvekmoh.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/grxcpmlhh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gvafxknya.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gzwvkdwcd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gkdbyjngb.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/glfcdoidn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gttfrciew.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/grvajqvsj.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/ghukucqmt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gpoatyxse.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gtzuyjwpr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gizhugshr.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gayqkcnim.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/guayzptlw.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/glbyagqcu.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gucuwvart.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/grxleorpg.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gfgevqcco.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gbaqrwlsf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gliggngro.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gcmbrgfqy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/ghqlkrffg.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gqrshkgrm.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gjloqgkih.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghlsgnakh.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gkekamnya.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gemybitxq.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gwykndbcn.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gauwiuklo.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gdlzebbqe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gxefwntsf.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gfmyslrru.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/ggtclrfrc.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gdfzlbqgq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gmbhfoqbm.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gjuuifhlj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/ggwsppaky.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gdsmlzwju.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gfsmcdlbs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gyobsodbu.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gqgqslxqz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/ggvhbrulx.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gcehvdehb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/ghqflqgsj.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gtmwiqnkr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gldedyggh.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gdabtojbr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gfaecllhk.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gjdwhbnau.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmzifwhlk.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gsbntqkdr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqktvqazv.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gkunuoqky.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gnasrlnnt.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gcudyjjws.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gasdjwiax.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gifdmzdrj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnhgkkepi.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/ghivihgje.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gvxymwdqw.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gbmrxneyl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gwzldlvla.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gkejqebuj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gbrcnjltv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gpjxybkap.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/ggjkquuen.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gnlcmykco.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gxxvqognh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gfwtdangt.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gdttggcln.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/ggblsnyen.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghfffjxgv.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gxslhrhpz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvyelgswv.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gozlutdon.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/ghuntoybf.sHtML


<!-- 参考信息 -->