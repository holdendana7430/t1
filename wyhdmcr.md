代发 wailian999

TS:   process.cwd()
来源：http://ne.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://hb.nicolike.cn

Go:   os.Getwd()
来源：http://vc.szsharing.cn

Ruby: Dir.pwd
来源：http://bz.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ox.nicolike.cn

[M05] 设置退出码
来源：http://pv.hahajie.cn

Py:   sys.exit(1)
来源：http://dg.9csxet.cn

PHP:  exit(1);
来源：http://ay.nszjky.cn

JS:   process.exit(1)
来源：http://wh.panjiajie.cn

TS:   process.exit(1)
来源：http://lv.nszjky.cn

Java: System.exit(1)
来源：http://zk.lnxyls.cn

Go:   os.Exit(1)
来源：http://ds.521024.cn

Ruby: exit 1
来源：http://wi.wgjwhj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bv.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://mk.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://vi.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ea.haigaiapp.cn

JS:   console.error("err")
来源：http://pm.lnxyls.cn

TS:   console.error("err")
来源：http://lf.szsharing.cn

Java: System.err.println("err")
来源：http://ep.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lm.gzmigu.cn

Ruby: warn "err"
来源：http://vy.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://bf.gzmigu.cn

[M07] 判断是否为主入口
来源：http://gn.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://cx.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://av.panjiajie.cn

JS:   require.main === module
来源：http://pq.panjiajie.cn

TS:   require.main === module
来源：http://js.hnjuh.cn

Java: public static void main(String[] args)
来源：http://go.bookmarksfly.cn

Go:   func main()
来源：http://sa.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vn.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://ek.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://sz.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://tu.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://hr.panjiajie.cn

JS:   process.platform;  process.version
来源：http://hq.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://dc.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kj.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ot.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://av.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ob.nszjky.cn

================================================================================
来源：http://op.colortex.cn

N. 数据结构与算法
来源：http://ye.huixiangedu.cn

================================================================================
来源：http://ip.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://kw.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yt.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sv.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qp.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gb.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://la.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://mz.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ku.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jn.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://cc.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://qh.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://st.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ka.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wq.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ym.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://ax.szsharing.cn

Ruby: arr.sort
来源：http://jq.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nx.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://sc.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wy.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://ic.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://en.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qr.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gx.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wt.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lq.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vz.9csxet.cn

[N04] 斐波那契数列
来源：http://qp.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://je.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rf.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bf.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jl.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fx.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xp.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://we.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gl.huixiangedu.cn

[N05] 最大公约数
来源：http://bj.huanxung.cn

Py:   math.gcd(a, b)
来源：http://uv.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yq.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bn.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mm.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yv.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ij.hnjuh.cn

Ruby: a.gcd(b)
来源：http://on.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://od.nicolike.cn

[N06] 判断回文字符串
来源：http://yh.nszjky.cn

Py:   s == s[::-1]
来源：http://dv.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://fz.panjiajie.cn

JS:   s === [...s].reverse().join("")
来源：http://wb.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://kp.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gu.newstarts.cn

Go:   // 双指针从两端比较
来源：http://gz.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://pk.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xm.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://dn.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bp.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ai.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dl.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://lx.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://lg.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://hp.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://oz.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iq.panjiajie.cn

[N08] 生成全排列
来源：http://ik.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://ha.521024.cn

PHP:  // 手写递归交换
来源：http://ur.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://xe.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://fi.chemitech.net.cn

Java: // 手写回溯递归
来源：http://ug.panjiajie.cn

Go:   // 手写回溯递归
来源：http://qi.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://vq.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://di.521024.cn

[N09] 栈与队列
来源：http://wf.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fk.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ah.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lr.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rj.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iq.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zb.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qq.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://go.hnjuh.cn

[N10] 链表节点定义
来源：http://nd.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://on.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rp.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://co.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xu.521024.cn

Java: class Node { int v; Node next; }
来源：http://hk.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fx.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ao.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pi.huanxung.cn

[N11] 二叉树中序遍历
来源：http://ea.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dj.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://ho.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qj.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zu.haigaiapp.cn

Java: // 手写递归
来源：http://ao.hnjuh.cn

Go:   // 手写递归
来源：http://th.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qj.nszjky.cn

C#:   // 手写递归
来源：http://nn.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ny.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iz.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mp.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://za.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pr.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ig.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://as.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ux.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ho.colortex.cn

