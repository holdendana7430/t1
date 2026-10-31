代发 wailian999

[M04] 获取当前工作目录
来源：http://lc.asd995.cn

Py:   os.getcwd()
来源：http://oy.shxzskj.cn

PHP:  getcwd();
来源：http://mx.shxzskj.cn

JS:   process.cwd()
来源：http://oz.wgjwhj.cn

TS:   process.cwd()
来源：http://fh.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://kt.bookmarksfly.cn

Go:   os.Getwd()
来源：http://fb.shxzskj.cn

Ruby: Dir.pwd
来源：http://pi.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vm.hnjuh.cn

[M05] 设置退出码
来源：http://fk.hnjuh.cn

Py:   sys.exit(1)
来源：http://jr.lnxyls.cn

PHP:  exit(1);
来源：http://ib.haigaiapp.cn

JS:   process.exit(1)
来源：http://du.newstarts.cn

TS:   process.exit(1)
来源：http://qx.chemitech.net.cn

Java: System.exit(1)
来源：http://bq.shxzukj.cn

Go:   os.Exit(1)
来源：http://ip.521024.cn

Ruby: exit 1
来源：http://dy.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zj.hahajie.cn

[M06] 向标准错误输出
来源：http://je.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://qc.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://br.huixiangedu.cn

JS:   console.error("err")
来源：http://wa.521024.cn

TS:   console.error("err")
来源：http://dh.shxzskj.cn

Java: System.err.println("err")
来源：http://kp.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xw.shxzskj.cn

Ruby: warn "err"
来源：http://sr.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://sr.panjiajie.cn

[M07] 判断是否为主入口
来源：http://vi.panjiajie.cn

Py:   if __name__ == "__main__":
来源：http://ez.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pt.shxzukj.cn

JS:   require.main === module
来源：http://ar.yuntaijiaju.cn

TS:   require.main === module
来源：http://eg.huanxung.cn

Java: public static void main(String[] args)
来源：http://fu.huixinmuqiang.cn

Go:   func main()
来源：http://st.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tq.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://ti.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://cf.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://wd.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://br.shxzskj.cn

JS:   process.platform;  process.version
来源：http://ah.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://vr.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lk.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hw.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ls.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sy.szxytkj.cn

================================================================================
来源：http://yz.wgjwhj.cn

N. 数据结构与算法
来源：http://gv.chemitech.net.cn

================================================================================
来源：http://oz.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://ry.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dm.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dj.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pc.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bq.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ev.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://da.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lf.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qk.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://ir.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://tc.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qj.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qm.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://li.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gj.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://zj.yuntaijiaju.cn

Ruby: arr.sort
来源：http://sd.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xl.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://qp.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ff.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://kf.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ln.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wf.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pt.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ly.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ze.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ub.shtwfgs.cn

[N04] 斐波那契数列
来源：http://nv.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://od.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xc.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://em.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://al.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yn.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://io.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bh.huixiangedu.cn

[N05] 最大公约数
来源：http://el.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://mh.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rx.colortex.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zn.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sz.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dz.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qt.nszjky.cn

Ruby: a.gcd(b)
来源：http://cd.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ka.szsharing.cn

[N06] 判断回文字符串
来源：http://dx.huixiangedu.cn

Py:   s == s[::-1]
来源：http://ar.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://ho.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://fr.bjjhwx.cn

TS:   s === [...s].reverse().join("")
来源：http://wg.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qa.521024.cn

Go:   // 双指针从两端比较
来源：http://xs.hahajie.cn

Ruby: s == s.reverse
来源：http://ba.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ca.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://cf.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wp.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qh.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tk.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://qw.colortex.cn

Java: // 手写 HashMap
来源：http://jp.newstarts.cn

Go:   // 手写 map[int]int
来源：http://ho.panjiajie.cn

Ruby: // 手写 Hash
来源：http://ec.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kh.521024.cn

[N08] 生成全排列
来源：http://cs.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://gt.shxzskj.cn

PHP:  // 手写递归交换
来源：http://kk.szxytkj.cn

JS:   // 手写回溯递归
来源：http://dn.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://pj.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://px.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://fu.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://ok.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://hw.bookmarksfly.cn

[N09] 栈与队列
来源：http://hz.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yx.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jb.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gh.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tq.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gp.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jj.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tu.colortex.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nb.nszjky.cn

[N10] 链表节点定义
来源：http://hq.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jq.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xg.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mu.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xo.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://cz.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ae.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yf.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ih.nszjky.cn

