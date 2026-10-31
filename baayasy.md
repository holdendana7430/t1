代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sk.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qd.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tm.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ju.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ye.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zj.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ol.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://ba.shxzskj.cn

[M04] 获取当前工作目录
来源：http://jy.lnxyls.cn

Py:   os.getcwd()
来源：http://ln.gzmigu.cn

PHP:  getcwd();
来源：http://qx.hnjuh.cn

JS:   process.cwd()
来源：http://du.wgjwhj.cn

TS:   process.cwd()
来源：http://bv.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://yd.521024.cn

Go:   os.Getwd()
来源：http://pg.colortex.cn

Ruby: Dir.pwd
来源：http://dw.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wy.shxzukj.cn

[M05] 设置退出码
来源：http://es.muxihuayi.cn

Py:   sys.exit(1)
来源：http://jw.chemitech.net.cn

PHP:  exit(1);
来源：http://jm.lnxyls.cn

JS:   process.exit(1)
来源：http://ip.shtwfgs.cn

TS:   process.exit(1)
来源：http://cr.huixinmuqiang.cn

Java: System.exit(1)
来源：http://za.haigaiapp.cn

Go:   os.Exit(1)
来源：http://za.nszjky.cn

Ruby: exit 1
来源：http://ko.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://if.szsharing.cn

[M06] 向标准错误输出
来源：http://zu.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://qc.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://oe.521024.cn

JS:   console.error("err")
来源：http://jg.hahajie.cn

TS:   console.error("err")
来源：http://xo.jctech888.com.cn

Java: System.err.println("err")
来源：http://rr.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zk.lnxyls.cn

Ruby: warn "err"
来源：http://lf.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://vs.gzmigu.cn

[M07] 判断是否为主入口
来源：http://eq.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://ot.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gg.nszjky.cn

JS:   require.main === module
来源：http://kg.jctech888.com.cn

TS:   require.main === module
来源：http://vx.shxzukj.cn

Java: public static void main(String[] args)
来源：http://gn.nicolike.cn

Go:   func main()
来源：http://uz.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nb.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://eb.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://np.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://wx.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://bh.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://jb.panjiajie.cn

TS:   process.platform;  process.version
来源：http://re.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gj.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ph.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ug.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kh.521024.cn

================================================================================
来源：http://bv.hnjuh.cn

N. 数据结构与算法
来源：http://pm.hahajie.cn

================================================================================
来源：http://eq.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://fv.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uc.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jy.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rz.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ba.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ow.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://bj.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qu.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kk.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://sj.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://zo.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ml.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dq.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ca.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zg.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://wk.huanxung.cn

Ruby: arr.sort
来源：http://yc.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nq.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://go.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uj.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://bi.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://el.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xq.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tl.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ry.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tx.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xu.9csxet.cn

[N04] 斐波那契数列
来源：http://ed.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jy.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fc.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bs.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ym.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ox.newstarts.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sb.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rs.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ds.wgjwhj.cn

[N05] 最大公约数
来源：http://xx.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://oc.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lq.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://id.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ov.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cc.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pp.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://kf.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ct.gzmigu.cn

[N06] 判断回文字符串
来源：http://uw.chemitech.net.cn

Py:   s == s[::-1]
来源：http://xc.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://bg.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://om.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://oh.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://um.asd995.cn

Go:   // 双指针从两端比较
来源：http://hg.huixiangedu.cn

Ruby: s == s.reverse
来源：http://sm.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kd.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://iw.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://us.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ys.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cr.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://ux.shxzukj.cn

Java: // 手写 HashMap
来源：http://qw.colortex.cn

Go:   // 手写 map[int]int
来源：http://qy.hahajie.cn

Ruby: // 手写 Hash
来源：http://yv.szxytkj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yf.bjjhwx.cn

[N08] 生成全排列
来源：http://dg.jianghongdianzi.cn

Py:   itertools.permutations(arr)
来源：http://yi.newstarts.cn

PHP:  // 手写递归交换
来源：http://gi.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://op.hahajie.cn

TS:   // 手写回溯递归
来源：http://sj.muxihuayi.cn

Java: // 手写回溯递归
来源：http://bt.hnjuh.cn

Go:   // 手写回溯递归
来源：http://lx.shxzskj.cn

Ruby: arr.permutation.to_a
来源：http://bw.panjiajie.cn

