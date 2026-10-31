代发 wailian999

TS:   process.cwd()
来源：http://wv.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://jg.bjjhwx.cn

Go:   os.Getwd()
来源：http://vx.muxihuayi.cn

Ruby: Dir.pwd
来源：http://fa.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kv.huanxung.cn

[M05] 设置退出码
来源：http://fy.huanxung.cn

Py:   sys.exit(1)
来源：http://lo.hahajie.cn

PHP:  exit(1);
来源：http://tl.colortex.cn

JS:   process.exit(1)
来源：http://ij.nicolike.cn

TS:   process.exit(1)
来源：http://cv.newstarts.cn

Java: System.exit(1)
来源：http://ul.huixiangedu.cn

Go:   os.Exit(1)
来源：http://va.asd995.cn

Ruby: exit 1
来源：http://hn.wgjwhj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mj.chemitech.net.cn

[M06] 向标准错误输出
来源：http://rg.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://us.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pz.521024.cn

JS:   console.error("err")
来源：http://jt.jctech888.com.cn

TS:   console.error("err")
来源：http://oh.nszjky.cn

Java: System.err.println("err")
来源：http://ee.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zo.521024.cn

Ruby: warn "err"
来源：http://ht.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://el.newstarts.cn

[M07] 判断是否为主入口
来源：http://kz.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://mu.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wf.9csxet.cn

JS:   require.main === module
来源：http://vd.9csxet.cn

TS:   require.main === module
来源：http://eu.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://fb.chemitech.net.cn

Go:   func main()
来源：http://by.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sx.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://wy.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://st.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://sq.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://qc.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://nv.521024.cn

TS:   process.platform;  process.version
来源：http://sq.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fl.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ff.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ba.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xn.jianghongdianzi.cn

================================================================================
来源：http://mz.asd995.cn

N. 数据结构与算法
来源：http://ch.nicolike.cn

================================================================================
来源：http://en.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://ew.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pl.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kp.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sp.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gs.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zy.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://vo.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wl.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yu.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://gn.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://ez.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ew.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ql.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mc.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ka.huanxung.cn

Go:   slices.Sort(arr)
来源：http://ii.jctech888.com.cn

Ruby: arr.sort
来源：http://ml.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://it.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://uf.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xd.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://kv.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ul.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jw.newstarts.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uf.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gb.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bl.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vz.wgjwhj.cn

[N04] 斐波那契数列
来源：http://go.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://md.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bo.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sf.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nm.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sz.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jh.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wz.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dr.newstarts.cn

[N05] 最大公约数
来源：http://jh.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://ud.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fi.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sq.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zb.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tk.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gf.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://tk.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ra.szsharing.cn

[N06] 判断回文字符串
来源：http://kg.panjiajie.cn

Py:   s == s[::-1]
来源：http://sv.521024.cn

PHP:  $s === strrev($s);
来源：http://rt.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://ti.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://ch.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fi.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://hr.shtwfgs.cn

Ruby: s == s.reverse
来源：http://ew.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://eh.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://sn.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bn.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uk.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qv.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://vu.shtwfgs.cn

Java: // 手写 HashMap
来源：http://kg.nszjky.cn

Go:   // 手写 map[int]int
来源：http://fw.panjiajie.cn

Ruby: // 手写 Hash
来源：http://ip.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zs.nicolike.cn

[N08] 生成全排列
来源：http://ly.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://ru.asd995.cn

PHP:  // 手写递归交换
来源：http://iv.nszjky.cn

JS:   // 手写回溯递归
来源：http://vh.521024.cn

TS:   // 手写回溯递归
来源：http://po.yuexingan06.cn

Java: // 手写回溯递归
来源：http://hy.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://mi.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://io.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://dc.szsharing.cn

[N09] 栈与队列
来源：http://aq.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wt.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gr.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://za.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hs.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://po.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://av.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vf.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ga.muxihuayi.cn

[N10] 链表节点定义
来源：http://nw.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://af.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://us.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kh.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lk.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://gg.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zi.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hs.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://it.nicolike.cn

[N11] 二叉树中序遍历
来源：http://ft.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://es.szxytkj.cn

