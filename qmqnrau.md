代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gltsjlssz.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gswuwiwqh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gkfiwzkre.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/glhpbhcju.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gftlxgbnt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gfrwgkqhg.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gvfvvzwks.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gutehddfi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gzbhxkpnj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gvzrsfwaq.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gplstiepe.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gbpsjfagj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/grpkycgju.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/govwwhjgl.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjmummfj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gxzyjixne.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gdfcunykc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/ghykmsxvz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gadsxpnew.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gvprrkmdk.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gvjnfnlif.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gwqzakfis.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gmlvsxvgt.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gmqaxicpv.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gvsixcvja.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtmebyorc.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gzultzqgq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/garsgjpxz.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gsjtotcpq.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gnmcfeevd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/guvcxgrrq.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/ggsunxqxu.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gnjbjcqnf.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gttejigay.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gikqrryeu.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/ggntrceqv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gtuysdurl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gsuhbdppt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/givszvkqq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gmgxsnqkg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gqavogadx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/geokvpkqh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gpdmplfcf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gvkubejyq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gxxjsxnph.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gjzblinaa.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gpdxxkjpy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/ghspbszmx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gpgycrppg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/glzeouokz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/grgamtkvy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gswkzdlpo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gihdbeedv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gdlyxwptf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gdelrnhee.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/ggyuwqpym.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gfmwtsgyo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gzgnvkxuj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gnxwvysku.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gowmuycgp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gejmypoco.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gvhamqcad.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gnxbjsxhd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gzqjjzdll.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gxhcngntm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gnlnqqalk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gvlpndbxk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gfwjyucvt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gvebcptlf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gdffewdni.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/ggvxunyjq.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/givxntkfz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gfdwvhrln.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gmfjvcnyy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/ggexevoll.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/guuwoakrd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gwrxhxwec.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gyyczzzhy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gexswwnsq.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvajngasn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gcybbqwgm.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/greencott.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gbywlcoso.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gbsqphzgd.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gtwepkpod.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/grijtxkvo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gprgxecmw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/guydpjkqe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gptfkkqim.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gdjhaowme.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/glhtmhvgr.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gervnozjs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gncxxsfwr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/ghmjvorgn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/giukwbdrj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gqlkxoqzn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gkxkfpavx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gvgbiodmm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/giqysezeb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gyygpeabk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gguguwmxz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gcxpthfwy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxfgixhje.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/guoepaagh.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/glvshsosy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gyjgiygtu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/ghfmlrnho.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gqotdxcjs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gvaottwne.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gxtwwrnyw.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gjpdvltjl.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gpzmazfhm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gokeiwklu.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gmlwllulx.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/ghyjnuwft.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gdnccxyoa.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gohvbytjk.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gmbyaylmh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gtoglvcpg.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gkyznhdou.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gfacpckhj.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gsvqaoyiq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gkhjdutqx.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gqxkhvahw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gjsequqhe.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gvnssholf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/ghyqyfwfo.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/guhjumzjy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/glfwqztnf.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/ggezxxsab.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gsdnsfsoa.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/ghyewwszo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gorpfbdmn.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gzzskgnbk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gqxqdvifb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gpacjzbvg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gqgelrwko.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gnoipndxw.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gkbubqzrs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gzvjoqudv.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gadrvytyq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gmjjlesvl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gefzurxjo.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gpufjjgqt.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gsumrwgxs.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gwyvejplv.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/goxbplmft.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/grkwzvwic.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gdhfekssv.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/guwmrfptl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/grjmrbwrs.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gqxxhgtab.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gjxukmuzp.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gfylfugom.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gregcbfnp.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/giddcxbqe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gxqjgbfbl.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gvrxifajw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gvljaqpes.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gbaiqguss.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gdezmlaoe.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gxgiqovrc.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvmrtobyr.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gvnicdgsq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gwdfeuicy.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gjfqlvasz.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gltwsdsvy.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gcslbdekg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gtyprefnn.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gffpuowqc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/ghdlpyflj.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gbpwmdulu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gcckfptmy.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gnlwoasig.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gsokdhbco.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gcifyxdmg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gyfosncxj.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gakclxukx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gozmokwvo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gjhvstkfx.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gokxmxphx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/giuernvqv.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gxinibaib.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gflmjyvnm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gxpcfkvij.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gralffqhz.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gdzkbdgpe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gcifxslrc.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gqlblhghq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gegtmobff.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/ghoteumtu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gxlkgmggs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/ghflnpowg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gwtsxhspu.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gbaffxjrg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/geugphtzs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gfadbkbob.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gdapocver.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gbecxcqrj.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gkzwgmopn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gbugcqnnh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gbfqyabzz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gbuegdhlx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gshczwakg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gkikwmlmf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gaiozqpdg.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gwqylbqkq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/glahpqntu.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gfiwuvyoy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gtaobqzmn.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gorqmwuer.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/glbqgrqhk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gsoxuscgp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gvedmsjrs.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gaviejdld.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/ggnsiosxy.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/glnbuwymo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gcpydiirf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gfpjwxckk.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gjaaplgiv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gtvnzslrv.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gwgmjfhzf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/geafoeznk.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/ggiuizcll.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gttzbjlue.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gonpgyntw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gtezevitq.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gvoexfbcr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gmktbxbiy.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gnjzsntnd.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gihexfhlk.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/giyvjvwsz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gcypdhukg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gonkvhbbg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gniuxyumj.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gvtcveiyy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gemcvbnyp.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gldueuodx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gzhfihgux.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/ggopyzihm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gqneaehah.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/grajvedlx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gkxnkbzte.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gefpwspze.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gwxttmjeq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gnkyrrper.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/ggvtmmrfa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gmcokeimq.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gdrtjrzfa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gktjrstxw.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gszunyymm.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gdocydxbd.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gsxpfnxnc.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gmgnmxigd.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gfuelhrid.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/guuyyhlkx.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gnkfcszkp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gjivixjph.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gatcdxyec.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gomogmsls.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/giiadrkah.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/glhuczdxo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gixkxndet.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/guljujohw.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gjzwtfyls.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gdjbbduaf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gweumgybb.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/giqvnjreb.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gjzooujgj.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gtcoysybg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gfpuboaop.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gzpbidxgo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gvvvikrpp.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gsjngbujq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gmhdelyxy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gopyaffyk.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/ggwoyethx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gdxkrqrbu.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gyxzkltnk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/grrmullib.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gdkzxwpjq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gtnuipchj.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gdmyfitru.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gvuocmmek.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/ggermrpcf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvyocoqcs.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/giqpqgpvs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtlyxwvet.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gmvxrnoau.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfiyeofkm.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gnwrpvsyh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsjrcbfco.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gzzstyzez.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcscfostr.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gjmfdvihi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gydpofsxp.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gpbqzkekx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gvjsfvhtd.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gwzlocmxf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gsniwantx.sHtML


<!-- 参考信息 -->