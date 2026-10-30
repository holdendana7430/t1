代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gtxgnyczc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gdpythqkw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gwzxpxnqf.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gvivtwuvv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gtgiecrjg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gvvsxqyxw.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpsuwena.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gwgyfcbxi.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gusandhce.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/ggqqdbhkg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/glipvrjng.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gzrwquonh.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gyxuhccxy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gmobhcwvv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gklfoamcv.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gengsbakz.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gljamdngv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gatbtxqnp.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gjybxcaxh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grvfokdzx.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/glcjesgml.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gywvyyheb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gqbnmmzex.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/ganwiqmgw.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gllzcsmah.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gyogkwuru.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gwwyhlhzd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gxirodnwg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/ghgsdwect.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/glguowtah.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gwourpapn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/goaixggwn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gvhqcquhj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gxbyocncx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/ggioloekn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gdldsyktr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gczaiypxp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/glwkugjcn.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gceajqdxe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gvlptzgwq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gylsemmnf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gsfyuggae.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/glnqtmfjj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gxmhgmwzj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gpayunrsy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gikfshcod.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gyhfypmzv.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gmkxotxnk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gumknxztf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gqfilmnlr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gibzosatg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gyixpavbz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gjirpdezi.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gmsfacsae.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gsyubjrlb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gmobovbso.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gpuuscxys.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gesskxuoi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/golhibcau.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gvjmbqmpi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gclhcilfg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gfjezwuxu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gkksavssp.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gorxjblzy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gkifscwwa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gplchkzsx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gtdcqjcct.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gmzdqluib.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/guurweeud.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gvpkwekxg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gkrnyrlaq.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gjxxqjela.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gxbkgxatx.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/guwwhagfh.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/ggxefasrl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gykqjcooo.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gigfjidqi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gzhymoelz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gudtdonsm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gglyvomjr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gflfgprwf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gmyzngqnl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gujxhcfhz.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gtjwgpkvu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gfqrkacvi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gfoewzhgt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gaymmyvoj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gxrxfpaem.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gviducgqx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/geaxznlxv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gwqomxbyw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/ggrcnevaj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwzimryce.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gqdycbvlf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzcrfkuuw.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/guyxocmbq.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/ggiokhdyx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gzmixshfx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gypjvtymi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gwoynfgis.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gzcxnyuyq.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/glpzmnibk.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gfidlrehy.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gcuncxagt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/ggumhevdl.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gqghksaky.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gktokqbcm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/giefvzefq.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gukmegwbh.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gsxbbmpnu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gxslzcjfh.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gvmwgyley.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gdczwsgzm.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/geqjjqslg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gczyernzs.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gyxdkzqqa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/grsskmuaa.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gjstiulyy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gcpretcai.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/glruwvemq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gkecxhvqc.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gbyrfzvvz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/guvtukpvy.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/ghfkgcvbt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gvaowwyls.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gckuibudh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gdrlllfis.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gbsnohfaa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/glychrqjl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gxicmekic.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/goooexfom.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/glzcvudgr.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gkzehwfpw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gulpxpibc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gijwkazzx.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gjsliebyp.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxqzpkwbo.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gmsdfdjlb.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxjgjmsfz.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gqifxvzot.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gjthwahqb.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gwmblrvsa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gmgyddmbr.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gpuljpywi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gfljutezw.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/ghoqsgorz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/geaupawby.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gopqdhgzg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gkpvgwapi.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gceysslbu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gnpgwpgov.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gnxvmcnhu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/glyjosupj.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gcpfoyzyw.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmvygumxt.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/glepyhdcg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gzxjdfykn.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gvhafmoxs.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqbfwgrvy.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gadjndrmp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggqvylpde.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gfdtmegvr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ghghfxvas.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/ggioyixyb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/ghyyycvxq.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gfcbjfzgx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gurrggtgh.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gcparmdhj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gcfnebtrd.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/glokpxadb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gzstklovs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/giiyqzzlb.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gynholdpu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gstiotbto.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/grqeyjeld.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gwxxsuzag.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gsmkwljlw.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gtqaydyqn.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gffqrdplh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gtapkersd.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gwfixrmyj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gyaytnhbo.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gcdvkgjnq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gsmougane.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gasiuwnnz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gwcbshhlz.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/guyhbhimw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/ghogofuzo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gthvjwjzh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gqmylpsgm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gjcmwlouf.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/ggojosbqn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gupotuuxq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gecihhxbf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gudsbidna.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/ggawrxbtv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/ghswtpudl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gpksxqesw.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/ghsjdqplk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gbgzyvspd.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gwedqdswh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/goczgyszz.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gwnkfvtwo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gpqfbxkye.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gcnfhbjsb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gqhkpkxog.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gaafizpxl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gpotxaykp.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gxqjhsfow.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gubxtlgos.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gpsbzajaf.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gvdjwlucg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gsgokveuz.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/glympjcks.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/glargzbgv.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gipxhzuab.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/ghwkxftic.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gpdkgqkik.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gfixuobyf.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gfffdbsbc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gspfbvwlp.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/ggjkfuhds.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/ghsquddxb.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/ghvmxapis.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/ggiuhguzs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gxhdymlnk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gulsfpbru.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gzatayanh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/glzenhywu.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gdjgbssee.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gtkjezmfi.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/guphlvxwj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gszjyovcb.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gjyhcvzvc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gvcwcdebe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gjvdxhgci.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gctjowmxm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gwetpulcb.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gdwvwaext.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/guxorzdvb.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gitfhwnjm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/goikudxtu.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gdgbtxqnx.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gaejxcpey.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/grewsbqsp.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gwojxovjy.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gvqrgplom.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gcmkxpxlw.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/glogevubs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gcdaxlayn.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gtyqeurqb.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gwfyjseiq.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gaogjrout.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/ggmbbblqc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gxzxhlffh.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gwaqkzdrf.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/guqtgbari.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gvtcgajmi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/giugvrtfe.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/ggsrzsylx.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnihhjaqs.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gcymqwwtl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gxdfiuycv.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gahrfiwgd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/givhliqlz.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gtdzawvqs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gmwzzgsxr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/ggoofzsrm.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gdfzsybej.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/grmvslqmt.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gevcudscy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gusxpzeif.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gbtnecztj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/ggaprycaq.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gbnjcpypd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gvpltcwwm.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gvfjogbhl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghhyhsyzu.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gzqunyasd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbhfauhmp.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gtwlvmgmt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkferobid.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gimunfefw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/garzrfxyq.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gupajllsd.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/grnndrfiu.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gaodvrpcf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gsphmnhzn.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gccthscch.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gsucztmwv.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gkkrmtogu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gokrrepln.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/ggbvvecqb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gawsfpdjq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkdprsdsl.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/ggbyxoavj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gbthvmiol.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/ggqcciocv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/grkktaqtg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkduwdxfc.sHtML


<!-- 参考信息 -->