PHP:  // 手写递归函数
来源：http://hf.hnjuh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kc.jctech888.com.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nz.haigaiapp.cn

Java: // 手写递归
来源：http://bi.huanxung.cn

Go:   // 手写递归
来源：http://li.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jl.shxzukj.cn

C#:   // 手写递归
来源：http://ud.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qg.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xe.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sm.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yv.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://co.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ek.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rn.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gh.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zp.nicolike.cn

================================================================================
来源：http://kz.chemitech.net.cn

O. 并发与异步
来源：http://ph.lnxyls.cn

================================================================================
来源：http://yf.yuexingan06.cn

[O01] 启动一个线程
来源：http://od.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nk.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qm.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zt.szsharing.cn

TS:   // 同 JS
来源：http://kt.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://vq.jctech888.com.cn

Go:   go f()
来源：http://ls.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://sk.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://aa.asd995.cn

[O02] 使用线程池
来源：http://to.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wh.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://px.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://lp.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://zh.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fh.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nk.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vd.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ao.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://be.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://ac.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://fa.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yg.nszjky.cn

TS:   // 同 JS
来源：http://xq.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://wu.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mc.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vw.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://dx.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://xf.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://cl.gzmigu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://na.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://kg.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ur.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xf.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ej.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rg.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://so.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://zr.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://vb.chemitech.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://be.asd995.cn

JS:   await Promise.all(tasks)
来源：http://ms.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://lj.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wp.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ub.wgjwhj.cn

Ruby: threads.map(&:join)
来源：http://ws.panjiajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fw.lnxyls.cn

[O06] 使用进程池
来源：http://ka.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://we.muxihuayi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ic.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://qr.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://sn.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nl.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qn.huixiangedu.cn

Ruby: // fork 块
来源：http://mj.shxzukj.cn

C#:   Parallel.For
来源：http://rc.szsharing.cn

================================================================================
来源：http://sa.wgjwhj.cn

P. 常用工具函数
来源：http://cn.haigaiapp.cn

================================================================================
来源：http://ci.panjiajie.cn

[P01] 生成 UUID
来源：http://vm.colortex.cn

Py:   str(uuid.uuid4())
来源：http://nd.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xz.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://ra.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://oq.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://pu.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://na.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://hb.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://vo.chemitech.net.cn

[P02] MD5 / SHA256 摘要
来源：http://fe.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qn.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qz.bjjhwx.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mk.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tu.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mm.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ja.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rh.521024.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qp.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://ir.huixinmuqiang.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yz.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hi.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nf.shtwfgs.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nq.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dg.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dd.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sq.muxihuayi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mr.szsharing.cn

[P04] 求长度
来源：http://cp.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lj.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pj.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bv.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://je.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://cd.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://ex.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://mk.wgjwhj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://oi.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://xt.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://eh.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ex.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yr.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tj.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tk.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vt.nicolike.cn

Ruby: a == b
来源：http://zl.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ao.jianghongdianzi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://so.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rh.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://ev.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://le.haigaiapp.cn

TS:   if (x == null) {}
来源：http://in.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wc.asd995.cn

Go:   if x == nil {}
来源：http://ad.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xt.huixinmuqiang.cn

C#:   if (x is null) {}
来源：http://lq.asd995.cn

[P07] 防抖与节流
来源：http://iv.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vb.colortex.cn

PHP:  // 手写时间戳比较
来源：http://zz.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zb.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ab.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gd.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ik.yuexingan06.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://py.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ug.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://ja.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dr.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xe.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gn.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://is.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ar.wgjwhj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vo.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yw.panjiajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ei.shxzukj.cn

================================================================================
来源：http://ld.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mo.bookmarksfly.cn

================================================================================
来源：http://xx.muxihuayi.cn

[Q01] 创建表
来源：http://fb.shxzskj.cn

CREATE TABLE users (
来源：http://mv.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ls.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://ky.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://ax.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gm.521024.cn

);
来源：http://ux.nicolike.cn

[Q02] 创建带外键的表
来源：http://eu.hahajie.cn

CREATE TABLE orders (
来源：http://le.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fu.nicolike.cn

user_id INT NOT NULL,
来源：http://gh.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://ww.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fo.bjjhwx.cn


<!-- 参考信息 -->