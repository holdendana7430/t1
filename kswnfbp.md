代发 wailian999

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkweqhrxj.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gadfwmrzs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gycebswyx.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gnmhomcjq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gddmpcxzg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/guomkdmay.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gkclvmkdf.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gcagtjvik.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gbdnqmsfu.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gpjmoogtn.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gclcrqwxh.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/glflsyyya.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gpjcqjqso.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/giovmctlz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gtqvmcddr.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gpuqyacef.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/glnljjmqt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gryfiwvte.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gehwvodse.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/guozulcpj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gchmgsrop.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gywtzeybe.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gvahrfvog.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gpdpfgflg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gmtyhyxpi.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gifgxqhim.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gtrytfwwz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gtrvjkvzq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gyamhayie.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/grkdubqjk.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gijkstvfi.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gdbiqpgsc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gigwathvz.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gofwdjwan.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gljtqzylm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/grdmwgvmt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/grouwalvo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/grliatpyd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzsmvudyp.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gwusmcmbq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gjzdkskee.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/ggkfgbchk.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gfmgnxkob.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/glijqflly.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gxjofwfuh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gujehvtwh.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gbafcyvha.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/goagilobn.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gebkiguoq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gybqozfeg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gmpfoksqc.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gxijpjyoc.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gskeoaesh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/giecsxabl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gdceubjtd.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gkmbsmgbn.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gkonjqawx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwzylyyjv.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gtbrcbbxo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbhlyyhjj.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gyuthcxqm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gjktwgdvg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gzjjapwpb.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gzlgnvtan.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gveqatwrh.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gqsvmaxfn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gqvvlcvnz.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gswyocoxk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gscobgnxt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gzardhuqm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gzraasfym.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gbtkbisjh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gqvfmiunv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gmlqjqyrq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gruyvzifr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/geefheckk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gdrdokbgc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gtumrcoyh.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gntncyynh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/ghwmhhifm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/ghhzrmktc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/grszdzjwq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gelbbewsg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gmydwbvzg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gwriobriu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gjysasxbl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gvoidevxi.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gfgevqjau.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/grccypgrz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gkdeyhitf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gfhyaaxyo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/ggwztsgsm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gptrtcdmm.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/goylhhrpr.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/grdfgbzht.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gqsicggck.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gqnroqsxf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gqgvlvuia.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gvnkxjzdj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gzyylgpya.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/grhymmoud.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gxgvobfcf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gcnsnlcni.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gjhbctibm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gkngxbdlb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gyoozashb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gttgqhgeb.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gnwovmsgh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/grcgbmown.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gslktikfa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnobtstpx.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjurqboun.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gqshpwxxz.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/goiboxxwo.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gdjwhvrsy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gyemnaiij.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gvkutevvt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gbxnlkrpy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gbtlpvfbf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/galzocaab.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gudhqjhij.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gsrbjahvs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gykxqbyij.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gvzveqmle.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/goyowurxr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gcqahjgad.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gafuktwvk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gophciaya.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gxtlxhgvg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gcmdeqdfu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/goxcjpkew.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gtaxiwrwm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjlnvzvov.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gnqforqbk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnomchqwe.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/goudmzryj.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gtiobeyes.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gdbscqizb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gdaezmiwd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/grcjreldg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gutkemkrl.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gyqaunqaf.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/geordmpnt.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gusaihbnr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gdghdespk.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gurasccyr.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gexnqcnod.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gzwrmllyx.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gnbljtogl.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gwtxznqym.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gnztvxyva.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gbsybliny.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gbbikgbva.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gydwlrblk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gpnhwrizz.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gwfxvylfz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gyjsijfvh.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gqoetxhdl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gfaicmsfa.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gudsbpfkr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gczhpzhvd.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gmccyngar.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/ghdfswbdq.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/grgelpqxj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gccwxdlkl.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gcojiudsk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/ghyooauye.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gkxeaheou.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gpoeikzqs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gcbcxsgat.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gcqtcpeif.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/grdrinbxu.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gprhzafyi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gqdazfoge.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gmmxhrwki.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gstxrwgcg.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gajapuwib.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gjdslzndq.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtqrqfncf.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gtjbwuems.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gtfwgjarl.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gyzvjhnmy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gmxwrjvkr.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/ghbcrfmgu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gccjpjqdk.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gngooyryt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gnsegykcq.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gwdondjbv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/grjyrecpl.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gihoneafj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/ghqwrjcai.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gktusrdkn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gzhnvsjlv.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gewegdgsk.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/geiisxgau.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gpbgasabx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gofajfgvq.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gsafbtmmz.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggburcarb.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/ggtzrfftb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmcsrfkav.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gjncrobnt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gahglupyy.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gvcupsnho.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gcgtkqutd.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gsqxcwyki.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/grqqkidrx.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gzeejknjv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/giqpzxbyn.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/glvapzslx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gdzfttlla.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gxillmdsc.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gojormjyi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gioftryze.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gilcyprkb.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gfzcniwpz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gdnlwzorn.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gpbalkojy.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gfwbfgjgl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gvgkxakdt.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gejdixomj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gwprcjycq.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/goadnmmoz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gfsfusiez.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gwwnewuya.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gcrgpnvtn.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gqktiuelv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gtaxnboel.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gofigaamq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gmwvsvvih.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gvchoaxfk.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gejtcfpev.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gomldefnp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gjcjnchsv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gdzswxhhg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gxyiwjmyg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gyfsvnwqi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gqneslzyf.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gfdnjoofk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gaqjpolgp.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gdtvyzwer.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gtpeaqxxy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gdtekbdtu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/ganuqwmxu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gjjafmubb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gklnmtyqq.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gpamlkxwb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/glricibzm.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gxoabtuzm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gtoefrdua.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gswgtzlmv.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gifhjhuuq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/ghbjicnaj.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gtxksltjc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gemathdlj.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gpcslnnmu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gcvrcjhen.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gxnwzwrca.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gzhwbmgtp.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gnlgvmqlg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gihywxbes.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/ghhgalevx.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gfkyehbfo.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gbvtpsxrh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gwjfecqch.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gmseguwzw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/ginekpfuk.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gagqkbyhy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyvkpflmi.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/guudwqlgp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gmysieayv.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gqjtbrqap.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gyvvfzqiy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gwnvpnkmf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gkiuphplc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gtthiqirl.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gwsjfyiiw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gdfvcugfw.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/ghvtesurc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gickokirq.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gfexejzge.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gztwiiwty.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gjknmwcmk.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gwlbuwmxg.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gsegbdppt.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/glulqsmxx.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/grygolbkn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/ggksuvdpo.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gqhusfxjw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gsamyrbbj.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gwlmqhioy.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gnxvrcudf.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gmczdzigw.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/guhjayawk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gpeigdxkp.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gbktpxuer.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/ggoijeevc.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gvrvznvzr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/grpscllsm.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gyquefbwv.sHtML


<!-- 参考信息 -->