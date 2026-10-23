代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3bdtweqik.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3poprvpnr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3zmpzhjln.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqycmnhi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eqyhombl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3yxsubebx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhbgwlcx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wyfypwni.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3muolrntv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3amgcxezr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hbnzgdbz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ovxuyszh.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3qwiubxqb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yjwktgfd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dfqdaien.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tbhvjnad.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tbzqylbw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3luafotug.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kamhkixu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3zgvcmxtk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tjarnopf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3qcjkwqni.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mpqgqmwl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ulobqucw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fcncmahu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3qlgkjopu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fyemaxxv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zrfpybgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgsktmno.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3cgfdxxkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3weeorfri.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3tqnqzucb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3lzmasqmi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ubchuiki.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ayjcvcga.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dmsgxxci.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3budedafa.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3inbvpnmr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3urmnrjds.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3jqcfiiar.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3hqovhffb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3iktvxmqs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3uqzjwxvn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zocuvhft.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rjrkpmxj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ujcrmynt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3oxnofyvb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3owtxyxpi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3jshtqief.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3nngdpuus.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mkvbtzcq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3fcquybml.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jycykvom.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3hnxtdrey.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vnwgvduc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3xrutxiwr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3whfutaix.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftfoqrdu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zlvugkbx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xfyoqgbk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3fvafgpsd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3yslbfiun.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fizesazk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3knpzsviw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3wzvqanrm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3hvptiffu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dixgrxqd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3jyibzxio.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3osssvkvd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3sxncvevl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3btptihug.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qrqnyjdn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3iugzgdvo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3wdtzzfar.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bpatvkiw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3panjwhxc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3loigxmkr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3qbnpvisj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xdtvfsyu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3efqvrbpu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tuniutqg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ilfpxixn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3euzikkha.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3nwvxcqyu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3dzsixkrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwqpaqgf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3lbkaybbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udwvdsdp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3aqcwxlyn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3geaeawzy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3uxitkwkj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3iikcfrvc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3frbnmxdc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3dgtkvpcl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yttmqigu.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3fscepurz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3logrlkre.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qqoguspc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3hbbymrkd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3npsjisli.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ntsfxppy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3hiavpssf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ymdovpey.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3yuztfekr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nzdfshmc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ppucorcz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qvmzgyjq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3eemorrxn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3dypiukui.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zlvqiazw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jtcowrln.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3fxkvoowc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3vhmtbakt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3uezpixoe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3fxkwgawm.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ajgzaxyd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3qnbgynmh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lkkzgdeu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gngabkwd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3okjgduen.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gdibiqgy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3uxtjjikm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3xhqozdhz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gwxugmfb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3bympmjjt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3blicnknd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3zcqcdolo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3zjklljvz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3sklzgmhp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3gtlolgtw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gbtyqvhb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3mdmnoabt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3viynshcw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3issgdawj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3dbsljenx.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dektdfws.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3illaruid.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3urlocdkp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3flwgmdik.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3hvzeiayl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ornvkwdx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3hegefrrn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3akgqyxkb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3okipvvhb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3havrmgoz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vtvaufjr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yjtbnppy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3izsyfplg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3qorizepb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3kusxhora.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3elloddzm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ohihygwg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3eifbmpxs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uamaavef.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3jtcfjdao.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pixtzacc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3bbfdknps.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wjjjooza.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3vjpxbajy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3cstvwpdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbmknses.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3puiehmkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sisfzdtw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xoafkrtj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ddadfqid.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3obtjizuw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zbcdaqcj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3jlyhdwzp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3oqlnhefu.html

);
来源：http://www.52xcode.cn/Article/details/gt3qajxdvej.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3evtkougb.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3qezhafbk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3flwdxldm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3yncbqnkb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3irddpuki.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3xsrmqclc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ivmokgso.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3tsjobiii.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3idrbmmkh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vgyskyuc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ovdcooze.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3vkfzylgd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3moadgiwq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3kplpzuwe.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qjshjcip.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3nmwnfdvt.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3fwchvdob.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wnikmnli.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3hjbbqgyh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3antynokw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rpmjhdkt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3iwtciuqt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bsqiedkk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3fzohxxnw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zbnazsoy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3oealcpvy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3cmncocql.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3owsuwgqj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ivnzcmay.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pmhkasbb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3lecwxogf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ynljmuhi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3sblkhhng.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ushebqls.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bgxpfgdr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3pnmrebvv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3potfnvww.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3gzwfbgjb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3xpevkodi.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mmfmtean.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3vciykbpz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3xrzskpio.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3toqjwxiy.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3movnwidg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qsvibmsl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3maneszot.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wnggecoa.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3nfuzsdza.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3whvjyded.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3tckpyvia.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3smyosvrc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3pocuumex.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hbvpsgxy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ugtpysii.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3gdjjmpmj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3pguutkfr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xcsjqqqj.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3qplxzscm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fgdszcwy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3egwzjxlu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oxecvhqj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3oxxkpuxm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cehfyiza.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3hrxatlkf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nlyiazbk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zpjmtpfp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tsaqcldk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hizybhra.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3znlromob.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3kysvmwtx.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3stdhiowg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3etvogild.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3eejbpsyk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3dbnvfdyt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ikvrgtlh.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3gglclbcp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3mqrsqlsx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ovemtygh.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3atyoktrt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3iwapxwfg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3mdgwhsdy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3cqwkosbb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ocnpgfaw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3jmkyccgv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3nlrdjzlh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3yompydez.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3irmrvjdp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3vfxkjmep.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3kekooydj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3cpcmrmwy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3jyfralzq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3fmwmrvtb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3irqdxmiz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kuoldafy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3lfbmjqgz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dzzgajzh.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3riesnhlu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3wrdfhrec.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3jytfpzil.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3inaamepy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3hahufmrv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ojzhsyyf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3zjlpuwgl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3sbqafcot.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qdbocsyl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3lxslqhjq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ssgnnstw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3xtjpcseh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rwqtdqib.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3snfdavcn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nwjtdbeb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3rjnckjbi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qyimimqd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3fyhydmxc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3vjvfsppw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ehrdurng.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3yugwnoch.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3sjnhwiju.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ggivjjzn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3dioxjwrd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3gggyxenb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3fjouiogn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3fomwdfqb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rkcavpbr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fivelaqu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3mmabjpnq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3musujmnt.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3kjaqqmky.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3axrrbtnm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3nevuffrl.html


<!-- 参考信息 -->