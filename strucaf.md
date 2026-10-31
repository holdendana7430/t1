代发 wailian999

JS:   process.exit(1)
来源：http://uf.bjjhwx.cn

TS:   process.exit(1)
来源：http://gb.nicolike.cn

Java: System.exit(1)
来源：http://tz.muxihuayi.cn

Go:   os.Exit(1)
来源：http://wf.jianghongdianzi.cn

Ruby: exit 1
来源：http://jf.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ml.jctech888.com.cn

[M06] 向标准错误输出
来源：http://bz.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://kc.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uz.chemitech.net.cn

JS:   console.error("err")
来源：http://gb.521024.cn

TS:   console.error("err")
来源：http://yw.nszjky.cn

Java: System.err.println("err")
来源：http://vt.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://id.shxzukj.cn

Ruby: warn "err"
来源：http://wt.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://lw.gzmigu.cn

[M07] 判断是否为主入口
来源：http://rb.521024.cn

Py:   if __name__ == "__main__":
来源：http://qn.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hx.shxzukj.cn

JS:   require.main === module
来源：http://fv.wgjwhj.cn

TS:   require.main === module
来源：http://gt.panjiajie.cn

Java: public static void main(String[] args)
来源：http://fc.chemitech.net.cn

Go:   func main()
来源：http://dw.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pg.hahajie.cn

C#:   static void Main(string[] args)
来源：http://ig.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://pd.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://ly.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://pr.nicolike.cn

JS:   process.platform;  process.version
来源：http://qm.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://xz.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rb.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mz.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kk.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kc.newstarts.cn

================================================================================
来源：http://pl.shtwfgs.cn

N. 数据结构与算法
来源：http://rv.muxihuayi.cn

================================================================================
来源：http://ct.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://nl.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qy.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pw.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ky.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mz.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fk.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://nw.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://do.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vf.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://wl.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://ib.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gn.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ye.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vz.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bp.nszjky.cn

Go:   slices.Sort(arr)
来源：http://zc.chemitech.net.cn

Ruby: arr.sort
来源：http://ch.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ar.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://ot.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wz.haigaiapp.cn

PHP:  // 递归实现，或用 usort
来源：http://cu.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zs.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nu.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ni.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jr.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://st.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bt.panjiajie.cn

[N04] 斐波那契数列
来源：http://st.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mk.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jg.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://he.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wx.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ah.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nz.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://et.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mz.szxytkj.cn

[N05] 最大公约数
来源：http://vf.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://zg.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ft.nicolike.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kd.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ze.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lz.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dq.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://zp.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bw.521024.cn

[N06] 判断回文字符串
来源：http://ac.hnjuh.cn

Py:   s == s[::-1]
来源：http://kq.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://wa.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://zf.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://uf.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://so.hahajie.cn

Go:   // 双指针从两端比较
来源：http://hg.haigaiapp.cn

Ruby: s == s.reverse
来源：http://uu.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nn.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://nq.muxihuayi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hd.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eu.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qt.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://vr.colortex.cn

Java: // 手写 HashMap
来源：http://py.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://hy.panjiajie.cn

Ruby: // 手写 Hash
来源：http://nw.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lp.huixinmuqiang.cn

[N08] 生成全排列
来源：http://ku.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://lx.9csxet.cn

PHP:  // 手写递归交换
来源：http://cd.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://og.panjiajie.cn

TS:   // 手写回溯递归
来源：http://wh.wgjwhj.cn

Java: // 手写回溯递归
来源：http://ng.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://tv.jctech888.com.cn

Ruby: arr.permutation.to_a
来源：http://up.shxzukj.cn

C#:   // 手写回溯递归
来源：http://sn.9csxet.cn

[N09] 栈与队列
来源：http://sj.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ro.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kk.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rr.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://js.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bx.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pw.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zw.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nk.colortex.cn

[N10] 链表节点定义
来源：http://he.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ux.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fi.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dr.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ra.huanxung.cn

Java: class Node { int v; Node next; }
来源：http://fq.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ap.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vp.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vx.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://hv.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qc.colortex.cn

PHP:  // 手写递归函数
来源：http://pc.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vo.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mq.panjiajie.cn

Java: // 手写递归
来源：http://mq.nszjky.cn

Go:   // 手写递归
来源：http://mn.szsharing.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zd.szsharing.cn

C#:   // 手写递归
来源：http://xt.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dn.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lb.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dt.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uz.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zo.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iz.newstarts.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fj.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ls.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ps.bookmarksfly.cn

================================================================================
来源：http://ax.bookmarksfly.cn

O. 并发与异步
来源：http://mv.huixiangedu.cn

