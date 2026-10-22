代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2yjjggtsw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vkprdldf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jaegiimz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2feqjorkv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bohxnyyl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqsgychz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tjurqnge.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fgpqpyny.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xogkqpid.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2cxnjiyco.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dkgcmzoi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kpkrsppc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2jtlgkqlt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gbsvjhlb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2yoldrgmr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbkwasch.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2raborhev.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2rmbgshwi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2idrvaddq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2dcutfaza.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2apxaoetd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rgklhkoz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nyxcnfjh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vhbabowf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nvvwgnqa.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tgijgdby.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2kbbqyvrk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cdmxqqgv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ahpqcsdg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wmtilfmd.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2rsfdbxft.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2dhslztfp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2fuvdotjj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2olyqmoxf.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2isuezshr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2dqkuykrh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2pzvbufmf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2okflkvqh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2xnvfyeno.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jbgydpkd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2voanvgjs.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2wpllxwgu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bfeabyta.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kzibxqej.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hlhkfbsh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uriqbodt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bbvotcnw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2owmvjpzb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mimwpumi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2nqallyjw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2onnieims.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ajkylvvu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ibstzcdm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mbyutptt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2dxcnlhli.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dhdhoeci.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2axkidzks.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ucdhpief.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2juxexrhi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2bmxjmmso.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ybtsjstu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2yqjouoay.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2mpyiwwty.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2wtrqdxjt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2khyuarhe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvqaavij.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bkeuwxeo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2lzbvogwl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2nhnmjecg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tnyjrakq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cobzjylw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2axanhcgn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fxrhtueo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2iqjzolqm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yvodggpz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ichccmjt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dndpnela.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2kvgzbwmd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2drdfoqyo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2bkuxlifi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pylmnjan.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2oecttere.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vhjcwlbk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ndejfjqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rchulast.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2lholbbfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pdwvmhyq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2skvfqmno.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wbumgrjt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ogeoehjg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2fgpnkqad.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ydvwojth.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xznfnlyc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2phpazksi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2azsdzgor.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2mebmaiyr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gelrvaly.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2zefifuiq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2wyrrvsub.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zjfcwryx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2raridcgy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mwhhhxjf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2eqxazapt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2dgrvhymp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2texqslhd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2zblcndqz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qsqrgwsa.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gqjflliu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2uuyxkaui.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2slnxycrw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvghkrdk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2zlcdzgaa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rsyfytzw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2idzaiqtc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2cqzdlnlb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2fybftbad.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2odnmeisr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jwbbuckk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2griiyljs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ooahzema.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2znwswjgv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2mzkwodzi.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ipeuhpdd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2fnidlzrv.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ideeelwv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2wuevvcmu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ugseolvx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2toleokgl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ibeigzdt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2kinzmpvk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2utzftxol.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2lzgxwhav.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2gmjuxspo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2rigewoyt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2xvkmclvx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2spekahdo.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lfzvzxwm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2fsgfkonw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ybcneist.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2fadydisj.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2jehbgwda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uztppgue.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ubigbpoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbzvalvz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nyztdpif.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2buxmhicf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2aczklkvn.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2urzajzjr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lujcjaey.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2loecsthi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hkargxtj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2hfalnlor.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ffrxxwrf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2botyfbhy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ighazawc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2gemvvaoi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2sxfmzwaw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2boaqgtax.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bonbwiar.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2cinxbspu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2gwmvqwta.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2dlyacysz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2orkdleoy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2bqdmkmza.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2dqiokxzi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zhfgcprn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kzyhhwhb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2plupyqzr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2limufqxc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2unaboqnt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2qvtyklvo.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2hrzbbjym.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2batidxiz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qqmdwxne.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2bzkcudqk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2phfuprmf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hhlwznia.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2gpmthyau.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ronmggzf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cauzfjyl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2malrikxt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2xcbiufiy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2rtrpvjcn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2myedcylj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aztzbrjr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2wkurauol.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nkhbenif.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2gdqokryq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xwocgyul.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2txfxhehs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ozhjforq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vuerxott.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2twybqkco.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkvgkvyk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xigpfeyf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2mzgmxtwk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ngyddqly.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2unjzxsen.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2xhdmzdfs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2fgjurwtc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2wlzytnwm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tifgsdms.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vfpfnylq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rmexuvhv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2bmqcieze.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fuzynney.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ksvkizif.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2tvuzusvd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2cxsnvpok.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hyaqyceq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2wosskxxf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2aapwkstb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2noglyjvw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2antmtsqv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2hqyrtuzx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2jtkevcqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlmhrhbl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ftyetqqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbalttgv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2arrzailj.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2zdynhdhf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ljazqdpt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2sclzrhnm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2drszarnb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wzdjdtfq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2haxaxecg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2nylxiupt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vnwmkzbg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2zuzrfkhi.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zuhsnakk.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2smmzrtct.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2zjnxvtog.html

);
来源：http://www.52xcode.cn/Article/details/gt2zbruqnwy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2olsclqsn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2fdnbpwxv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wflrmgbt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jmairhkp.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2nvohfeye.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2vtueafhe.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2hdheojrx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2eophsfra.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2aogfohke.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2gogbszeh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2vvlwwikx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2fcwxovkl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2prysxetl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ulhdexyp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2wvsvklha.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dtjxzcac.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2qrsryooe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nyvgrcld.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2idimneuq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2pcanvqav.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ayuiupdp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2pbhdfptu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2idkicjzj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2lrfihdpc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2oqrthqrw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wshqcwfn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2zpbmhydm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mlbedkvw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2aimhvdom.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fpitgzbn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2gdnyirwn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2tgqvtytl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2tirpjlue.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2eorixgjm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2culfuxty.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2pbvzbvjq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2bvslynis.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ufwheyqf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ddphhjpc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2crzogtsw.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2lxfqnwlg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2pauqbxnw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2loyevfij.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2aslbcwvz.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cajpmbgt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pipodhqw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2bthcnfiw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2fuxzagwt.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2idnqpqjl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2loiknsph.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2nvoqazsu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jfrloiit.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2wzzosvxd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zuwwxgdj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2njjwtckc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dpebsrtt.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wudkcfrp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2efztchpn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2puyguwsv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kgoylbdq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uusingyg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2izgvbjei.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2mgogywaa.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2bqprqfao.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vtfdvnld.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2gomhulrz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ecuxsmnc.html


<!-- 参考信息 -->