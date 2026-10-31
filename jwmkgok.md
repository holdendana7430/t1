代发 wailian999

Py:   resp.json()
来源：http://mx.521024.cn

PHP:  json_decode($body, true);
来源：http://ar.nszjky.cn

JS:   await resp.json()
来源：http://mf.bookmarksfly.cn

TS:   await resp.json()
来源：http://da.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yf.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ar.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://um.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ln.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://kg.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wd.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://db.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://ek.asd995.cn

TS:   resp.ok;  resp.status
来源：http://gf.szxytkj.cn

Java: resp.statusCode()
来源：http://uv.colortex.cn

Go:   resp.StatusCode
来源：http://xw.shxzskj.cn

Ruby: resp.code.to_i
来源：http://hg.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://lv.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://rp.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tt.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://xt.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ji.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oe.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pd.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gg.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://af.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tr.shxzukj.cn

================================================================================
来源：http://vu.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://ge.yuntaijiaju.cn

================================================================================
来源：http://iz.szxytkj.cn

[M01] 读取命令行参数
来源：http://yd.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://uq.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://xe.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://zz.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://te.colortex.cn

Java: args 数组（main 方法参数）
来源：http://lt.muxihuayi.cn

Go:   os.Args[1:]
来源：http://ex.yuexingan06.cn

Ruby: ARGV
来源：http://zs.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://oy.shxzskj.cn

[M02] 读取环境变量
来源：http://yo.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://vb.bookmarksfly.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yb.lnxyls.cn

JS:   process.env.HOME
来源：http://ok.gzmigu.cn

TS:   process.env.HOME
来源：http://qm.521024.cn

Java: System.getenv("HOME")
来源：http://wp.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ma.newstarts.cn

Ruby: ENV["HOME"]
来源：http://pa.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yi.nszjky.cn

[M03] 执行外部命令
来源：http://ar.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kg.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ny.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wi.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nv.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ev.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ft.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ic.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://mu.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://vj.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://fi.gzmigu.cn

PHP:  getcwd();
来源：http://eu.jianghongdianzi.cn

JS:   process.cwd()
来源：http://la.haigaiapp.cn

TS:   process.cwd()
来源：http://bm.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://qq.521024.cn

Go:   os.Getwd()
来源：http://vj.shtwfgs.cn

Ruby: Dir.pwd
来源：http://bi.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ha.yuexingan06.cn

[M05] 设置退出码
来源：http://ly.yuexingan06.cn

Py:   sys.exit(1)
来源：http://bq.wgjwhj.cn

PHP:  exit(1);
来源：http://jp.yuexingan06.cn

JS:   process.exit(1)
来源：http://zm.muxihuayi.cn

TS:   process.exit(1)
来源：http://fv.wgjwhj.cn

Java: System.exit(1)
来源：http://fc.hnjuh.cn

Go:   os.Exit(1)
来源：http://sn.lnxyls.cn

Ruby: exit 1
来源：http://op.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ep.hahajie.cn

[M06] 向标准错误输出
来源：http://up.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://ah.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sh.hahajie.cn

JS:   console.error("err")
来源：http://ll.wgjwhj.cn

TS:   console.error("err")
来源：http://rv.yuexingan06.cn

Java: System.err.println("err")
来源：http://xr.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://am.nicolike.cn

Ruby: warn "err"
来源：http://ck.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://je.521024.cn

[M07] 判断是否为主入口
来源：http://hu.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://dk.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gq.colortex.cn

JS:   require.main === module
来源：http://jz.newstarts.cn

TS:   require.main === module
来源：http://jo.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://xr.panjiajie.cn

Go:   func main()
来源：http://cz.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kw.newstarts.cn

C#:   static void Main(string[] args)
来源：http://mg.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://na.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://qe.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://qz.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://kz.colortex.cn

TS:   process.platform;  process.version
来源：http://cb.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bk.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tn.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bs.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ey.muxihuayi.cn

================================================================================
来源：http://rt.jctech888.com.cn

N. 数据结构与算法
来源：http://ho.wgjwhj.cn

================================================================================
来源：http://fy.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://fy.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qe.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yw.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://so.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lq.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hy.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://hl.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zr.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fy.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://ax.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://lw.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://te.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xb.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kf.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://of.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://zg.lnxyls.cn

Ruby: arr.sort
来源：http://bc.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://va.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://xv.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://le.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://qq.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bl.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dy.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wl.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jc.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sj.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mc.huanxung.cn

