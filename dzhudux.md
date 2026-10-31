代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jz.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nu.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://op.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pb.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://ln.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gy.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yg.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://tn.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://mb.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://bs.newstarts.cn

Go:   resp.StatusCode
来源：http://od.szxytkj.cn

Ruby: resp.code.to_i
来源：http://qr.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://vq.colortex.cn

[L08] 并发请求多个地址
来源：http://go.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iv.521024.cn

PHP:  curl_multi_init() 系列
来源：http://av.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rr.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tx.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://es.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bc.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zq.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ld.muxihuayi.cn

================================================================================
来源：http://rq.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://qs.jctech888.com.cn

================================================================================
来源：http://xl.shxzukj.cn

[M01] 读取命令行参数
来源：http://we.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://ns.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://xp.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://gd.521024.cn

TS:   process.argv.slice(2)
来源：http://hk.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://wl.szsharing.cn

Go:   os.Args[1:]
来源：http://kd.huixiangedu.cn

Ruby: ARGV
来源：http://tp.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://st.wgjwhj.cn

[M02] 读取环境变量
来源：http://wx.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://rw.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fa.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://sa.muxihuayi.cn

TS:   process.env.HOME
来源：http://xu.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://xt.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zu.szsharing.cn

Ruby: ENV["HOME"]
来源：http://gh.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oi.hahajie.cn

[M03] 执行外部命令
来源：http://gi.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lg.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jf.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zd.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ar.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bf.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://el.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://db.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://fz.panjiajie.cn

[M04] 获取当前工作目录
来源：http://tv.shxzukj.cn

Py:   os.getcwd()
来源：http://cl.hnjuh.cn

PHP:  getcwd();
来源：http://tm.hahajie.cn

JS:   process.cwd()
来源：http://gz.521024.cn

TS:   process.cwd()
来源：http://st.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://yk.huanxung.cn

Go:   os.Getwd()
来源：http://cj.szxytkj.cn

Ruby: Dir.pwd
来源：http://ho.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fe.lnxyls.cn

[M05] 设置退出码
来源：http://uk.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://ye.haigaiapp.cn

PHP:  exit(1);
来源：http://mz.muxihuayi.cn

JS:   process.exit(1)
来源：http://hw.szxytkj.cn

TS:   process.exit(1)
来源：http://xr.yuntaijiaju.cn

Java: System.exit(1)
来源：http://no.yuexingan06.cn

Go:   os.Exit(1)
来源：http://ng.panjiajie.cn

Ruby: exit 1
来源：http://zs.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ol.shxzskj.cn

[M06] 向标准错误输出
来源：http://kh.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://hn.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cr.szxytkj.cn

JS:   console.error("err")
来源：http://rp.huanxung.cn

TS:   console.error("err")
来源：http://uw.asd995.cn

Java: System.err.println("err")
来源：http://nu.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jn.hahajie.cn

Ruby: warn "err"
来源：http://xy.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://bd.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://nr.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://rv.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yq.huixinmuqiang.cn

JS:   require.main === module
来源：http://hj.haigaiapp.cn

TS:   require.main === module
来源：http://qw.szxytkj.cn

Java: public static void main(String[] args)
来源：http://iw.hahajie.cn

Go:   func main()
来源：http://ri.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hh.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://mf.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://zj.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://wh.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://wq.hnjuh.cn

JS:   process.platform;  process.version
来源：http://zy.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://qj.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yc.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ud.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://im.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eu.yuntaijiaju.cn

================================================================================
来源：http://bg.wgjwhj.cn

N. 数据结构与算法
来源：http://ht.yuntaijiaju.cn

================================================================================
来源：http://je.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://xc.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fk.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://az.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jg.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bn.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xx.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://vb.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jp.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pg.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://gs.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://gp.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dq.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jm.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ek.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://my.hahajie.cn

Go:   slices.Sort(arr)
来源：http://un.asd995.cn

Ruby: arr.sort
来源：http://cn.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kf.yuntaijiaju.cn

[N03] 快速排序（分治示例）
来源：http://fk.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tv.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://hf.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tr.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xa.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lw.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nf.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dx.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wv.gzmigu.cn

[N04] 斐波那契数列
来源：http://dm.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jx.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pu.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wb.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kl.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wg.newstarts.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vt.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://br.muxihuayi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xk.newstarts.cn

[N05] 最大公约数
来源：http://cu.hahajie.cn

Py:   math.gcd(a, b)
来源：http://el.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mb.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qs.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://as.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cj.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ui.shxzskj.cn

Ruby: a.gcd(b)
来源：http://zg.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ad.asd995.cn

