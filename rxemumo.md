代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hk.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://qm.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zt.nicolike.cn

[M03] 执行外部命令
来源：http://wu.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ad.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ap.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rc.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wf.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hk.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cz.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xg.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://jx.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://iv.chemitech.net.cn

Py:   os.getcwd()
来源：http://ne.hnjuh.cn

PHP:  getcwd();
来源：http://va.huanxung.cn

JS:   process.cwd()
来源：http://kj.gzmigu.cn

TS:   process.cwd()
来源：http://jn.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://ng.hnjuh.cn

Go:   os.Getwd()
来源：http://ox.asd995.cn

Ruby: Dir.pwd
来源：http://vz.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gk.yuexingan06.cn

[M05] 设置退出码
来源：http://nn.szsharing.cn

Py:   sys.exit(1)
来源：http://ii.szxytkj.cn

PHP:  exit(1);
来源：http://cc.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://nr.jctech888.com.cn

TS:   process.exit(1)
来源：http://rw.nicolike.cn

Java: System.exit(1)
来源：http://pb.huanxung.cn

Go:   os.Exit(1)
来源：http://fa.szsharing.cn

Ruby: exit 1
来源：http://go.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ef.muxihuayi.cn

[M06] 向标准错误输出
来源：http://ur.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://xn.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ai.gzmigu.cn

JS:   console.error("err")
来源：http://te.lnxyls.cn

TS:   console.error("err")
来源：http://tk.haigaiapp.cn

Java: System.err.println("err")
来源：http://ps.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://js.huanxung.cn

Ruby: warn "err"
来源：http://dh.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://tw.hahajie.cn

[M07] 判断是否为主入口
来源：http://qy.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://qj.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dw.muxihuayi.cn

JS:   require.main === module
来源：http://nt.huixiangedu.cn

TS:   require.main === module
来源：http://ul.shxzukj.cn

Java: public static void main(String[] args)
来源：http://wo.newstarts.cn

Go:   func main()
来源：http://qd.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wm.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://bg.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://ek.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://gf.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://ep.hahajie.cn

JS:   process.platform;  process.version
来源：http://ub.newstarts.cn

TS:   process.platform;  process.version
来源：http://tq.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rp.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jd.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ey.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://du.newstarts.cn

================================================================================
来源：http://di.szsharing.cn

N. 数据结构与算法
来源：http://fz.521024.cn

================================================================================
来源：http://pe.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://al.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sq.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ic.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gi.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ur.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mp.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://jb.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fa.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://se.nszjky.cn

[N02] 排序（工程实践用内置实现）
来源：http://rk.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://kk.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ds.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cr.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ct.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ks.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://na.huixiangedu.cn

Ruby: arr.sort
来源：http://au.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ml.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://fl.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gs.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://ta.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tk.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ka.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://id.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zr.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dv.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rq.521024.cn

[N04] 斐波那契数列
来源：http://sb.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xp.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ro.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ck.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ko.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vu.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zc.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xw.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ym.bookmarksfly.cn

[N05] 最大公约数
来源：http://rx.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://mt.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ra.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zl.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sl.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ij.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cy.panjiajie.cn

Ruby: a.gcd(b)
来源：http://jo.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wl.colortex.cn

[N06] 判断回文字符串
来源：http://uq.szxytkj.cn

Py:   s == s[::-1]
来源：http://pw.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://og.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://ye.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://yn.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fe.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://rv.shtwfgs.cn

Ruby: s == s.reverse
来源：http://lv.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://da.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://dm.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ea.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jg.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fe.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://bp.521024.cn

Java: // 手写 HashMap
来源：http://pu.hahajie.cn

Go:   // 手写 map[int]int
来源：http://ve.haigaiapp.cn

Ruby: // 手写 Hash
来源：http://hl.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wd.wgjwhj.cn

[N08] 生成全排列
来源：http://aj.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://iu.szsharing.cn

PHP:  // 手写递归交换
来源：http://yr.huanxung.cn

JS:   // 手写回溯递归
来源：http://tw.hahajie.cn

TS:   // 手写回溯递归
来源：http://ld.hnjuh.cn