[N04] 斐波那契数列
来源：http://kc.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yq.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jf.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pn.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pz.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rc.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lb.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wq.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mt.shtwfgs.cn

[N05] 最大公约数
来源：http://gm.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://tl.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yx.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://te.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iz.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ka.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tc.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://ug.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://me.hahajie.cn

[N06] 判断回文字符串
来源：http://cr.shxzukj.cn

Py:   s == s[::-1]
来源：http://jc.colortex.cn

PHP:  $s === strrev($s);
来源：http://ua.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://no.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://js.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://im.521024.cn

Go:   // 双指针从两端比较
来源：http://be.asd995.cn

Ruby: s == s.reverse
来源：http://sq.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uk.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://iz.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zr.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sg.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gs.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://xg.colortex.cn

Java: // 手写 HashMap
来源：http://rg.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://ae.szsharing.cn

Ruby: // 手写 Hash
来源：http://pq.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yp.nszjky.cn

[N08] 生成全排列
来源：http://de.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://ae.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://jq.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://ks.panjiajie.cn

TS:   // 手写回溯递归
来源：http://nf.bjjhwx.cn

Java: // 手写回溯递归
来源：http://io.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://ze.jianghongdianzi.cn

Ruby: arr.permutation.to_a
来源：http://ik.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://kb.bjjhwx.cn

[N09] 栈与队列
来源：http://na.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fp.asd995.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ch.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ay.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ns.colortex.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yl.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mn.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lw.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://br.hnjuh.cn

[N10] 链表节点定义
来源：http://ma.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gr.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bx.szxytkj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vz.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yv.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://qk.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pq.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xq.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ui.szsharing.cn

[N11] 二叉树中序遍历
来源：http://fn.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gx.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://gh.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cc.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ga.chemitech.net.cn

Java: // 手写递归
来源：http://kk.yuntaijiaju.cn

Go:   // 手写递归
来源：http://lm.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sh.hnjuh.cn

C#:   // 手写递归
来源：http://bb.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kz.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sk.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bs.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cc.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rt.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mk.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mp.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lr.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oo.jianghongdianzi.cn

================================================================================
来源：http://va.shxzskj.cn

O. 并发与异步
来源：http://pa.bookmarksfly.cn

================================================================================
来源：http://mo.521024.cn

[O01] 启动一个线程
来源：http://ah.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qt.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bq.huixinmuqiang.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ta.shxzskj.cn

TS:   // 同 JS
来源：http://cw.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://pd.jctech888.com.cn

Go:   go f()
来源：http://ei.nszjky.cn

Ruby: Thread.new { f }
来源：http://cb.szsharing.cn

C#:   Task.Run(() => F());
来源：http://jw.hnjuh.cn

[O02] 使用线程池
来源：http://oe.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hv.chemitech.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ah.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://nh.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://yr.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vb.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gx.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://or.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://na.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://tx.szxytkj.cn

Py:   with lock: shared += 1
来源：http://qe.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://rm.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ev.huixiangedu.cn

TS:   // 同 JS
来源：http://jy.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://rt.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wt.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://md.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://hv.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://vz.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://gp.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gm.hahajie.cn

JS:   async function f() { await g(); }
来源：http://qw.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dh.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oi.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yp.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://is.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://ea.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://yi.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://nf.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rp.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://po.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://fl.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vm.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ju.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://dl.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jd.huanxung.cn

[O06] 使用进程池
来源：http://vy.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ng.huanxung.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fw.colortex.cn

JS:   // child_process / cluster 模块
来源：http://qe.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://dk.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wa.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ky.yuntaijiaju.cn

Ruby: // fork 块
来源：http://eu.hnjuh.cn

C#:   Parallel.For
来源：http://le.panjiajie.cn

================================================================================
来源：http://ln.yuexingan06.cn

P. 常用工具函数
来源：http://st.huixiangedu.cn

================================================================================
来源：http://cu.jctech888.com.cn

[P01] 生成 UUID
来源：http://cv.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://wu.shxzukj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://um.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://xk.colortex.cn

TS:   crypto.randomUUID()
来源：http://fl.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://vu.huixinmuqiang.cn

Go:   // 用 github.com/google/uuid
来源：http://gi.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://nh.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://ej.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://zd.lnxyls.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gh.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qt.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uj.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zv.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://of.colortex.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wm.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dh.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nf.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://bm.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ap.hahajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ae.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jo.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fp.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ln.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yb.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vj.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qj.jianghongdianzi.cn

[P04] 求长度
来源：http://eb.haigaiapp.cn


<!-- 参考信息 -->