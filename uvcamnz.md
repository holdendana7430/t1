代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ma.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://ny.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ar.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://by.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xj.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://il.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zv.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://io.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qw.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xo.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tj.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://wj.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://xw.nicolike.cn

Py:   os.getcwd()
来源：http://jj.shtwfgs.cn

PHP:  getcwd();
来源：http://es.hahajie.cn

JS:   process.cwd()
来源：http://br.bookmarksfly.cn

TS:   process.cwd()
来源：http://wk.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://cz.nicolike.cn

Go:   os.Getwd()
来源：http://fa.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://xz.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ee.shxzskj.cn

[M05] 设置退出码
来源：http://qx.shxzukj.cn

Py:   sys.exit(1)
来源：http://hs.shxzukj.cn

PHP:  exit(1);
来源：http://bg.shxzukj.cn

JS:   process.exit(1)
来源：http://se.shxzskj.cn

TS:   process.exit(1)
来源：http://kt.huixinmuqiang.cn

Java: System.exit(1)
来源：http://pg.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://ww.shxzskj.cn

Ruby: exit 1
来源：http://be.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kz.bjjhwx.cn

[M06] 向标准错误输出
来源：http://uv.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://as.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xc.muxihuayi.cn

JS:   console.error("err")
来源：http://qu.shxzukj.cn

TS:   console.error("err")
来源：http://hw.hahajie.cn

Java: System.err.println("err")
来源：http://kj.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sn.wgjwhj.cn

Ruby: warn "err"
来源：http://gf.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://xv.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://in.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://pq.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cq.asd995.cn

JS:   require.main === module
来源：http://xu.yuexingan06.cn

TS:   require.main === module
来源：http://uu.9csxet.cn

Java: public static void main(String[] args)
来源：http://mn.shxzukj.cn

Go:   func main()
来源：http://ef.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pe.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://id.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://vl.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://ol.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://xi.shxzukj.cn

JS:   process.platform;  process.version
来源：http://oc.huanxung.cn

TS:   process.platform;  process.version
来源：http://rp.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fd.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://um.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bf.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vp.521024.cn

================================================================================
来源：http://vj.shxzskj.cn

N. 数据结构与算法
来源：http://za.yuexingan06.cn

================================================================================
来源：http://sz.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://sa.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hm.szxytkj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cs.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rf.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lm.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mu.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://of.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ez.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ip.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://el.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://if.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xb.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://df.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gv.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sf.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://vb.hnjuh.cn

Ruby: arr.sort
来源：http://zo.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xr.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://uo.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vr.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://xc.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://to.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ge.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ql.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cb.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tu.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fx.nszjky.cn

[N04] 斐波那契数列
来源：http://sx.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nm.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://az.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kg.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jk.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nl.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ge.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sf.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wu.shxzskj.cn

[N05] 最大公约数
来源：http://vl.colortex.cn

Py:   math.gcd(a, b)
来源：http://yv.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://di.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://da.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ny.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zq.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mb.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://cc.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nl.huanxung.cn

[N06] 判断回文字符串
来源：http://pj.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://ur.nszjky.cn

PHP:  $s === strrev($s);
来源：http://ny.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://ah.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://di.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://da.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://qc.jctech888.com.cn

Ruby: s == s.reverse
来源：http://zt.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bm.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://rt.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://as.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vl.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sf.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://yo.lnxyls.cn

Java: // 手写 HashMap
来源：http://sv.colortex.cn

Go:   // 手写 map[int]int
来源：http://xn.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://eh.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fg.bjjhwx.cn

[N08] 生成全排列
来源：http://fj.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://po.hahajie.cn

PHP:  // 手写递归交换
来源：http://tq.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://cu.szxytkj.cn

TS:   // 手写回溯递归
来源：http://nr.yuexingan06.cn

Java: // 手写回溯递归
来源：http://lr.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://xq.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://jq.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://ja.hahajie.cn

[N09] 栈与队列
来源：http://te.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ro.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nu.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fj.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zf.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qw.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hj.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ti.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wo.bookmarksfly.cn