C#:   // 手写回溯递归
来源：http://nj.newstarts.cn

[N09] 栈与队列
来源：http://qy.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bq.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wx.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hi.shxzskj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xu.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dd.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rb.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yb.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lz.hahajie.cn

[N10] 链表节点定义
来源：http://ae.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jf.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zs.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cg.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rr.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://sj.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gi.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sa.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qt.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://da.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vf.colortex.cn

PHP:  // 手写递归函数
来源：http://go.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ow.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nl.shxzskj.cn

Java: // 手写递归
来源：http://bk.lnxyls.cn

Go:   // 手写递归
来源：http://id.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ok.yuexingan06.cn

C#:   // 手写递归
来源：http://nt.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sk.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fp.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jr.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ek.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rr.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tb.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vw.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pc.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vz.haigaiapp.cn

================================================================================
来源：http://ne.huanxung.cn

O. 并发与异步
来源：http://rq.asd995.cn

================================================================================
来源：http://gb.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://dm.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wk.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qk.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://le.chemitech.net.cn

TS:   // 同 JS
来源：http://ug.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://bg.muxihuayi.cn

Go:   go f()
来源：http://ts.panjiajie.cn

Ruby: Thread.new { f }
来源：http://am.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://zt.haigaiapp.cn

[O02] 使用线程池
来源：http://qf.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pl.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zc.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://nw.panjiajie.cn

TS:   // worker_threads 线程池
来源：http://eg.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ov.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rt.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gh.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ts.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://fz.huanxung.cn

Py:   with lock: shared += 1
来源：http://lh.shxzukj.cn

PHP:  // 用 flock() 做文件锁
来源：http://bv.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bb.huanxung.cn

TS:   // 同 JS
来源：http://pd.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://fi.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://se.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bf.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://ob.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://ng.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://ef.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tt.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://nn.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ny.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pb.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yl.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mn.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://qh.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://eb.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://dq.muxihuayi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ks.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://uq.shtwfgs.cn

TS:   await Promise.all(tasks)
来源：http://cf.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ye.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tk.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://zp.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pj.shxzskj.cn

[O06] 使用进程池
来源：http://zv.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zu.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dl.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://yv.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://ww.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pf.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yg.nszjky.cn

Ruby: // fork 块
来源：http://cj.szsharing.cn

C#:   Parallel.For
来源：http://pm.huixiangedu.cn

================================================================================
来源：http://jq.szsharing.cn

P. 常用工具函数
来源：http://ij.newstarts.cn

================================================================================
来源：http://eq.shtwfgs.cn

[P01] 生成 UUID
来源：http://oh.shxzukj.cn

Py:   str(uuid.uuid4())
来源：http://rb.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rj.nicolike.cn

JS:   crypto.randomUUID()
来源：http://rx.asd995.cn

TS:   crypto.randomUUID()
来源：http://kx.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://nw.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://wa.shtwfgs.cn

Ruby: SecureRandom.uuid
来源：http://bf.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://vc.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://ya.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mu.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jr.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sk.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bk.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uq.shxzukj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fb.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eg.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hn.gzmigu.cn

[P03] 生成短随机字符串
来源：http://ex.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nz.chemitech.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wb.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rq.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uo.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gh.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://om.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://db.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jb.asd995.cn

[P04] 求长度
来源：http://wc.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tb.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ky.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rw.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://id.asd995.cn

Java: list.size();  map.size();  s.length()
来源：http://sb.newstarts.cn

Go:   len(arr);  len(m)
来源：http://lt.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://do.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wy.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://tp.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ey.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cm.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wx.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ts.nszjky.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ar.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pu.colortex.cn

Ruby: a == b
来源：http://hh.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ev.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dl.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ol.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://gd.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://of.huixiangedu.cn

TS:   if (x == null) {}
来源：http://gd.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tz.wgjwhj.cn

Go:   if x == nil {}
来源：http://eg.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://td.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://ez.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://ix.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bl.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://xt.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lk.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pf.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ds.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ki.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jd.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xf.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://cd.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gx.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://il.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nk.nicolike.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yc.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://js.jianghongdianzi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nj.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://va.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bt.huixiangedu.cn

================================================================================
来源：http://nl.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pa.wgjwhj.cn

================================================================================
来源：http://eb.jctech888.com.cn

[Q01] 创建表
来源：http://if.gzmigu.cn


<!-- 参考信息 -->