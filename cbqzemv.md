代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ae.asd995.cn

JS:   process.env.HOME
来源：http://vd.jctech888.com.cn

TS:   process.env.HOME
来源：http://ol.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://uk.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eg.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://qr.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ua.newstarts.cn

[M03] 执行外部命令
来源：http://ow.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dw.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eu.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://za.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kv.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oa.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sd.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xg.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://av.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://go.haigaiapp.cn

Py:   os.getcwd()
来源：http://wy.muxihuayi.cn

PHP:  getcwd();
来源：http://uv.521024.cn

JS:   process.cwd()
来源：http://zy.lnxyls.cn

TS:   process.cwd()
来源：http://yc.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://dd.hnjuh.cn

Go:   os.Getwd()
来源：http://sc.szxytkj.cn

Ruby: Dir.pwd
来源：http://rl.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pw.muxihuayi.cn

[M05] 设置退出码
来源：http://eu.huanxung.cn

Py:   sys.exit(1)
来源：http://cm.szsharing.cn

PHP:  exit(1);
来源：http://kp.bookmarksfly.cn

JS:   process.exit(1)
来源：http://wg.gzmigu.cn

TS:   process.exit(1)
来源：http://fe.colortex.cn

Java: System.exit(1)
来源：http://lm.521024.cn

Go:   os.Exit(1)
来源：http://iy.shxzskj.cn

Ruby: exit 1
来源：http://yq.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rw.bjjhwx.cn

[M06] 向标准错误输出
来源：http://ki.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://af.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sx.haigaiapp.cn

JS:   console.error("err")
来源：http://te.colortex.cn

TS:   console.error("err")
来源：http://hg.haigaiapp.cn

Java: System.err.println("err")
来源：http://od.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tl.hnjuh.cn

Ruby: warn "err"
来源：http://ez.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://et.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://xi.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://dd.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://in.chemitech.net.cn

JS:   require.main === module
来源：http://nf.gzmigu.cn

TS:   require.main === module
来源：http://fb.nszjky.cn

Java: public static void main(String[] args)
来源：http://aa.huixinmuqiang.cn

Go:   func main()
来源：http://tp.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ek.huanxung.cn

C#:   static void Main(string[] args)
来源：http://lc.521024.cn

[M08] 获取系统与运行时信息
来源：http://wy.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://pj.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://jd.9csxet.cn

JS:   process.platform;  process.version
来源：http://rr.szxytkj.cn

TS:   process.platform;  process.version
来源：http://wy.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uh.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ut.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uv.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ru.muxihuayi.cn

================================================================================
来源：http://mq.jctech888.com.cn

N. 数据结构与算法
来源：http://os.szxytkj.cn

================================================================================
来源：http://lv.asd995.cn

[N01] 二分查找（有序数组）
来源：http://bg.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cb.szxytkj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://av.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vj.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yq.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ma.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://dv.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://be.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ur.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://uj.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://iu.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zf.shxzukj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oj.huixinmuqiang.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nf.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wb.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://kt.lnxyls.cn

Ruby: arr.sort
来源：http://zx.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cr.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://kt.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cb.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://yk.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uv.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qt.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hw.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gs.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qt.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ay.9csxet.cn

[N04] 斐波那契数列
来源：http://uc.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jl.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dx.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ng.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gk.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hn.nszjky.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://is.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bc.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://md.9csxet.cn

[N05] 最大公约数
来源：http://in.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://lt.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nf.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zs.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mn.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fc.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zb.nicolike.cn

Ruby: a.gcd(b)
来源：http://hg.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nq.nszjky.cn

[N06] 判断回文字符串
来源：http://mg.huixiangedu.cn

Py:   s == s[::-1]
来源：http://kx.521024.cn

PHP:  $s === strrev($s);
来源：http://fj.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://nd.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://rn.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gw.9csxet.cn

Go:   // 双指针从两端比较
来源：http://kg.haigaiapp.cn

Ruby: s == s.reverse
来源：http://fo.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dz.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://zz.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qy.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uo.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bg.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://yp.shtwfgs.cn

Java: // 手写 HashMap
来源：http://lg.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://af.hahajie.cn

Ruby: // 手写 Hash
来源：http://de.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ix.jianghongdianzi.cn

[N08] 生成全排列
来源：http://bt.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://cx.nicolike.cn

PHP:  // 手写递归交换
来源：http://lr.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://ja.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://bm.lnxyls.cn

