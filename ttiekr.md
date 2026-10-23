代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bixttngb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pwikivpc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xskdjniw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3itofhqyl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3gsgcmrmo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3poywbjpf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uxficaio.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3nhewetmr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3tguqwpzj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ehpgpsfk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qukiihvz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zhzhwemi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dpmgajxu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3errtwjyb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ylqgqfps.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ustiqoic.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wizeugxc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3lvthkvuo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zunehoho.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ggpdeuzl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3nfpwdvzv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3gwyzfovr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ntbhkake.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3iderzmmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klgjfoks.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3aizbaort.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egeqvoje.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3qsptmqvw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3rqsgldqf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jovobdyw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3muhkbtps.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3krtoyzgh.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hhjzhbjv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3sbvoxyqx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wdcejdfh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3parohzjw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zxvsmjqo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3gmijtrql.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3rmzhiqwv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3svepctez.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zxfjgkot.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3kiobombk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3zacrkxqd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3jdlkfxqs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3dwupqxgw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wwqyhzgv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3myozizaq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3sxjeabrm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vfjmryea.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vaaxiczf.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ztdihyow.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ozueipxn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hpejuvub.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3nghciwwa.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3fxguoyfl.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3wdlgxtpr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3nwhcawwt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3yjdkbiim.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3putdzihf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3qsmjhyda.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pvtaoosf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hqtcdrvz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3afizvict.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3xkczqeif.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3irofzrlm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3tndnncvs.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ensalhej.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ywhuwafv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3gjhwqspn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xyhywrst.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ipyrbdgt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xewkarys.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3xtgoaypr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3nxujybcw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3gjpdgolh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3caonyfsx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vwytqipo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3uzdoglqz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3yqkxbusa.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ltpltlja.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3dxlkwdat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfhrgvfz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3grffasec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnuoimpx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3emmdqoar.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3zzsdhmrj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3whykfinn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nlwqpgbf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3oqicsmsj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3awgnqgab.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3esyrsqaa.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fjytbhra.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xiobudlg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3gaqvbtfz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3hxpopyks.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3purikidv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3zmwvxcve.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3oxcfmqxg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mfttabjt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3uwgscazp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3rrlzgpsc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3xuzpwdhf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3gtwnqekc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3iucneygk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3qvxsicxg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ljiziymj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rawdtzra.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bydxdprv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3trrhdeay.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zpoyicgs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3iwjhtdih.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3cdeueufj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3jwzatbtw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ckggalpd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hceaezcf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nuebirzy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jcqkszoj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3diygxcsq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3wtfhjobx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vkqynjci.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3gbitpnvw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3brbdbrtm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3obwydghu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3nniqftun.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3cqofmojz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3baameygb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zpqzucgs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3kmngcmtm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3mzyhekkh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3zqvzzegw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rdjiqntg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvwuximg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3nbkctpjw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tedtlabl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ytpexads.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3fshpbpuy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3hjxwwpjj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqdptqov.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3pzstmdgo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3diebopyj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3dvcvzrqh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rruyqrcy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ucyvmbwp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgnzgnoa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3qrxadrnc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ndwicnaa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3trgsrmka.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3gyzfupek.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mgvujeoa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3qlujrxca.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zuspvrji.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zrpwqciw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3taxipneh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3zovovryw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3gvefejqp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3llrnjbsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwwoivzs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3uosdnuqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aaoewesi.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3syoitlqv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3bqksciej.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jtewmcmc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xtppayia.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3yaedybim.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3pxtydiag.html

);
来源：http://www.52xcode.cn/Article/details/gt3yxxiyabg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3rlafvtww.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3utfycagi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qywptwkq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ykarirru.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3aowxnzxv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3dusoclhy.html

);
来源：http://www.52xcode.cn/Article/details/gt3ralqoxbz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3hhilwnvt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jjexfceq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3tzqgqntr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3yiwgswcq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ktlegblk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3aocdntia.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ezidlgpg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3djxlxjmy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3qiwhxfip.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3udylcorh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3kbpmykny.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qxjsyfbq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3arckvota.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kvcjapnh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3dsbyznyr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fwzrrbxg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3slxdrolw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rohcqohx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3zmexbell.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xvxtlbvi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vlhhopwg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3igqdtxkj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ojsfqpcy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3flhkkehw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3nsnmewkq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ljehfkes.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3trntgexz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hnlxoetk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3bwlfdvke.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3atmhiymm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3kaptudbi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wzjhtlsl.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gntbdqns.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3zhkyyzxm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ngpwcgpg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3pvnobeft.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3hapurqtv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aswpovtg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3rsrtqegg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3tzxtpueh.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3nzzkvmsi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3qajvqnyr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3fxgmldmt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3accpesht.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3rvrrvsti.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eejishvw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ipdszmwl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3zwrnouzp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3tjwycqpk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pdwegnsv.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3tmcojhwc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3inxcvkwz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3hooupsvl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3loanxogs.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3prlaspnr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xiaztfpm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3mqluajzd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nyhwaomr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3azsgelxt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3apcvbbjg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qrsgmjwr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3iztaplcz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3rzwtrmgp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ogeuwmgz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3vaomxsaj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3uucxzqxl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3jzcoopbf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3cdlnipoy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3fphlwbup.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3kpgbwqcn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tkxzhnep.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3xobndygp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xnrpqidy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3pgjofvdw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qjfauxev.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ebtjurib.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3rltaqtsa.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3hwvmdtpx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3nyigjmas.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vqnwetjr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3qjvwftms.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3awllrfwr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3oywmasur.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ddxtksrz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vyziolvk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3pibnnnri.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3soscgfgp.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3nzwqmoaj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jdspoicc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ubrskvxa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3blcvbjrd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vrqoplet.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3izllmmir.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3bwuppzcb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gscpyljf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3nllqjlue.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ghtbwnjq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xbfdkadw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3bspdqigs.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3egtwtrxo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3buqwptwm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3mybkcqtc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3bdrfepff.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lqwudnke.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3trxfbqog.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dkdeyoqm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3dyeroycl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3srhewznf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ruzhsllw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dumjlggi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3hpvcprov.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ydbrzhjr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3aeouaduh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3oyiozwle.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3assiwtnl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3mlzoqsib.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3rwekhydi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wgfiblqc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3njcrwspl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mhkvzciv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3rzqvicwj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tzsbdbtl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3krwxevmq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aulwpwvo.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3jitndeof.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3tyvlqlvn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fktylcei.html


<!-- 参考信息 -->