[N10] 链表节点定义
来源：http://ax.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ar.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nx.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dp.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sa.chemitech.net.cn

Java: class Node { int v; Node next; }
来源：http://id.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fc.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qo.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wu.colortex.cn

[N11] 二叉树中序遍历
来源：http://of.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jn.panjiajie.cn

PHP:  // 手写递归函数
来源：http://xo.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lt.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ys.panjiajie.cn

Java: // 手写递归
来源：http://qq.9csxet.cn

Go:   // 手写递归
来源：http://kv.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nl.colortex.cn

C#:   // 手写递归
来源：http://du.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oi.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fb.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oo.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://na.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rt.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ef.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ug.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dl.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cc.szsharing.cn

================================================================================
来源：http://rg.hnjuh.cn

O. 并发与异步
来源：http://ew.szxytkj.cn

================================================================================
来源：http://vw.lnxyls.cn

[O01] 启动一个线程
来源：http://ho.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pq.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vr.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cu.shxzskj.cn

TS:   // 同 JS
来源：http://lz.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://rq.gzmigu.cn

Go:   go f()
来源：http://hj.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://sz.newstarts.cn

C#:   Task.Run(() => F());
来源：http://ch.haigaiapp.cn

[O02] 使用线程池
来源：http://zn.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ql.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ny.colortex.cn

JS:   // worker_threads 线程池
来源：http://yx.huixiangedu.cn

TS:   // worker_threads 线程池
来源：http://mc.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://py.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ve.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eo.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vq.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://rg.asd995.cn

Py:   with lock: shared += 1
来源：http://jj.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://ou.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://co.colortex.cn

TS:   // 同 JS
来源：http://lt.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://df.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ft.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gg.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://sm.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://bn.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://rh.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dc.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://ax.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xj.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://un.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fb.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bl.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://dr.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://zl.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://sl.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ag.colortex.cn

JS:   await Promise.all(tasks)
来源：http://ki.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://ub.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eu.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fr.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://rk.lnxyls.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kp.bjjhwx.cn

[O06] 使用进程池
来源：http://og.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wm.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qd.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://ty.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://pz.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://le.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mm.bookmarksfly.cn

Ruby: // fork 块
来源：http://ue.521024.cn

C#:   Parallel.For
来源：http://dw.szxytkj.cn

================================================================================
来源：http://dy.jctech888.com.cn

P. 常用工具函数
来源：http://ja.huanxung.cn

================================================================================
来源：http://yx.lnxyls.cn

[P01] 生成 UUID
来源：http://rx.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://ji.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zk.colortex.cn

JS:   crypto.randomUUID()
来源：http://ff.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://lc.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://dk.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://qd.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://ed.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://bc.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://ow.hnjuh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://we.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oe.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qg.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yf.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ct.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ky.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ir.521024.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://au.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://mp.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cf.bjjhwx.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://be.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lb.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sz.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qo.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wy.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ck.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hx.9csxet.cn

[P04] 求长度
来源：http://ef.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oo.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wh.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fi.jctech888.com.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cm.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://zv.hahajie.cn

Go:   len(arr);  len(m)
来源：http://ev.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://ks.gzmigu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://eb.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://ne.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mm.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ru.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ui.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jo.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rd.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sw.asd995.cn

Ruby: a == b
来源：http://nw.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dz.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fl.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ep.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://la.jctech888.com.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ix.asd995.cn

TS:   if (x == null) {}
来源：http://zh.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uh.huanxung.cn

Go:   if x == nil {}
来源：http://ue.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xh.9csxet.cn

C#:   if (x is null) {}
来源：http://tj.colortex.cn

[P07] 防抖与节流
来源：http://pp.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pg.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://co.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://au.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ag.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ai.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lx.yuexingan06.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vf.lnxyls.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kj.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://gc.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tx.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zm.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qp.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kh.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gu.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gn.hahajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gb.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yh.nszjky.cn


<!-- 参考信息 -->