[N06] 判断回文字符串
来源：http://xb.szxytkj.cn

Py:   s == s[::-1]
来源：http://wv.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://mc.panjiajie.cn

JS:   s === [...s].reverse().join("")
来源：http://bh.wgjwhj.cn

TS:   s === [...s].reverse().join("")
来源：http://gi.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vm.colortex.cn

Go:   // 双指针从两端比较
来源：http://aq.huanxung.cn

Ruby: s == s.reverse
来源：http://tj.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qw.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://wx.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://us.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tf.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://am.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://or.panjiajie.cn

Java: // 手写 HashMap
来源：http://cs.szsharing.cn

Go:   // 手写 map[int]int
来源：http://yn.panjiajie.cn

Ruby: // 手写 Hash
来源：http://wd.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jz.haigaiapp.cn

[N08] 生成全排列
来源：http://wo.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://qt.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://pu.nszjky.cn

JS:   // 手写回溯递归
来源：http://xx.asd995.cn

TS:   // 手写回溯递归
来源：http://wl.nszjky.cn

Java: // 手写回溯递归
来源：http://to.huanxung.cn

Go:   // 手写回溯递归
来源：http://qk.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://nm.asd995.cn

C#:   // 手写回溯递归
来源：http://xo.shxzukj.cn

[N09] 栈与队列
来源：http://no.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bt.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tk.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hc.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qg.colortex.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sd.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ye.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ol.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hq.521024.cn

[N10] 链表节点定义
来源：http://xi.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://of.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://we.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lc.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ag.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://vp.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mw.huixiangedu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uo.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oc.nicolike.cn

[N11] 二叉树中序遍历
来源：http://zf.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pj.lnxyls.cn

PHP:  // 手写递归函数
来源：http://ax.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cb.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sf.gzmigu.cn

Java: // 手写递归
来源：http://ff.asd995.cn

Go:   // 手写递归
来源：http://ma.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://il.9csxet.cn

C#:   // 手写递归
来源：http://qh.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://em.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xz.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://or.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dh.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yw.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://la.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://up.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://re.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ry.shtwfgs.cn

================================================================================
来源：http://ct.szxytkj.cn

O. 并发与异步
来源：http://ow.jianghongdianzi.cn

================================================================================
来源：http://hl.bookmarksfly.cn

[O01] 启动一个线程
来源：http://al.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xf.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qk.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gq.lnxyls.cn

TS:   // 同 JS
来源：http://ot.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://jo.newstarts.cn

Go:   go f()
来源：http://cs.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://zv.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://sh.lnxyls.cn

[O02] 使用线程池
来源：http://cf.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ns.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ek.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://sg.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://zr.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://as.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://da.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aq.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vn.521024.cn

[O03] 加锁保护共享数据
来源：http://aa.9csxet.cn

Py:   with lock: shared += 1
来源：http://ev.szsharing.cn

PHP:  // 用 flock() 做文件锁
来源：http://vv.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cu.asd995.cn

TS:   // 同 JS
来源：http://dd.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://ms.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zs.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://os.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://ak.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://hz.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://mo.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yp.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://pq.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nk.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fy.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://us.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://er.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://zt.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://ti.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://ng.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wd.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://zv.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://bg.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://np.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ie.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://no.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fp.nicolike.cn

[O06] 使用进程池
来源：http://dy.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nk.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dk.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://ik.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://hg.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://se.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ze.wgjwhj.cn

Ruby: // fork 块
来源：http://ew.huanxung.cn

C#:   Parallel.For
来源：http://xs.lnxyls.cn

================================================================================
来源：http://jr.huanxung.cn

P. 常用工具函数
来源：http://pb.wgjwhj.cn

================================================================================
来源：http://kc.huanxung.cn

[P01] 生成 UUID
来源：http://xe.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://ig.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ic.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://sg.huanxung.cn

TS:   crypto.randomUUID()
来源：http://rv.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://pe.panjiajie.cn

Go:   // 用 github.com/google/uuid
来源：http://yu.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://zc.9csxet.cn

C#:   Guid.NewGuid().ToString()
来源：http://jx.szxytkj.cn

[P02] MD5 / SHA256 摘要
来源：http://yu.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ir.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tu.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bz.szsharing.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rb.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ws.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xd.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ee.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ck.nszjky.cn

[P03] 生成短随机字符串
来源：http://ip.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rq.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jc.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xf.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ui.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xx.huixinmuqiang.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gj.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gm.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gd.gzmigu.cn

[P04] 求长度
来源：http://fj.muxihuayi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bp.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xa.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://af.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zx.jctech888.com.cn


<!-- 参考信息 -->