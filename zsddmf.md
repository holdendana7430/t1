代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ibrgewrx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2jfbakesa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2wqpeoddk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2humhwwkd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nbpmflxy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ndrtwday.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2fjfxfasz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2gmfvslew.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fuyeivct.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvllqgbt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zxsusnkg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2pulsgvnu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2jzcyovdt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2soehhvbz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dturrrjp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2akovotgv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ouffsgzc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2sdnhfpni.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cyuguwun.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2itrpttao.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2zbqbaiip.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2okuoavbw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tofaychi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ugiijeyh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ntztzbjq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ofyxkffg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2yqncryne.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mcwpuezg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tuzircty.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2fpcynwig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvuodwce.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2cbvaallm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2uclxwqrn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mnkbjtfz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2usoytwip.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2omtgfugp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ozhmjupi.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2cmknlyoo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2unimmzer.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ucwkslla.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2rnslnwwj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2blvasfjq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2rtzdtboc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2oecprxlk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2kykgagqb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2brprnnzy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2soyodvfa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2kiokpukj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2jxaksexw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2wseofjof.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ftusntmt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2wumdvagw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2fxjyuieb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fhaeinen.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kvyvbydw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2wotixxdz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xitieqpe.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqqrieuy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2tgujunss.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vzvnfdsq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2axckqhuv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewjswacc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tqiwycic.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ijremktw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2igbasqdm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2masjquwl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2zecylrgh.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2gdlhlqum.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fqvlidts.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2uemzragh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2arkmakry.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lmzqyqkx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2slrnsnak.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2veyuoocq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fyykpijy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2nswuqxgi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2wfxmobhw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ralqgzpn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ezixftvu.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xnnzlzxb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2yejkxxlr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2isktseby.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2rnrqrhoz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2vluukwkm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2gmiyuasl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vapvyxgf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2vxujfham.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fflkjpzz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2lkccghqg.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ffihbxsb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gvggfeef.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tatuywxf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ubbxjout.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fxbggyjf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2alxmkpxz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2msakdful.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2eaczpkty.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2fyggrucx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2rabjqguo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sfnoubei.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fmnkygqe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2hfslyscj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kgfmdmps.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2uwmacjrl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oqcqwmfl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ycgdtbjs.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2lvrxhgtl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2fcxbwxmo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fuaqpgha.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fdzwtaql.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uwzvmdop.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2asisykzb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2bwwvuogl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qpcpsfiy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2mkebjwmb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2efuogpxk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2dhxvpcjg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ewqydtoq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lartxdwy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2khfgillg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jjuyxdfa.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jaicmtcq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2zytqxvhy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jmjdadqp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2iweaciqq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2nvazhsvr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2anupwcqm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2zjlnuxve.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2peklifyu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2hilwkbpa.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gawvkemn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ncvwpgyj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2fbrmpttj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2bjrcjqge.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2cklyhjde.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlwvdelv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2agqllsvc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uspzyeed.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uteqsgye.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2dgnqrstq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2mmwgamfd.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lflyszoj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2jhyyjsrm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2wbkrhbfj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2hfyuijkk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jdrrhfew.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2prvppeqk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkwpbjss.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2qdqhvzjc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lxnqxotl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2tqrkzdzs.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2fvtafvjk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ptxkpnzb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hpxtqjzq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tmhaybqd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2svdjnukn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2nmrtoxlv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2zhfjvdnn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2lhpobmfn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2gspfmmix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrqehdmq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ohalwlna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npwbkyqa.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2lheswcpq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2lahokcjz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nnmdcwdp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vfsrrleo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ahzylens.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wndtbonf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2uktzatag.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2lzyivugv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ifnpdnyb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2imbrlnrg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gndhokba.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2opypwnkv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2tzjrkrmx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2lxnqiryf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2lumpptho.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2lilytxva.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2oswnipbc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gdhncfgx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2yfyhfpos.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2itewrjbx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2mjtlgntv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2yohhhklm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2rsucqdxj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ktvvmbtq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2hejpxtas.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ctvuhrsb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2drlwtkhz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hojypbos.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2rvleboie.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jvvfmusd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2abilqfrw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2poiwclcg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2vthphpen.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2iawsggwz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2clsrmawg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2koavnsfd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uoadiljn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2inszbmjj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2rrumtdtv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2rvunxylu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ynmcasyu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rrovquhj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lkntemed.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mjgncloa.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2chnvsiue.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2eyunwgnv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2sswoggoh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2bngdibxn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ctsayxei.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zmvgglet.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lrkirurf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2xyskzfyn.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2yttuhmjw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cjdefpwl.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ennslseu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2hxljaswc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2cqmudjof.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2yjwodosm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lsddcarp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tbhfnyya.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2iglolnwy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ukiavyls.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2yjaphekz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lsafytfx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2mdrqmmhd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fqtlzpma.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2efitahbf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cyxmwyti.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nxkuzvjx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2payvrtwh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2tkfgpmzi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rvkoqiqy.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2aeweuakr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2sidufttv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tiswvyvw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2erspuzgx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2kvkjtcmu.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2shpwiord.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vcenorng.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2dznkydhr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2fykyssfn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ddkelytt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ymwmtegc.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2cuycwugp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hoyrrhht.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2igmwlrmv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kabgbnzw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2kwtbtkla.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tgmcxpsl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2eofadlyr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2jmuyadut.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qknkfuva.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2nzjonfdr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2tytipbut.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2jebrftyq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2rhzgcqip.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ilfuzmar.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2okhhnwyu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2yumucqnx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2nlxrjdex.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2qguhchqk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qagsfxhy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ictnzvzb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2nazfikbb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2hlnsqcja.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wbgijmoi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2sqjlbbzf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2hjlratsm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kaevidnl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2veslhmxp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nvytrsps.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2nzqeyeig.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2drrpymxo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2rnoozglf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2rrbbkaxg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vfisueko.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2oxoykwgw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hdscvyyh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ktkzceqi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ujlcufgp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2uskrmokn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2klkpusnm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2dhzgihok.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2szjohkop.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ibmtduux.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2lmqvchdd.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ynsyaqzs.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vjohisoh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2pdmugnos.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gqzhztjb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qphnwpsv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2iuxdkpsw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2higezhhi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dvzmybsq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ioqpcbvx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eihmpgig.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2pxhizaov.html


<!-- 参考信息 -->