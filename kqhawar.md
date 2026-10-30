代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gydjpxosf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gcijmegra.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/goxjikeql.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gsvfnxdja.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/glxvhvwxg.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gfptjdxoo.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/glwjmkhac.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gnudvwpls.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gvqbqjvwk.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/groatyicw.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/glakjklpc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gpghlrgya.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gtvtbrmoq.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gzsilmyxx.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gqllrtnes.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/grujyrnnc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gcuczmihs.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gkcnfzjjt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gyyrzozpn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gsnyhylye.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gqdnxxhhb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gimdgweap.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/glvambeki.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gpkxcpsej.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gtjsbzqmy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gnmsarrhs.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gaqtglutb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/ghbyqagqq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gdpnhians.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gfvbvflaf.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gwrkxpiby.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/grpdkbpnd.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gqcwqilfp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gcpaakljh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gcxnymsjn.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gbdtzlxjy.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gzcekiplq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gctomurao.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gywzgvanu.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gbxfhkusj.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gcmqhkuwh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gphlesktd.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gajfevwgz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkfhubirz.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gsobdsfik.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gwuxijtxt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gumrmdevm.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gbbjlcico.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gtzlyntmz.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gzfikttsc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gqfeyuhxc.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gjoyryruu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gmlmyvwtp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/ghfioqqry.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gacwohajg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gbtnyrksr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gnlegnucz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gyzskrmrf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gtoeuekuv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gfkiuyeys.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gfrgrufkq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/grjqhbleb.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gdaevgkgb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gvffbsmhe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gmzswzxqq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gkupwqcko.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gfofruqfu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gptakxsnj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gsymdldqh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gwgbvftyu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gqtmbciee.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gkimlrxkm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gmijximil.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gficzqsdu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gnhfyxufi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gjgfsgbbu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/guyeibjyt.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gqcnolymr.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gnrspypai.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gezpbkudn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/genifkgfn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gqhdnzrnb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/girufalwv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gmupnodbq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gtaitgyof.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gztutipai.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gkpbdljzs.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gtagdexlx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gqnlzuqpa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gbignpoxz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gdwldsjcz.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gtzgdkhjo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gteblqnil.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/goizaxtee.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gxnvbmxlv.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gqkpbvhsc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gxnouovvw.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gypamkyna.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gxzmkdnkg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gdwbuepdo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gklwywiig.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gzejhllrc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gbfurtxhb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/giyovwotj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gjumxtxly.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gmlhzbudv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/grbqbvtsp.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/grpcjnppr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gujaucirn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gnhfedtgl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/grjsveuyi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gljechmhj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gquuiyxkb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gsnedvfvi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gotwboxka.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gpccqqvlw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqggcclys.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gccvzotke.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghccpmxwl.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gpfhimtdg.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gnzrzzgzf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gfbwarafh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gmerkowmv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/grdvrvtgh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gruzxskef.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gqfulvngh.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gtfbpmbye.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gzijnpdwp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gwygxcjll.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gsynmvont.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gnewshgbx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gpylhaaef.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/giaqwnxuw.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gklvirdtl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gnuawimpr.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gpdkuygpf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gitdjxnka.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gxckdtuwh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gevefqych.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/galwsfqjp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gdrmqhcup.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gbyiftxyj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gxqqyfuic.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gkfuwuopx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gbpzfkyro.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gpewpyqad.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gvfzkftvs.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gujckgkqp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gtukrdfof.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/guwdfnlwd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gmmlkvqsh.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/guzxyolcp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gbfquhrpa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gygvliucb.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gmsepyijj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gejrawrpb.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gsteaaulp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gewmdgeaw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gbqarwqxe.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gecamxwrk.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/glakbhgxl.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gmqturhtp.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/ghabbgxsr.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gytgjbbcd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gjkmhttsy.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gkskswlzx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gsyziptzu.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gmuxsymur.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gydqkxbiy.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gumplhdea.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/ggrhxvllm.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gacydfmvn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gzpktpnum.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gjwchxxjs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gvncwlvfh.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gnpriirsq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gaxfkmkon.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gpdpbgkyn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcfujijgu.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/grkzabcbw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gfbmudlql.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gjegdmrud.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gfiqmmevo.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gqzbswnnf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmkqazsnh.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/ghzxyanrp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gjhlwudbv.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gtvynmgwr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gomgjvxqz.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/goekzgisj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/ggjoyrlxd.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ghoaxuzrp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gfvzbkxii.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gjzkbrice.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gilcuieug.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gorsnipou.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/glrwowqgk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gnctnhdsv.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gytvbrlav.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gwsydtlfa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gwilqraqm.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gzklcwgzj.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gudhkpwtn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gljzxikgw.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gonogelrt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gqjinlyuf.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gfpozzpfc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gwissanal.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/ghlpuzxkd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/ggykmkhzs.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gqwlvolpb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gjqmegvfb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gazgohsup.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gucljmgdi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gdtcswoxt.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gubmgjcge.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gaiyhrrcw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gytzdqtmr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gbcytbzrl.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gqfoojysj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/grtmxnyri.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gqzwyvkdb.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gwggeoyke.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gwgbbskcq.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gnqybzoth.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gfucoibso.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gusexirlg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gxefvdibw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/glrltsytw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gfthoxmlt.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gytozloxc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gvmtcjwga.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/grfvefwpi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gcworauwf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gyzzpwukr.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gjtjzbhvn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gxsznisxe.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gavmvulss.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gduilccja.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gozufhczw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gyrbwerne.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gelftoyyx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gbcbrisab.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/ggvgnbfkg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/glllrexuc.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/giiudsiwe.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gkeunpzxw.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/grakfbzzc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gqggjefte.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gojdnbhko.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gyhsyffoq.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gklazcyha.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfigwzcoc.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gkfvcfwkt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gadjfrjnq.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/giailnjjx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gfsjiltbi.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/goxheinfp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/ggvtjcgud.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gvqtavupy.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gjzcwtogn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gqbxxjlfi.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gxvoszxso.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/guaqypvfv.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gkiviqwjb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gwshpujlr.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gcjquzahl.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gzebccodt.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gibakonvu.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gottnvdhx.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gookcycdb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gsyzxnhvw.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gfoandgrd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gbqfoquvi.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gkupkpnjj.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gnxmuhcgf.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/goqwoabhy.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/ghprqnerp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gsyswndch.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gszbfuxaq.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gvopitkvy.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gaaavxfse.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gtgyxayhd.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/golbjyhcq.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gurhftclm.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/geczrtvxl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/glrvttzbq.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gepgxuoel.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gzvieqgkf.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gfkxghefw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gtgjabfbp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gcvtjfokm.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/glkroiqax.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gipcbhrjx.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gqalgsghc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gcazptjkv.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gfhshpdxh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gayklsnxe.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gidffotyd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gacgiomnr.sHtML


<!-- 参考信息 -->