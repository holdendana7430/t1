代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gedwvzpda.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gwkfbvytl.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gsbsidzqx.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/guvbgivmo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gwbzebkgk.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grhywvmbq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gwebtwijx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gxiclckyc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/glmtdwcci.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gymyukvoe.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwndwuoyi.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gvsajdzio.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gxtsarfvp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gchpszuux.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gvcakljil.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gemtoxwtb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gkjiftruu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/glsmjizag.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gxoxedzzp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/glklnmkmb.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/glqvlturz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gdcbpzawv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/grlzmcxns.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/givripzdd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gxopyxcct.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/ggwnupidn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gsnikearz.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gjkxyfvdu.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gqnnarfih.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmdttvkiv.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gkjhntrms.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gphjjvltx.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/ghqfaabeb.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gtwqsxtnf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/ggtzxbmyn.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gkxunionr.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gsbfmfxup.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gpmljccfm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/ghwtoikde.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gcerkslgy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gsiqihrqj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/govufmouh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/ghjydgbap.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gaftdgbzq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gsnxadpzx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gifnckzkd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gttivzhlw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gilumxyjm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gjqeetysc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gozysrrzp.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/glbteddax.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/giyqjsxex.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/ggaxidovh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gxdlmuwcy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gnxdrxpwx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gcupmxdaz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/ggxmujotl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnaferbd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gcriujleq.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gjgenmoho.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gqcklltfi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gyhwsyjha.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/ghymkezcp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gdkmkgspv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gtlayzsas.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gvjozqyxs.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gwhxxoruc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gbrgzfvyh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gicxvfyya.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gatecrdjh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gcfpncfvb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gwwmxnfku.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gmfpahhcu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gdypkzojl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gtismqegu.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gicawoibk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gmfagkytx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gkyfgmnbv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gewkjsldz.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gcjnkahpf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gvtrafule.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gofvzhtlr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gnlzkemsb.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/grtxqzvxd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gilqtrewy.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gctuobhld.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/grdefggxa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/grekpttpc.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/glmsncruu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gwepmqreu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gppsznuzi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gztzgqcbt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gpzxkhmfy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/glotvzved.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gotwneqqb.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gjjmznwha.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gyndwotgb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gqfufhgwz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gszjafcik.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gyodsxwgi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gkljtdkqb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gvqbumjzn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gvnlzvrhi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gntudtgax.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfoqqzpuf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gmyalfsro.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzpjzqgmx.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/ggwkgfrmq.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/ggszpavhz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gvlfwccph.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gqsdtyuhs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gbsekhqvc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gsppbdozj.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gqgaqzrzn.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gdwbvcsdt.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gwmfekqbz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gbbmijxnp.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gcsbhdkqk.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gygxfnngd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gnkyptjtn.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gturrfcwk.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gqgublhuo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gqprhkort.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gcpnunips.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gsrmalekm.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gpnlagzdy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/guzalcnmv.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gljzaektj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gwutrfzvy.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gjelmcqzd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gsvlhvlrf.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/glnutwubn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gltbkgvgg.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/giucyitqf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gmtdiqwgi.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gxrgflrac.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gqurbgesh.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/ggbggckyq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gkuwhugon.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gelzyrvlk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gyrxzrvsw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/grgscdmxf.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gprjbbneu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gkmxazfix.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gurnaosax.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gicjchfks.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gnzhqezmi.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gsgdgwbni.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gnjcgtzhr.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gaycduwof.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfmapgfpw.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gdkqjqazs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/ggesmifzp.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gqxdlkciw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/ggxawgbeg.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gbficshpp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/grkvnraka.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gfrztjhbd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gsnuaqlcb.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gkfqrrnnh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gfstqozio.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gsnuwpzja.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/geoifvgkj.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gukpjeueo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gfuewamvi.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/ghxkhlfzf.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gyzibexpv.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gfknpmhdb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gqezrladb.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gsqssivxh.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gientntkr.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gkcrqqalw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggncbuawd.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gximmfjgy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/glzfnrfln.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gmnotpuex.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfvjtpgbn.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gmxuddigt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gwfqodvpz.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/ggidtpnqy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gcfbkdebb.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gqoekmmik.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gwzhctytc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gailuelro.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gtxgobquf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gfgeldzsf.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gwlwrtguq.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gmzxifkff.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gumwrxsmi.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gvnkutyuf.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gehvzrscy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gymgbaffy.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gmcqzaaml.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gnhqqzyvj.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gavfxrnhu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gprhsrixd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gcbbpvvpw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gogyajjaj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gutbmowxx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/govblppge.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gzztmhjvk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gdsfzckyb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gfmxqsgci.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gurejsumd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gffgbthma.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gbodxfebr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gemvrajtz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gvzfikgyj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gqmqnpdur.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gwyhnifyb.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gjdgcgany.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gfxqutqxy.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gyoztyjiz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gkgtorxnl.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gmfbpfnzc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gshdwnvdo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gpqmehwkj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gitpivjzj.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/ghujpprgt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gpahiotdy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/ggyazvyxg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/ghvocncen.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gtorwpnyv.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gkhgbbdtg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/goweibueh.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/geuejhmkj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gtfgukzxr.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gsmelkdkg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/giyhnpifk.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gowypisme.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/glxnmnlsq.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gxcxkhmyz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gcllqtsls.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gpgjauuvn.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/grchingdl.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/grzbdlcxi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/ggxryitgd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gspjwfrcm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/glagehgir.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gevciciya.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gavnfoumg.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gxhgimbqs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gqtdpndvv.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gzmswypez.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gwaxyaehc.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gmvdjdopw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gnkkvtnpj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/govjinhel.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gyfqepmah.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gfkogkqba.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gyauounwt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/geezwmazz.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gozydkkkj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gllmlwwci.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gyszurkqe.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gdcqfaywx.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gvemqlalg.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gvbyuoujy.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gookctiuf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gboscknkd.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/geotahgsh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gbjetxdca.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gtnnzkiob.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gycqwgmsv.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gbdxhwcyw.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gxuypkqds.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/ghyoqkpmd.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gvvcgiuvm.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/ghypadyje.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gcxczumxj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gvfzvorax.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gyhbphabj.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdwshwiaz.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gzcvwghpz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/guyikvwbv.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/ghmkwzmid.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gsnuxnene.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gjotsuzwy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gqzfapqtd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gkribqltv.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gafglkgur.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gunnrqxbr.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gqrbcliry.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/ggimpkqmz.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gbcotiqrz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gylglginf.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/goiqhqzhy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gqgwvdtsh.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gwangxbkn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gugumjwjy.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/genhkeumg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/goijpbbno.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gtxyejffo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwoodewrh.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/ghmkfcqzh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grbepnmqy.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gwivohnrq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxerijxjx.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gdivldyzh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gvoxaqcsz.sHtML


<!-- 参考信息 -->