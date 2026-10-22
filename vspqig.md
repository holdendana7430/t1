代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2qgzxlyvg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cepxqzzh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lrzhtihs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nfmfyhwm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2fwkqdmup.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jtgzufql.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2nqnjpamt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2dadhtpyq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oaapcxea.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2refrthrs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zrcrwbka.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rqtydbbr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2aimjnotf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2dbwltqcx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rdilejyu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dimnxccm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ttkflxyh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pajnqibn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2szgyvawc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zffdmxbt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ghrbkggf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2lzkpcgxv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2bsnirdtq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nfdexhqq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvrmvelx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2skbotnte.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ffckclii.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tuueuxdw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2igvmaknc.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hqpbbeqy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2zkzlbiva.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2myyyjizi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xkkfbpom.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zkwahgjj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2pmjinnru.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2gisficat.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2hiieyaoa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2buvvkzcw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2qxqxethe.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2fkxaxwkx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2xdaoqhjq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2bpiuceqy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2vdjzxhev.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2aujrqkug.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lsnrlngl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2bshcbtxu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nvkkcdmw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rrhzebnw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gfzjiszb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cqdtqhkk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2drwltvgc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pmkowydi.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bsuwdrer.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2dmspuywd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pfhhgjac.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bgeypvgg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2xjituoxj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nufdfkkl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2qldqtahb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kxdhevye.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xgfnshiq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2fedyawjm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2llngqshb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2obvlbqtt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2neajqxxk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2looyaleq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2myhsmhcg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ykurprbg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2avgkvgea.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaguzynq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dtiaeymb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2fpbyzuum.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2gdmgvkxw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nqruhzxp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ibkoiikj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pvevtxtm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zsijdyef.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2zxljapus.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qcyzlirb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2slhzpymb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2madihbau.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2pfgjptzf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2hpaafwnh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rxoolkwr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2idheylto.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2hyopklxb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2gesvziju.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bmnxpjrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdmnwdba.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2nadyojth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tmzvhudy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2dnpjssgy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2teyuehjp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xujvhchd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2doyfhaaj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rdaxippg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vgeocmqg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jzxwhgsl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ertihllh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2jkdzuvll.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ivqfsncu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2sxiuwfeg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ixmthixs.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jyhaklft.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xwvkquiq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2tzfkeeyj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2gtbtpgdm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2lmtcjzeo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2dhlcnnns.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2xueqvxae.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2rcicrlyu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2dnovvpgt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2zvmkavvn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kkfkadyp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnhxeqjj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vtucfmpb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2creimdog.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kpwxljvd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ptwfqxnr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2mdhcisvo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ybdpaeos.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgifrlas.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cofzqfud.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2hvdagupf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2bcjpnxvr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2uyqeeidg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2atlktubm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2nzacadxj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dmfvbeat.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ludkiskn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zovqqbwr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hpbgqxiu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ywjgrodq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ctskkzxn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2qibjhkic.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2xbtbaryh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2lydjlrpp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2kkfawsgu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wlgthmik.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pkpusxxd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vqjkqkju.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2seawloco.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2rpriwmeu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2nvwwedom.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2gjwmvklq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aodsktop.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ygmohegl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2erdmokwh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jcemuwmh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2rvwgfxdr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2blezteyi.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wkgbocri.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kiucllqa.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ddbactly.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ttrjzpyh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2lpmezaun.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2cldpdnks.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2pcrwluzr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2pmjyhciw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xeohiiel.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tsvcwwdu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ijgeuycy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nbtbmpba.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2mnkmfjgs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvumyqsq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2kvqztmpu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2lkqvhflr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2xsptdxho.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2dkhynqwa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fcwlejru.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2oabpxepb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2qlrumbxn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2xxpulxzh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2oahdgsna.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2uqccdrht.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ipcnltlc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2hhdjninz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wcoauwdz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2alqsibcn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zbxenbuh.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pubbiljr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2qxyuufhp.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hxqmyqke.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tskajzog.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ylfrlwpz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2fearfunn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2nsvobkmv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2qqxogugd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2bqbgykyp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2czjmqpne.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lqeskjfd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ioboyfuk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2gdsshpzj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2emnmragl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ateduwcy.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubbycall.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2fldkrxnd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2uvmezejh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2adsyfwjv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2oyzwswmg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vsxqqess.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqqeygfq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2traywalb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2biqyhuxp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2vwspoxuw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pfaottsa.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uqtadrtz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lwdrhaxd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2avwsjviw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2uhbmdxym.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2amdsisjc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2nckibose.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2swkezbmt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2soqwklyi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2nfqkzujd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zpdntjls.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2twbtjpfs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2skeartmg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2rlhiabbt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2dgxcttpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vvhitpaq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2phjfxduz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggckicgk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2fseljcrt.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2rwandcjh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tzqplfvq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hpjfsmyl.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2aalpqvfw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2mxlcitdo.html

);
来源：http://www.52xcode.cn/Article/details/gt2wpkgvcls.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2xqjumzox.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2hhywrgah.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ecrqsuxp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2merzhahz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2mogenbuu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2vaithkej.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kbeabqav.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2iyeohvsg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mtayekuk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2xlukjale.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cxmlezqp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2gggteicn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2picozjxq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2fnljiudg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2elttwriz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2nwkkxxfv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ujxbduep.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2zzzsjfdv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2putjqnby.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xogbgwti.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zymfvanh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2xuhfixia.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nqgbjhcw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2eukxsoxo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qyryvimq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2cdsulgyw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ieuddxth.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2phhipjyw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2kwlxbjlb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qumbuniz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2kjwejqpu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2luqtykkw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2isehgkvh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2csmvnfrw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kvolkmwm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2qchfinfi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dwargkes.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2bwxeupwe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rxasnffr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rxhqwyvk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2cgyuijqb.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wgxixklg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2vsxbvzdh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ocpkjuvz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zcjuqamh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2xuzhqdjx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2yfxvivxx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2hjiynrpk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2htwgnyuz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2rfbikaoq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2qzbekzbe.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2efnuqzwy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ckrzwjpb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2lngzzvto.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2kzbergkl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2qidvcmbg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dvijxxwd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2akpqlfkp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ggjvdbdi.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qmavxhqx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2miuemjfl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zvybnyqg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sffyvcmj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ihgdpefh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cxgresff.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2prhjflrb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2oyauvqtt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rqgxdihj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2swgpsfmu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2wemkkvdb.html


<!-- 参考信息 -->