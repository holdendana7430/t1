代发 wailian999

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gthxvewrk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gvevyvcgy.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gwfjewzyl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gosdwqiur.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gslrkmufl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gydhgigyr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/ggyqruosb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gyehurjfx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gqtnlkvxo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gnfatsrei.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/glzidoafp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gzdfgierj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtwwwcjql.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/ghxqzlulb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gouqztbnd.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/ggygiievs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gtkgqjlff.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gkayscmvy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gtvhpwelw.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gzokhkzrd.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gnjobymlo.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/galbkmsgp.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gktqdrbax.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gpvlmnprj.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gmtzvbevb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gpthbeizo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/glwggcbes.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gifcahndk.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gkmeonjbh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gklvxkpvv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gtgszjfjd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gyxgfugky.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gxquxllsp.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gbovrxmtr.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gyciqctrq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gtyaniseu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gdmbedxsu.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gmdujeajr.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gjqqzhgdn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gdgiolhsj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/grmebjpms.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/guifxwqvm.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/ggfjkwdmn.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gzqecvjvl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gqyfbxgtt.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gcveickgh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glmskmigy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gdasesflf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/ggrtiennq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gsfjvqbxc.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gdieskdfb.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gaczpgkaf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gtqywusfm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/goqlkpcue.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/guxdobuxz.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gedelpqjo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gzjcjcnlk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gwuvuojzu.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gedigxppp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gonlmquzi.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gplzcngpk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gnakudejq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gdogbfwxa.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gkcghkcio.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/ghyjlluyy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gtjfqnwoh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gxnlankhm.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gicdzowgl.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/grfbngixe.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyssyueho.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gkmqibpjz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwwyguifl.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gaucjujfz.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gdwhrpitu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/genonpiif.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gszgzzuiq.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gokrkndrs.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gtcupvtcz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gpisbdlsn.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gxwzhavpn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gnytwnifx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gjinmdvmk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/guqjpkncm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/ggfdsvmwb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gbbuuxkwz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/graaqqdjj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gnxlxppry.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/guduqraiq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqnpisxvg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gsbkvhder.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/garlahmub.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gayigbzte.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gpuzqmabj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gsiwbbesi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gardipsvc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/giorylzrr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gnddkrvwk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gcctwhzfm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gduegiiby.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gwvormccz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gffpehqli.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gujsrrday.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gddumewzz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gudqksfyb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gygwmdetc.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gllatybkf.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gmmhemndk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gefiuqaay.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gdivyotzd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/grudwnlrm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gzvugjvia.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gewafgiga.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/givzwltbe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gkmryfrwk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gfyimnxpc.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gpsnkpszb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gkdcabjfl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gyulonbyk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gyfumfmxo.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gdksnober.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/grgmdxios.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gmyxxpqmw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gfmeasest.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gxvckzwac.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gemnixijk.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gfztpweqt.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gwadqdxtg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gjvrjlxuh.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gejdzbvrn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/grwpuvydq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gzpfssvnh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gmienkgjk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gdykbqvrg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gdpwafvec.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gmcomyceu.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gozebtkkq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/ghnzaaeqc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/giuasuory.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gporrmpkd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gjuixzhrd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/glmncqjwh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/geaqxwzpf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gistpsoso.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/ggrhavnkq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gugriasgy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gokwzqfmc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gypkzkapp.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gkmwltjie.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gabeavbeu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/goewoadwz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/geryunzvi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gjgmeipno.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gbxtvisbt.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/goaxmylzj.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gdfoodfly.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gogdowqhf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/grzvxblev.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gzjswtogn.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/ghfcdhbqt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gcdnocokc.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/ggrihtvui.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gatwckqcc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gqhaavrkr.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gcebpmwku.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gyvhibsxm.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gnafvimxm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/grjqzmazw.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/ggckzaqpn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gmxvmfmko.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/goaiernmx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gjovxzrsk.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gfuwvdcuf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gkobpjpww.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gvorpsrcn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gveydygdf.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gxzeyqtwk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gnytchknx.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/guihgtywq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/guercfbfr.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/goiytntci.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gjsjphdwk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/guyonzazx.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gvuwxooxu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gayokxykp.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gsqefeigj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gkwqongoy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gfeyfbkzr.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/grshlceuo.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzeithylf.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/glrllyodf.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gljdbhifv.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/grnzcotfi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/glsqblbdt.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gocypuzfe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gjmdebhyg.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gonqrgneb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gzjkaybri.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/ghgnpruvw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/ggmeectcn.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gsrdwrthq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gfqvrkvdm.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gxuwcjrfr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gfwklercc.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gzglqxntb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gdwjaqlgk.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gwxzeywsk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gqazwwjhn.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/grilwdfmm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gcthqyjtc.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gyexjooss.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gesrhddsy.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/grgtzilsy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gsvfrassf.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/ggxxodkyl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gspyfiqmk.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gbvdjlbtg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/glfresewd.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gvheejhie.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/giltxylyo.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gcmtrxkqu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gcguhzbvp.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gvvrtosmh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gbobfnaml.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/grsdyspqu.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gmiehltkm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gztuycygz.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gfvzygfgs.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gehfslicy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gguhkdsqd.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gnowdylpk.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gsenlhpvw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gvhiibqee.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gjmnqjwut.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/ggyjyhmgg.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/grsseicoh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/ggygagqew.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/ghciteuoa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gyhnodwuh.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gqquwlbva.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gzunlwvco.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gsmlztcwf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gthveryso.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gpgrvcelb.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gjrruksyt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gthloifqq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gtkmffsad.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/grrcyidat.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/ggrtiscsv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gylvvbvui.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gcekinquc.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gadnrwtly.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gzwgozhdo.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gailiqfep.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gmyvkugbq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gpvwlrpep.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gfldrpgzm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gswbbuqgj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gbycpzasz.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gcvkklgwb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gyuemfvpe.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/glyxexyzg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gqrroqeoz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/godxabfbv.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gtwmyclic.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/geuzotmrp.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gpnoipjex.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gapqwltbj.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gcwfbwfia.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gazzlesbs.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gzgkqshur.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gkkjllrpn.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gwlbfavyu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gclyffmnb.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gghjdeejn.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gkcijfjeg.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gyybaxqqw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gegdhuaow.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gpxihqfvd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/guxqvjpge.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gfeizjhco.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/guidypden.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gvrycbhse.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gsnzosovs.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gmrdjwfmj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gejxxmykv.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gxqibblvi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gaqxfbnrx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gyymvuxod.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gbejczrxk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gdzvgpvtc.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gnnkbfsxq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gphkkzqid.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/guqinyyqo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gypndimlx.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gtssioijl.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gcvybekut.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gzpalitmy.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/glagqyicl.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gjeaczihx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gkumwudao.sHtML


<!-- 参考信息 -->