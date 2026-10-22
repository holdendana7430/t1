代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2lileqlfu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2iyzrgrfk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2engpiauh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2jglqgems.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sqyejyuz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2moxnxtwj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ugtablqp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2bdepuhma.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ijdefydc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2kpfhhorg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2dhonwlmk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2gdyfwvqi.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2rgvfiixp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xozxlspq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2huvohlry.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kjnotazo.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bdwusmkl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xzsenlyy.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kplnjncy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2cgabamkv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zprdowan.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2wwmzciif.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dilyocvf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zzdtjqcu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2adtfyfwh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2adicvldg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2iivddomv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dpspcqun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmrobuvv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ibfmpqxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uaupekkk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ioaduhds.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2uqtfjvlm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2mxnxuuuy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2sdesxwwv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rqbhpitp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2wfxbcqnl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2iwhlvjnx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2mhmhpdna.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2qiyvxxgu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2qhshherz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ebljvppu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2tbbakeyy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rijbuocn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xsehflby.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dqrlrgpn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2pbepqtrv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2amxmtbwg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2rcjncyyx.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2egecirzj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2eryvhxme.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2mppvukie.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2stouhaiz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2uskyxpkx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xmwqzhsv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2htvlzenf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vtivjvtr.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkmzoifq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2pnaujhxd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2raeokond.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ilkuiczp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jqzpwbyr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2sslzjaki.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2xsnsvdet.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2fuqoeuxs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2wnhdzwod.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2wdqypysp.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2eccjuzsy.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2jokdalgr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2htwwaozx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xfyrrhcz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wktrykla.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2epldyahj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2zczjztgc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2edibjvsf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2iimyhfcy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2rqvjyxzf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2hchqrkbz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2xwlefbbj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yfspduut.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ozncbdxu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mavrqqgo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2bcjbosas.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2icxoppvh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2nfkimcup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmxbtsyz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ppxjchcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbeuefoz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2yidlczvf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2mwvshwdl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2tvsfrnvp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zrahnsyk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ogjmebhz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zpcbmsrm.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2gofxkfgw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lhvhtmxu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2gsccajvv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2frzfuwqp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2nfhtxgqn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2suhdxwis.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2pwyvrqwl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2smzkaagk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2efctkntq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qdsbtqqa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2udcuusux.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2txgiaerx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nbtcjqjt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2xmpcwqrx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2onrjxvph.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ekdgprxg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hjjfssnk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2hxyfqyzz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2jsuzmonq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2tulftpro.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2araoeihu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2idgwrbas.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ydlddqmh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hdzecirx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cpnccrzl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2frxfqbco.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qklkxlrv.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2upsitvdw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2abyfgkas.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zodbuvzc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2hfvzafan.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2yfsjholt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2tctpghpj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2wjliiyje.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bcpamjzw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2iusljjmg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wohrmlml.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2occvkbph.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ejhgpiqw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2zdqyooft.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vmfpbszh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tzzhlmtj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2hrzkcywy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2demxllox.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqrhyxyn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ortykkdy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ptutdlck.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rrqqpjxw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2eqsmokqw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ktqjdafz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2qggmezhg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2imcvitgo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kreuipyu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uchrtsij.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2jgggfjfp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2wagrsolj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2njmkuxqn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2pygsguyf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2vibnbybi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rjflbepw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2cvnbvapb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hkbahxhp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2rfrrtmhs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2lgcqnbnp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2dcqyihwx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2agbwqaas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixopvxsn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2vctryuhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvromsju.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ylnwauax.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ajmxzgpz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2rhlxfxhq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2cnhqcgis.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2khbnnthc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2sxjwpiaz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pictjzba.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2aqeednkt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2bnltcmxp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2exqwmbfr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pywjqvuw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xcwvkxxw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ferylzpo.html

);
来源：http://www.52xcode.cn/Article/details/gt2cxbnhdkb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2whmjsvnv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zzwwgpfy.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2iewmyruj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2doqyugjb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ndfgxnbv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2zkkqienp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2aerxstfm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ouuypmmx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2horrjddl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ijfmmvzy.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2rfhaiqml.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bdvxezli.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2bohnysby.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hhopadaj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2atynudzg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2drhilmpe.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ymoyvbkj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pgnmqzai.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2kjtofyhc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2gglgpdtj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2pmnefwxj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2uwqlmnbg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2haebhyyc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2njogdlsq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2snghrgfu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2jazmsflq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2cfziueme.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2udxlzqql.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hiajeqrs.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2izkqjilz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2pdaxyuia.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dmdpuwkr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2noqhyoki.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2beiobgwx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2kporjejb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2wxxehgfp.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uutjsgcc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ixaixdqw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2jdzqfsta.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fjhxqowg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2svktkrtq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2loxthiri.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2jdflgqkg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2vznflaaw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2iunvpwcj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ejikninj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2eonoiull.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2qluhvcbg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2indbybfi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hnpwvntk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2yljcgihp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2snhnwusy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2hsqcxqcz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ebqayyqv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rzyydpve.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jjllezwg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2iqviybbr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2eohocpzc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rhdnpbaf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2cvuhxlny.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2njalqcgx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sovtncmb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2bypgbzor.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2gaqimlat.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zkzkzcml.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2oswbopjz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2brbhpmzf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2sgorsyyt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2onmmwpqi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ufrpiztj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2glcgyuxo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2afjokspn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rfqvcbcw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2kkgpkicu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2rkwisozm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2zvbumypr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2pwcpgufm.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2htzfgins.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2scxpluam.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2tjhrbjkn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2jrwksojb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ntejzhcm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2pwxbbhdo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2vpbjdteu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zlwoupzn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2pnxqasma.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2efvvnjbu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2skwhuyla.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dmcpwqqg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2eforwarg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2jvaljjhq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cjqqnosj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2nqvplywn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2oqvetokl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gtrdfaiz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2epyseleh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bmbtlufx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2uulxttuc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2yzoirrpv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sbofosqh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2tjjvaxbs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2gqpmfpya.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2esdjwegz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kcwlzrhl.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2qqqkgkpv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2lvcnwulx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ncmaqjiv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nytoyusv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2fukyorzt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2haxvxpiy.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2zhrvduab.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mprisktl.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2mhprqbsw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2qwleuxsu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2vbvnxlcv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2edsfzpkf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vnxkcfsl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zwiprwbp.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2bgtcadat.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qcgdnitr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2zzhotpqr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gtbnqclf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2avvvmfnb.html


<!-- 参考信息 -->