================================================================================
来源：http://wb.gzmigu.cn

[O01] 启动一个线程
来源：http://pv.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sw.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cp.huixinmuqiang.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://po.huixiangedu.cn

TS:   // 同 JS
来源：http://au.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://ln.huixinmuqiang.cn

Go:   go f()
来源：http://fu.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://qe.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://xs.asd995.cn

[O02] 使用线程池
来源：http://jq.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ob.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kl.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://af.hahajie.cn

TS:   // worker_threads 线程池
来源：http://nm.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ff.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://or.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zn.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://io.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://po.panjiajie.cn

Py:   with lock: shared += 1
来源：http://gh.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://hi.nszjky.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fg.9csxet.cn

TS:   // 同 JS
来源：http://cr.muxihuayi.cn

Java: synchronized (this) { shared++; }
来源：http://qu.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qn.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ag.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://xg.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://xh.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://aj.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pi.nszjky.cn

JS:   async function f() { await g(); }
来源：http://zj.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://va.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vb.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zf.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hk.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://tl.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://ew.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://ji.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ys.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://pc.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://an.szsharing.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jg.colortex.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dd.szsharing.cn

Ruby: threads.map(&:join)
来源：http://mt.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pa.hahajie.cn

[O06] 使用进程池
来源：http://kc.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xn.asd995.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pq.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://dz.yuexingan06.cn

TS:   // child_process / cluster 模块
来源：http://fw.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gp.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ox.9csxet.cn

Ruby: // fork 块
来源：http://dq.bookmarksfly.cn

C#:   Parallel.For
来源：http://mz.shtwfgs.cn

================================================================================
来源：http://qh.gzmigu.cn

P. 常用工具函数
来源：http://to.colortex.cn

================================================================================
来源：http://nz.shxzskj.cn

[P01] 生成 UUID
来源：http://oy.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://gd.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lq.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://cv.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://yk.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://kl.panjiajie.cn

Go:   // 用 github.com/google/uuid
来源：http://fi.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://nm.szxytkj.cn

C#:   Guid.NewGuid().ToString()
来源：http://mf.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://ur.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dc.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xo.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yj.lnxyls.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dd.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ge.nszjky.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hr.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ty.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yd.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://na.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mc.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://do.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ll.wgjwhj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pm.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nz.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aw.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rv.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lo.jctech888.com.cn

[P04] 求长度
来源：http://ih.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.huanxung.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qq.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vr.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ve.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://og.hahajie.cn

Go:   len(arr);  len(m)
来源：http://pp.shxzskj.cn

Ruby: x.length;  x.size
来源：http://gg.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xh.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://ks.yuexingan06.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tm.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kq.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fw.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ja.shxzskj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qd.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ij.szxytkj.cn

Ruby: a == b
来源：http://yo.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://db.yuexingan06.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ns.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mh.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://wn.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cd.jctech888.com.cn

TS:   if (x == null) {}
来源：http://jk.wgjwhj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nx.nszjky.cn

Go:   if x == nil {}
来源：http://la.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qe.bjjhwx.cn

C#:   if (x is null) {}
来源：http://ph.huixiangedu.cn

[P07] 防抖与节流
来源：http://sd.jctech888.com.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nz.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://ip.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://md.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ms.hnjuh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hc.521024.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ri.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vw.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nw.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://rt.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rn.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://su.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jm.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gv.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zy.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fb.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jl.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zo.9csxet.cn

================================================================================
来源：http://pt.hahajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ly.muxihuayi.cn

================================================================================
来源：http://if.shtwfgs.cn

[Q01] 创建表
来源：http://wu.shxzskj.cn

CREATE TABLE users (
来源：http://fq.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cf.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://dp.shxzukj.cn

email VARCHAR(100) UNIQUE,
来源：http://pl.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hy.nicolike.cn

);
来源：http://wn.hnjuh.cn

[Q02] 创建带外键的表
来源：http://wf.huixinmuqiang.cn

CREATE TABLE orders (
来源：http://xt.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yh.jctech888.com.cn

user_id INT NOT NULL,
来源：http://cb.nszjky.cn

amount DECIMAL(10, 2),
来源：http://uw.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xd.shxzskj.cn

);
来源：http://ui.hnjuh.cn

[Q03] 增加列
来源：http://ma.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vu.nicolike.cn

[Q04] 修改列类型
来源：http://je.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bj.9csxet.cn

[Q05] 重命名列
来源：http://am.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bw.yuexingan06.cn

[Q06] 删除列
来源：http://sy.lnxyls.cn


<!-- 参考信息 -->