Java: // 手写回溯递归
来源：http://dt.9csxet.cn

Go:   // 手写回溯递归
来源：http://ge.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://yk.hnjuh.cn

C#:   // 手写回溯递归
来源：http://hm.huanxung.cn

[N09] 栈与队列
来源：http://ra.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sr.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://px.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tt.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ep.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mf.huixinmuqiang.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pe.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eo.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eq.bjjhwx.cn

[N10] 链表节点定义
来源：http://wn.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qd.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zy.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xp.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jo.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://zo.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ss.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mk.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yi.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://yu.bookmarksfly.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vr.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://fj.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://np.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oi.huixiangedu.cn

Java: // 手写递归
来源：http://yp.shxzskj.cn

Go:   // 手写递归
来源：http://bb.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://na.lnxyls.cn

C#:   // 手写递归
来源：http://uz.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sr.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kx.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wo.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eo.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sl.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yy.bookmarksfly.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yj.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nn.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uq.gzmigu.cn

================================================================================
来源：http://si.shxzskj.cn

O. 并发与异步
来源：http://cb.asd995.cn

================================================================================
来源：http://an.521024.cn

[O01] 启动一个线程
来源：http://tv.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mv.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ci.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bf.szsharing.cn

TS:   // 同 JS
来源：http://lx.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://zt.shxzukj.cn

Go:   go f()
来源：http://nt.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://vz.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://et.muxihuayi.cn

[O02] 使用线程池
来源：http://ry.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yg.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fu.nicolike.cn

JS:   // worker_threads 线程池
来源：http://bh.hahajie.cn

TS:   // worker_threads 线程池
来源：http://da.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nx.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ym.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cv.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sb.colortex.cn

[O03] 加锁保护共享数据
来源：http://lw.jianghongdianzi.cn

Py:   with lock: shared += 1
来源：http://rj.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://uc.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xu.gzmigu.cn

TS:   // 同 JS
来源：http://xq.huanxung.cn

Java: synchronized (this) { shared++; }
来源：http://wl.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nb.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fi.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://ws.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://pt.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://ia.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zh.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://mc.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yi.huixiangedu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mr.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ou.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gf.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://sr.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://uc.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://ul.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ts.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://ph.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://yb.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uf.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ee.hahajie.cn

Ruby: threads.map(&:join)
来源：http://wf.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tf.bjjhwx.cn

[O06] 使用进程池
来源：http://mr.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vz.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://so.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://ax.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://xd.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zx.huixiangedu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zi.nszjky.cn

Ruby: // fork 块
来源：http://fs.9csxet.cn

C#:   Parallel.For
来源：http://xy.huanxung.cn

================================================================================
来源：http://jz.shxzskj.cn

P. 常用工具函数
来源：http://pw.huanxung.cn

================================================================================
来源：http://ws.shxzskj.cn

[P01] 生成 UUID
来源：http://nk.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://sc.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jd.nszjky.cn

JS:   crypto.randomUUID()
来源：http://ck.nszjky.cn

TS:   crypto.randomUUID()
来源：http://gl.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://ch.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://ju.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://ff.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://lq.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://ct.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zd.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eq.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xj.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mm.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hh.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zy.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cb.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jk.shxzukj.cn

[P03] 生成短随机字符串
来源：http://cw.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://km.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mh.hahajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bk.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iq.bookmarksfly.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hv.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ah.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ty.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://my.jianghongdianzi.cn

[P04] 求长度
来源：http://vz.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://eq.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fu.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rt.nicolike.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jx.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://hd.9csxet.cn

Go:   len(arr);  len(m)
来源：http://do.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://wd.9csxet.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mv.wgjwhj.cn

[P05] 判断两个对象内容是否相等
来源：http://dt.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mo.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://py.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jo.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fy.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ny.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uc.hnjuh.cn

Ruby: a == b
来源：http://nx.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jn.bookmarksfly.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gk.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://az.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://ga.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rx.newstarts.cn

TS:   if (x == null) {}
来源：http://zl.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tx.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://nt.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ty.yuexingan06.cn

C#:   if (x is null) {}
来源：http://zf.huixiangedu.cn

[P07] 防抖与节流
来源：http://bh.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xy.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://yo.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lt.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hn.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cw.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://px.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ld.lnxyls.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ie.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://ih.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jc.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://im.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fn.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dp.lnxyls.cn


<!-- 参考信息 -->