================================================================================
来源：http://qq.asd995.cn

O. 并发与异步
来源：http://we.shtwfgs.cn

================================================================================
来源：http://be.bjjhwx.cn

[O01] 启动一个线程
来源：http://hi.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nb.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qd.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ql.lnxyls.cn

TS:   // 同 JS
来源：http://bf.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://ao.huixiangedu.cn

Go:   go f()
来源：http://vu.shxzukj.cn

Ruby: Thread.new { f }
来源：http://rk.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://vg.nicolike.cn

[O02] 使用线程池
来源：http://ln.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bz.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zf.lnxyls.cn

JS:   // worker_threads 线程池
来源：http://ki.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://yb.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ej.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mf.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wi.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ky.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://vy.hnjuh.cn

Py:   with lock: shared += 1
来源：http://gp.shxzukj.cn

PHP:  // 用 flock() 做文件锁
来源：http://at.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://az.haigaiapp.cn

TS:   // 同 JS
来源：http://oi.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://nv.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qf.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://za.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://tc.521024.cn

[O04] 定义异步函数并等待
来源：http://st.521024.cn

Py:   async def f():⏎    await g()
来源：http://xr.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xh.521024.cn

JS:   async function f() { await g(); }
来源：http://qv.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wa.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fw.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bb.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yb.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://pb.521024.cn

[O05] 并发执行并等待全部完成
来源：http://cv.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://uf.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kv.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://xx.colortex.cn

TS:   await Promise.all(tasks)
来源：http://yj.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bw.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ut.asd995.cn

Ruby: threads.map(&:join)
来源：http://al.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pd.szxytkj.cn

[O06] 使用进程池
来源：http://kh.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tb.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lr.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://la.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://dx.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pt.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://md.huixiangedu.cn

Ruby: // fork 块
来源：http://ll.bjjhwx.cn

C#:   Parallel.For
来源：http://hw.hahajie.cn

================================================================================
来源：http://qu.hahajie.cn

P. 常用工具函数
来源：http://ih.521024.cn

================================================================================
来源：http://sw.hnjuh.cn

[P01] 生成 UUID
来源：http://zj.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://cn.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sz.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://dt.jctech888.com.cn

TS:   crypto.randomUUID()
来源：http://wq.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://ik.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://bt.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://fa.gzmigu.cn

C#:   Guid.NewGuid().ToString()
来源：http://ve.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://tl.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://au.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zh.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ol.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sd.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://eq.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oi.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ky.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fe.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://op.bookmarksfly.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cq.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ss.nicolike.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bj.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uq.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pq.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vj.szsharing.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vw.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ba.yuexingan06.cn

[P04] 求长度
来源：http://eb.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ls.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jk.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://co.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tz.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://aj.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://gd.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://pw.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tx.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://gb.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cv.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ow.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pu.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hg.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sq.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jw.newstarts.cn

Ruby: a == b
来源：http://de.hahajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://db.yuexingan06.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bt.lnxyls.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://do.asd995.cn

PHP:  if (empty($x)) {}
来源：http://va.9csxet.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ve.huanxung.cn

TS:   if (x == null) {}
来源：http://uu.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ip.haigaiapp.cn

Go:   if x == nil {}
来源：http://ws.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ya.huanxung.cn

C#:   if (x is null) {}
来源：http://ad.huanxung.cn

[P07] 防抖与节流
来源：http://st.shxzskj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nx.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://od.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://es.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ds.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wk.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vu.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tk.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ca.9csxet.cn

[P08] 处理浮点精度问题
来源：http://pu.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gz.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xk.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gg.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kb.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xn.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mv.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yt.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sz.jianghongdianzi.cn

================================================================================
来源：http://ps.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cd.newstarts.cn

================================================================================
来源：http://lg.szsharing.cn

[Q01] 创建表
来源：http://hd.haigaiapp.cn

CREATE TABLE users (
来源：http://zk.nszjky.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pn.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://fw.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://ws.bjjhwx.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ui.gzmigu.cn

);
来源：http://bk.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://vp.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://zq.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://si.huixiangedu.cn

user_id INT NOT NULL,
来源：http://hw.yuexingan06.cn

amount DECIMAL(10, 2),
来源：http://jr.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ea.lnxyls.cn


<!-- 参考信息 -->