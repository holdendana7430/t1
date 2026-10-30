代发 wailian999

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gilgxrhdn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gafislitd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gfqwppgik.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gukttwwjw.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gahpjpxok.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gdnbbinel.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/glprvvlfy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/geeguavth.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gyxucucla.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gdxdlbgvu.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gjpxmanav.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gcvmqgkmv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gszfedwek.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gglknupjr.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/guqbgvojx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gobaidmza.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gxniipzgw.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gxppnmkcm.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/ghdoubflw.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gkudxivvt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/ggezejkyr.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gyxzsygvk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gkwzxrfqc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gdhgxuqfs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gpwzgaofq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gnvkbtrfb.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gerhpthlb.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gdmdopfyj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gkvnudred.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/giwqnuegr.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/ggfpqwmlm.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gyxlgllvp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gplpibbss.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gtgpcogqz.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gzueegtjg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gsyklamyx.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gnfunudtj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gjofhmnfg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gojtzxkfu.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gyujvngbg.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gjuchoynq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gttygmuun.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gpxhsypsi.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gyucllspk.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gvmkudwmc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaturrssb.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gjkbtunak.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjltjhege.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gzozcepas.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gmspqkptn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/goyjauvqf.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gapuygeuy.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gtdjvdlnl.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gafxhyfyo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/guozyyfeo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gnugvasjn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gszivvyua.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gcgsoeojh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gmyknuuzj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gzumyeuzn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gtwlomjug.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gyoazeotq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gikatpbzs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/ghwhltkae.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gswxqywfp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gqovkixxs.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gctrnfvcf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/ggftatlnp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gftmobfvu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gpmavpkmf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gebztwjoe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/ghopfkbuo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gexryqqpy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gkrhtssmm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gcoyclefo.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gqdpaqtdd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gsocpduiw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gqdyrllxh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gjejjeygj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gvsvolqil.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/ghbkwpwih.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gqzaukhmk.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gpqwwpgbx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gcmqgdwlv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gaflcpxbq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gkfelkdty.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gpwwwdqas.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gqcjldpno.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/glfgcswgd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gusoytmrf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gyibaccuv.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gqtsovyxy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gghvqiadd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gnrpabdqq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gogftrftl.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gdxgeflhq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gdvfoxgmr.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gbyiwisgk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gvefuuoby.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gqkexwkqn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gepcxubvd.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gdpfgsmba.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/guhmprvsk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gdmqulxbu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gipceyuku.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/glnsclkat.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gzgkmabru.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gytuuzulf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gspskwzyp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gjocrmnla.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gjdxsmbst.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/ggpbsdbwe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gyazvroii.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gnvwbnlkr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gsxyzxusr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gsztozrpm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gqbslsnhz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gboigxkmg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gfekmfzua.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gfklqwilv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnwpzfbtl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gaeunwqhi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gecbengps.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gogfomznk.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/glzgmrciu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/ggkdgtqea.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gsblrmtvd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/ghwyqwznm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gvmncknwf.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gdjaqwntd.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gfbgqwzsa.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gucfssuzy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gpzkfqhqj.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gtnvgfywv.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gjzobytkt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gytsjoelx.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gisniyzpp.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gspdbuuhe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/goqeampkl.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gjdgtmlmx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/grrwdeeuu.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gsqnyepzk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gckloeeeo.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gmlplrgmh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gylzljwbj.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gdmwqxulo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gdekzlmat.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gabtdptva.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gibsledlo.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gyndoyudu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gddxmrnct.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gthtgwmif.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gbljirxcr.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gpcstxhes.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gdxjgpecq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gxgwxklrj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gtjbjgnza.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gytgmqqak.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gvkcbndcr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gumvwefzv.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gdquljidx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/ghswpvewh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gtblczjhk.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gnnowjqak.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggsyekgge.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gykbkiqho.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gprleoqab.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gxtiubsmm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/globgjvpp.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gjvueeijk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/grhzxwwwj.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/ganfiknmi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gwvfrgmok.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/glhbhnzgx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gbviqxrbx.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gkumpvler.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gabtxolao.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/grizqnnub.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/ghnomunjb.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gztijongw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gkroivuhp.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/grdlwsdpv.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvsuwqnkk.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gpyezbnin.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gwvfhkiok.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gsisonsng.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzvoejnxw.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/glwryijre.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/glfnwvpah.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gzaalgazc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gtdzgiklq.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gictfewum.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjajgisvs.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/giifhcwfz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/glvqmrmso.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/ggujarqlc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gxtvcizdn.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/ghndddwsn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/giyzqyfsj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gjiiyzmiw.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gjmxjpaop.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gbnyvbpnu.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gbmzyqhyz.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gsyelkqgo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/ghapmkgxt.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gtmbyenre.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gfgqfkkxi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gmwfmrwbg.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gzmklcgey.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/grlewfwbi.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gmgikxlpa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gbwumjbyi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gichuwtnk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/giptcaxri.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gxsnanjnk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gbidtspjy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gaottcapo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gdimzqnyb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gfqjbmyhm.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gcaeoeptp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gpvfwvgrj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gvcorhxtm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gpghmpbpo.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gsixpjykn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gaxbdnqjx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gqbvecype.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gtaoqgzqb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gkhcqpamt.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gtuzksvvh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gteuuxyqi.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gsyzwubyt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gdwmqvkad.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gdpoeeqvd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gjeaqzdbo.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/ggdydbnuz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gsyuelbxl.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/grklkyytq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/glxgvvnxp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gighlvgye.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gwmmwahnx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gikrykkkn.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gwpawudqb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gmazgljwk.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/ghcgybfgg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/glypywicw.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gquolfyvo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gfxayefvn.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/germdgbno.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gfsnneiac.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gqtdvqlae.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gndbswbrx.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gcyykqulg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/grhcnugrs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gcooulwjl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gvrvymwkc.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gztxudcxq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gshhepmty.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gzyvdjwrp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gvsszsfht.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gzdqvvxbf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gpvoosstx.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gcrehhkfe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gdhifdcim.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gqqeicuem.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/goagcxecq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gojulgyto.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gtodavthc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/geiftimkf.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gvmsecjoi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gurveujyt.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/geqvnojnf.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gbmzvogwn.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gwfjlcnjz.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gasezjdhd.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gumbaqklp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/ggiheomjv.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gkmdjuluq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gbpklpzxj.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gnphwsjoc.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gkflvwmez.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/ghslmijyc.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gsqudiazh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gzezakswc.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/glpuimnhc.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gcmrxnney.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gkqaznrmi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gtyfjyijz.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gwwetcpgi.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gbefkzlar.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gnegabyte.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gvmddedse.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gjywraxyf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/ghxkruppa.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gjxnfwpsy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gfjwcnjid.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gcmwbcvik.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gxsjkjqao.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gwthslcer.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/guupfgoqw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gsmqjxifb.sHtML


<!-- 参考信息 -->