[N11] 二叉树中序遍历
来源：http://fq.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vd.lnxyls.cn

PHP:  // 手写递归函数
来源：http://yo.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dt.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sv.yuexingan06.cn

Java: // 手写递归
来源：http://oy.hnjuh.cn

Go:   // 手写递归
来源：http://qr.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gm.lnxyls.cn

C#:   // 手写递归
来源：http://yu.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vq.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wv.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://md.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ub.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eg.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uk.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cv.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ma.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://co.huixiangedu.cn

================================================================================
来源：http://zf.hnjuh.cn

O. 并发与异步
来源：http://ln.huixinmuqiang.cn

================================================================================
来源：http://sy.wgjwhj.cn

[O01] 启动一个线程
来源：http://xa.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vx.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ra.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wi.chemitech.net.cn

TS:   // 同 JS
来源：http://mc.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://mi.chemitech.net.cn

Go:   go f()
来源：http://bx.hahajie.cn

Ruby: Thread.new { f }
来源：http://yu.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://kl.nszjky.cn

[O02] 使用线程池
来源：http://eg.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rg.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dz.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://bm.lnxyls.cn

TS:   // worker_threads 线程池
来源：http://fd.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ug.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hu.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dq.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xb.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://dp.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://cd.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://cc.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jw.asd995.cn

TS:   // 同 JS
来源：http://wn.lnxyls.cn

Java: synchronized (this) { shared++; }
来源：http://vp.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://je.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gg.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://bt.hahajie.cn

[O04] 定义异步函数并等待
来源：http://lp.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://kt.gzmigu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kz.521024.cn

JS:   async function f() { await g(); }
来源：http://pv.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ql.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nx.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zo.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ih.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://ma.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://kj.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://ie.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nx.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://tk.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://at.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aw.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ww.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://dd.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tl.huanxung.cn

[O06] 使用进程池
来源：http://lw.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://im.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xf.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://yc.jctech888.com.cn

TS:   // child_process / cluster 模块
来源：http://nb.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cl.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ov.9csxet.cn

Ruby: // fork 块
来源：http://uz.asd995.cn

C#:   Parallel.For
来源：http://pj.newstarts.cn

================================================================================
来源：http://xs.9csxet.cn

P. 常用工具函数
来源：http://or.huixinmuqiang.cn

================================================================================
来源：http://bw.wgjwhj.cn

[P01] 生成 UUID
来源：http://ga.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://rl.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wm.9csxet.cn

JS:   crypto.randomUUID()
来源：http://qw.szsharing.cn

TS:   crypto.randomUUID()
来源：http://ue.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://qq.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://oo.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://sx.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://ne.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://qj.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zm.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jv.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dc.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qd.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nd.wgjwhj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qh.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hf.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ez.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://pq.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dj.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zi.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qo.nszjky.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cg.colortex.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fz.muxihuayi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pc.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qi.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xo.colortex.cn

[P04] 求长度
来源：http://sy.muxihuayi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dm.bjjhwx.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lf.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vt.huixinmuqiang.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jy.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://oo.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://hh.huanxung.cn

Ruby: x.length;  x.size
来源：http://ay.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pg.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://yw.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ok.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://do.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xv.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jm.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mk.nicolike.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vl.szxytkj.cn

Ruby: a == b
来源：http://ef.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xq.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sv.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jb.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://bl.szsharing.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gk.muxihuayi.cn

TS:   if (x == null) {}
来源：http://xq.chemitech.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tf.panjiajie.cn

Go:   if x == nil {}
来源：http://op.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rs.yuexingan06.cn

C#:   if (x is null) {}
来源：http://bq.szsharing.cn

[P07] 防抖与节流
来源：http://te.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yq.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://hg.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lv.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ju.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ag.9csxet.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pw.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qe.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rf.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://gt.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://by.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zu.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://su.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vp.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lk.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://aw.lnxyls.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jj.wgjwhj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uo.asd995.cn

================================================================================
来源：http://xj.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wq.muxihuayi.cn

================================================================================
来源：http://di.huixiangedu.cn

[Q01] 创建表
来源：http://gu.nicolike.cn

CREATE TABLE users (
来源：http://ex.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tm.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://si.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://cc.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tj.gzmigu.cn

);
来源：http://zo.asd995.cn

[Q02] 创建带外键的表
来源：http://ua.asd995.cn

CREATE TABLE orders (
来源：http://rc.huanxung.cn


<!-- 参考信息 -->