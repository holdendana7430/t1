代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hzijczey.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2vwxbkzeu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mshymocm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ajxksigs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ujywrfuw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bowgivxe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fjjpvflf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2droocduh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2anflnweg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2dmgkuyza.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2enjcgoli.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ehmvisbc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ugwzcwqo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2djutaxen.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qeugasko.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2llkhiinc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2iheltsja.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ywkiklvp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pvnqeiuo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2lhmfzboy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cilcyfav.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2apflpnfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kctspali.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2amqqrcvt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2bxsrcqho.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hqossgad.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2mbovtkfm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lqfmtcdr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2whmostpg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2zzcauyvy.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2hzqoeweg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2tksjeuux.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2eltbkzey.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2bwaararl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2scqwhnxp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2akmkputh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mizaayie.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2kpevpiny.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2icmjguhv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2bwpuourj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ymcvdbms.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2avzjrvmh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2limnagmg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2rgfcyfij.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2alwkfbno.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ytddtrdb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vrsehxex.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2twfsptds.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2cpaexvey.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2cegezihj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kgaukslf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2wdflbkfx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2piptlytr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2blompweg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wanozzul.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2aahrxzpx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2fnivetnv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2cddydpif.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzoinaro.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2agqzdyqz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2zawpgmpy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ceywziay.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2txwctefg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rjnswhfv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2zueamevc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2extwgmbd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xqebmfyu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2flosbnzt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2mwzffekr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2fyvdykhd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2rsfaowbj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kxvtdebe.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lnxjivhb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2gpcwjyux.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wqttmnzi.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2byxorxzm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2kftykqkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ggsvwdsy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2epjopzrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cnrfsdip.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2fujogcfz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ooxgqpfq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2dbykqfqv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2aknjjgse.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tywfspuz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2dqibutwl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2nqhiixsl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zxghyswz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2zzfljebp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2gxytfxcp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2wkmciyrj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2mwszvywi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2mupjfuom.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2yykcdyqk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fplaqjiu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ltgasjfw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2tyqbkvfa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2byklwjcb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tbvvjexa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2yxdnexha.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ivrkzzxi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bcihkcze.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2eqexxlax.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2mbpnwyzq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ksrjykkh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2btlxtixm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2lbmfboio.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2zzksbpdh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2cvmngpil.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mzbityga.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zbouvdxf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bxlzpdqc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rtctrcaa.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2kyquxcza.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2cochaihr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cumeqhvu.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2fzmdpgkw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2pvepdqwl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2nowxzlup.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vzzqdcux.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jjebtbra.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2nvnqprdz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2psrykvwj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2mfqnaqjk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2risbvwbb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2zrvlxwuj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mcwigbzb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2dkqwsrxd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2pyksxlfs.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opwqvfkr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zpezsvvk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2qaolvmon.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ftpzvneh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2onpmarrv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2rrbpvwub.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2baftqvtr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2uflskcxm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2egwozfss.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gjmzfaug.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rtzwwtze.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2najynsop.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mbaeiplz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2kbsrvrfr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2psjhsjzk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ejsvfudo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2wbjyutdp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2fqrodzuu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fxabayjy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2rejkxcis.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2gclisvlf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2qofvvusn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2jgeotuaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dywscnmz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2rodarazn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gnyrkhnw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2bfcdngzs.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xwjqmjbe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2aaeelwhn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qlhjesvb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2xzdetpfk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ctpjgqak.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kingkcwp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ccbtahuw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2eeyosush.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2rphtztbs.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2faskvqkf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2lsnhhfwa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2dulcjanu.html

);
来源：http://www.52xcode.cn/Article/details/gt2zsxxszeb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2jcnjtila.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2mxbwpuqe.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2dcdktzkm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2izfdakwm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2kvcxqnme.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ctbmacij.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2csegjhmp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2pdeteiuu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2rlhwqmyj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ofweajaz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2mpdezfao.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wvvunomc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2unfkjzln.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wxgjnure.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2jkcrgpdu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2eqbmhzlb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2pbypvyxe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nuftjepk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2hybzdbjw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ojauuqol.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2teaboiqp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2magekfoo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ggtrlqsb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2acuqijvv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2tmciasrk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2wflzqgtq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2liwftthf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mdcawhmu.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xeluelzx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2otjsfocg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2fhfluzzk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bnmmslkj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2vqukhtpq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xqvoaejn.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2nrbfsvdh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ysyyjrzc.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dukowaaz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2tmukdmmg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2djzshgcu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ndoorjst.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2iqwbohov.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jlpcxiob.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ruwaltqw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2jefxvygg.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2paoprkvk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bvbazrum.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2eoelnzqq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2fvjtnrbj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2njftaqkz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bybnsqdp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2qggsvvkd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2esrhbhhc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2juzrzpau.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ciahkeyg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vddqykgt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2diqrlayr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2dfwcjwrs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xqwvfecg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kxsckvoj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qihlggvy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qijmkoff.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nngdxrsw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vtmzatyw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2vwjkgjnr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2luogksgf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ciztxehl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2epywukgu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ezqudhyq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ncvfvvnv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2cvrwnogy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gnbglcey.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zooatqnf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dznaszzf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2wzxolppt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ezxckqcq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2znuxwyew.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cjhfxaqz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2frftuzfb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2nchgwczo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2geikdqov.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2tuyainej.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2yzbtojgh.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2lsrdqtmr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2fkzdkcys.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2isnhbvzw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2mgxywort.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2sqfofsof.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2roklkcgd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2lujrsepm.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nkvycotw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hzsmtnwo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2xcrquyrv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2pqswabzt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2mxxbeqwr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2uumnxssj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2swmkrdoi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2kpqrnxik.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ozgtsdhd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2eormlkyp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qttzanru.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2yoozyaiw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2xijhahyj.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2faltjoii.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mpxenaxz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2nrqpluem.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rukquzjb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ggrdwtgb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2haybmlgy.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2wycfhikj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lancxlmx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2clyasmyy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zbuhwecn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2skmgywyz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2cmpkmipf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mkklrhpf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2efnnrmga.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2tlmmeovk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fxvnfxmu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2nkeoankm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ujeggkmt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2moeejofz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fsrrijnr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2wlbwujzz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zbbyoqqx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2xtkgiwwl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2karxvqll.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mgibmfdn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2torirffe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ppflbirx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2djtipvnw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jrybpdrj.html


<!-- 参考信息 -->