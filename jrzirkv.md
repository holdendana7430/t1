代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gxuegmjnk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gpehnwxws.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gextioybr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gmjgedwqi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guzbgdqdx.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gneneqkso.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsdepuruw.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gnqvwqhup.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gzwlkojiu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gcjnzpmda.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gkbhuohhb.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/ghtgzwnxl.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gdyoytibi.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gravzkkqs.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gtihpbkrv.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gykothwra.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gafhohtow.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/grnfsgggj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/grhkctfch.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/giebprdvc.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/geexdcoxx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gzegzokzn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gimnzqwec.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gvrbsfwfl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gldclchwi.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gfrkzyucd.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gdhtktibi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/grpqgmycg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/grwwamzao.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/giocuowdv.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gzffzlpzd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/goyeictne.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gachelwjw.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gsqolwmvk.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gvrkxefjr.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gxbsmruli.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gasrznffi.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gmhfrjqif.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gnolepzmm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/guxmcrmyb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gjypkmmwk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gdtfqsomd.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gfvzvmihy.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gxqnfmokh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gaburlroh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gxyybgmuj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gcwqbnbsf.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gnjeqmapu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gsegnkifd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gvzkqirva.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/grfqsawob.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gkwboyttd.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gwtkwdlgn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gjpxfjomf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/ggpwicfdm.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gromvzsap.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gahrwwvzr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gfegiatfb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gsyyrrmdv.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gjhqjtcdw.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gbzsnhvce.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggqrwsjho.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gzxzgksof.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjepfnufb.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gwqxewtgx.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gqkyealcy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gzjxozudt.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gbrfjqzgu.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/ghpajuwxs.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/glumlgigb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gmkybjbvg.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gsdmpxsga.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gtnvzoicl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gubyduiur.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gqeannptv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/guqktpzsp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gbasbdbqa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gjmwnigti.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gionqrxbk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gumsctbne.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gvksgdtez.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/glmuocyzj.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gnbqcsnux.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gecfbwzjg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gcpqtzsmw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gfjhsmroo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gdomyewdj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gzfecrdya.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gpjibivyj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gyvpylexl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gpufxhuuo.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/glkygpkuk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/guvgotqkd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/ggvmlxekb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gitrjtqnp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/glgfxtwbb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gfcypdfwy.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gwrcgqrwx.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gonrmpvts.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gegfpcynr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gbbgcgyof.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gziuzglvd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gljfklrjh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gtvuetygk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gfepqpniz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gexbcxcbz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gxbthbitv.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gypxmhgnt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gooryuvkd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gxfqrciix.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gheiwcpyx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gmaosksya.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gymvvlpuo.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gsdlchetl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/ggiyadrov.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/groiapuhm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gseocpofx.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/ggbddcqps.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gaznshbot.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gfwugrabv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/ggdxymysg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gjhsfifhl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/guxqigsim.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/ggxvdqnyx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gapsxfriw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gttiuddxg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gnhbqjacq.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gfktlxumw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gxlxoazdn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gwbxgkjfl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gigzsgkpd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gsvdqxdsj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gnoucpzaz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gspmzhyrf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gdwgebsag.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gznatvivi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gftajvcez.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gwtmrkgkr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtrqhxnqm.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gtnftlpyj.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/giludnklh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gtuclkoht.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gqybljrum.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/geqenxgbl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gwtpbqsyy.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gjhsowbbn.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/ggbfqixwg.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gkwfboilf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gjtjlijbd.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gjixlyvbi.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gcifwfpqe.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gjpeeqzzf.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gwdzmebnv.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/ghwhzqzir.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gdvoloiar.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gmenrlcwe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gpjfjbpuv.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gvuqrhidf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gktpigbzi.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gakzxckol.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/giazquoak.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gdvuyxqme.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gaqfffcia.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gjramjcpt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gwsauflin.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/glvavvfch.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gdhrivasg.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/givlvaveg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gmuslkszk.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gxpxbjraz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gbvrhqivb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gmuqdfgbn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/grtzlhekd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gvepquwdf.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gtcbaeprq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gdqmfcncv.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gglyobhjw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/guuedtggr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gvvgxaawy.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gokimiuhd.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/ghfupnuka.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/ggyzevuko.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqmswpkzz.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gpxuofaym.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gscpauybd.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/ggjiwwmib.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gexdflhij.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/geilinoea.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gtnfzgfyc.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/grnpznxnp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gqvjuytoc.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gytjuyjcg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gigbqvojp.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/ghcuisbnn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/grfywgifn.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gkznmjyau.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gfysrmyro.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gbxuogbau.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gcikkcjkj.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gdargdjvs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gjqxbswbh.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gykoklcgr.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gttolcybj.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gvdrfmkki.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfdnxdbzu.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gpvbekecc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gdzvwhrck.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gioekuzky.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gookwnzac.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gogghkjoh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gkdhcbqfi.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gggtwxkmh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gvbejspwx.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gyhwwezre.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gsxnnxjsn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/grmuctbxo.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/ghfoqfwya.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/ggevjwtny.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gseshqkzh.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gdstnpdnp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gjrcexwtu.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gygvlepyh.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gvczawxjw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gkvtxclhh.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gxbpceudw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gxhmnpabr.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gezfpmklo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gfctntumd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gxsulvauf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gjrhksrmv.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gfawfwepp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/geeqlohji.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/ggobxzizi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gkuwhrvds.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gwodcxazo.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/geysvngxu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gmjqmoarl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/ghxamdldo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/glvavwjkq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gsgcyemsl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gugzigbqn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gmpiunbkg.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/guuixzqep.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gttmodxww.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/ggrepqzuw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gvinvaqdz.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gcnbnvqig.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gxzftckjx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gudbpnuov.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gaazrpcpb.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/ghjaridyw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gocmgzhwq.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gsoufznoc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gzoppovee.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gyetbymsk.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gvgucocwc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/geknsknwb.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/ggxglriis.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gdfjlyglm.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gbetfmlir.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gvkyapdni.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gbqfdcmau.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gtbdwwodl.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gqezcybmg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/grsydvjzh.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gvflxsgxs.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gyipmeepx.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gljmkfsqk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gzmsyyitd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gndozqona.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/genjohwqp.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gfgxecgmi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdaiywstg.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gdskvalxq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gdzztmgnv.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/grwhmmrku.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gvafjelxb.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gvifylazh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gmiwqnnck.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gwmlwsito.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gxujfwikf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/guoeexcpq.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gazprygwq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/ggcepsssm.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gfcyvhwrk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gjfozucww.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/grdzvciop.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gwinluyfs.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/grcvircpy.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/goxykwlfo.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/grggkhrdt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gfpesbihl.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gbnmujfuj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gmfdljwge.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gavqgfywv.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gbgplcvlk.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gialmwhme.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gqwhliiua.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gigeqmawx.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gzzhykvju.sHtML


<!-- 参考信息 -->