Java: // 手写回溯递归
来源：http://xb.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://ho.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://mq.521024.cn

C#:   // 手写回溯递归
来源：http://bm.haigaiapp.cn

[N09] 栈与队列
来源：http://du.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ia.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://am.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ob.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://va.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qv.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kv.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sj.szxytkj.cn

[N10] 链表节点定义
来源：http://fw.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yl.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://js.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hb.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ij.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://rh.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ai.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zp.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cx.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://ky.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jq.9csxet.cn

PHP:  // 手写递归函数
来源：http://wv.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ye.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ib.hahajie.cn

Java: // 手写递归
来源：http://br.bjjhwx.cn

Go:   // 手写递归
来源：http://zd.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nu.jianghongdianzi.cn

C#:   // 手写递归
来源：http://qk.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://is.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iq.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ye.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vv.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ax.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yg.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vt.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kd.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dw.colortex.cn

================================================================================
来源：http://ja.shtwfgs.cn

O. 并发与异步
来源：http://le.jctech888.com.cn

================================================================================
来源：http://ie.521024.cn

[O01] 启动一个线程
来源：http://ug.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vj.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://po.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zi.muxihuayi.cn

TS:   // 同 JS
来源：http://bm.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://xv.yuexingan06.cn

Go:   go f()
来源：http://kj.panjiajie.cn

Ruby: Thread.new { f }
来源：http://oq.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://am.colortex.cn

[O02] 使用线程池
来源：http://nj.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pc.shtwfgs.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oc.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://as.asd995.cn

TS:   // worker_threads 线程池
来源：http://vn.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://me.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gt.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lv.szsharing.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ax.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://sd.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://my.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://eg.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://js.huanxung.cn

TS:   // 同 JS
来源：http://ro.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://bf.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kt.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bx.521024.cn

C#:   lock (gate) { shared++; }
来源：http://cb.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://hr.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://hg.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vn.bjjhwx.cn

JS:   async function f() { await g(); }
来源：http://dv.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bx.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ub.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cr.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://av.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://bq.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://jb.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://gs.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fe.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://ll.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://kc.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zr.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ek.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://ry.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ql.colortex.cn

[O06] 使用进程池
来源：http://en.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iu.szsharing.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://or.shxzskj.cn

JS:   // child_process / cluster 模块
来源：http://lo.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://ng.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xn.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sp.nszjky.cn

Ruby: // fork 块
来源：http://cl.shxzskj.cn

C#:   Parallel.For
来源：http://pm.bjjhwx.cn

================================================================================
来源：http://vs.hnjuh.cn

P. 常用工具函数
来源：http://wf.huixinmuqiang.cn

================================================================================
来源：http://bq.newstarts.cn

[P01] 生成 UUID
来源：http://nk.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://qr.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ov.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://oj.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://es.521024.cn

Java: UUID.randomUUID().toString()
来源：http://xo.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://zz.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://lv.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://js.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://if.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://td.chemitech.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rx.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://us.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ek.521024.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gt.gzmigu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uk.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ba.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lq.szsharing.cn

[P03] 生成短随机字符串
来源：http://ke.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hk.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ha.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gb.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jr.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lq.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iz.newstarts.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jg.bookmarksfly.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://do.haigaiapp.cn

[P04] 求长度
来源：http://be.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://co.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fz.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xl.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lo.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://xy.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://rv.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://sz.newstarts.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ue.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://nv.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fc.shxzskj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mp.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zc.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ss.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iu.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://on.shxzskj.cn

Ruby: a == b
来源：http://ym.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://os.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dr.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sy.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://vq.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tf.9csxet.cn

TS:   if (x == null) {}
来源：http://ab.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vo.9csxet.cn

Go:   if x == nil {}
来源：http://op.shxzskj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xf.newstarts.cn

C#:   if (x is null) {}
来源：http://ng.yuexingan06.cn

[P07] 防抖与节流
来源：http://rh.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yw.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://js.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bp.chemitech.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ks.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qm.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ik.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zq.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cf.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://xd.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lf.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ca.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gu.nicolike.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sc.huixiangedu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nn.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zr.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sk.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rn.colortex.cn


<!-- 参考信息 -->