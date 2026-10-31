代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jz.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vm.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://op.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://op.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://kb.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://in.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://de.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://qf.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://rc.szxytkj.cn

Java: resp.statusCode()
来源：http://uw.bjjhwx.cn

Go:   resp.StatusCode
来源：http://wb.szsharing.cn

Ruby: resp.code.to_i
来源：http://sa.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://df.hnjuh.cn

[L08] 并发请求多个地址
来源：http://hb.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rw.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://ny.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ni.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rj.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yi.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ri.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yu.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ju.hnjuh.cn

================================================================================
来源：http://ua.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://nb.yuntaijiaju.cn

================================================================================
来源：http://ir.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://hm.shxzukj.cn

Py:   sys.argv[1:]
来源：http://cf.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://pl.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://dw.asd995.cn

TS:   process.argv.slice(2)
来源：http://us.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://vx.huanxung.cn

Go:   os.Args[1:]
来源：http://xp.shtwfgs.cn

Ruby: ARGV
来源：http://il.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://ae.hahajie.cn

[M02] 读取环境变量
来源：http://xe.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://vq.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://je.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://sz.newstarts.cn

TS:   process.env.HOME
来源：http://hq.huanxung.cn

Java: System.getenv("HOME")
来源：http://bq.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zi.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://rg.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fo.newstarts.cn

[M03] 执行外部命令
来源：http://xf.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://do.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ra.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xn.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xt.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cc.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hm.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uj.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://wy.521024.cn

[M04] 获取当前工作目录
来源：http://wc.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://gr.newstarts.cn

PHP:  getcwd();
来源：http://at.bookmarksfly.cn

JS:   process.cwd()
来源：http://cn.hnjuh.cn

TS:   process.cwd()
来源：http://cr.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://mj.bjjhwx.cn

Go:   os.Getwd()
来源：http://ab.wgjwhj.cn

Ruby: Dir.pwd
来源：http://ay.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sa.panjiajie.cn

[M05] 设置退出码
来源：http://fq.nicolike.cn

Py:   sys.exit(1)
来源：http://gp.shxzukj.cn

PHP:  exit(1);
来源：http://sw.shtwfgs.cn

JS:   process.exit(1)
来源：http://qy.szsharing.cn

TS:   process.exit(1)
来源：http://bu.bjjhwx.cn

Java: System.exit(1)
来源：http://zb.yuexingan06.cn

Go:   os.Exit(1)
来源：http://xu.yuexingan06.cn

Ruby: exit 1
来源：http://lk.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ps.hnjuh.cn

[M06] 向标准错误输出
来源：http://fz.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://fi.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jl.hahajie.cn

JS:   console.error("err")
来源：http://nj.lnxyls.cn

TS:   console.error("err")
来源：http://ts.szxytkj.cn

Java: System.err.println("err")
来源：http://hm.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lq.chemitech.net.cn

Ruby: warn "err"
来源：http://dd.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://nt.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://ez.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://fs.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oq.lnxyls.cn

JS:   require.main === module
来源：http://bv.newstarts.cn

TS:   require.main === module
来源：http://nd.hnjuh.cn

Java: public static void main(String[] args)
来源：http://yq.wgjwhj.cn

Go:   func main()
来源：http://ew.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gs.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://ug.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://la.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://gd.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://gu.nszjky.cn

JS:   process.platform;  process.version
来源：http://by.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://lx.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rg.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vy.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qu.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dr.nszjky.cn

================================================================================
来源：http://ic.huanxung.cn

N. 数据结构与算法
来源：http://uc.huixiangedu.cn

================================================================================
来源：http://pa.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://rn.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dm.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pu.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://co.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fq.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qu.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://va.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xh.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fd.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ec.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://wu.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wz.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jq.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ye.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vb.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://dr.szxytkj.cn

Ruby: arr.sort
来源：http://dc.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hj.521024.cn

[N03] 快速排序（分治示例）
来源：http://uj.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jm.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://rh.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lz.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ir.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ku.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ed.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yx.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tu.9csxet.cn

[N04] 斐波那契数列
来源：http://nh.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qi.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ui.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bc.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ix.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nw.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tc.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://we.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sd.nszjky.cn

[N05] 最大公约数
来源：http://ce.9csxet.cn

Py:   math.gcd(a, b)
来源：http://ns.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xm.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ev.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fs.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kz.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tm.colortex.cn

Ruby: a.gcd(b)
来源：http://qn.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ci.shxzukj.cn

[N06] 判断回文字符串
来源：http://he.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://ru.szsharing.cn

PHP:  $s === strrev($s);
来源：http://as.jctech888.com.cn

JS:   s === [...s].reverse().join("")
来源：http://cs.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://ep.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mj.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://mr.muxihuayi.cn

Ruby: s == s.reverse
来源：http://zo.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jx.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://vy.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iy.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lz.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://po.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://nl.huixiangedu.cn

Java: // 手写 HashMap
来源：http://gv.szsharing.cn

Go:   // 手写 map[int]int
来源：http://ls.colortex.cn

Ruby: // 手写 Hash
来源：http://bb.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vy.panjiajie.cn

[N08] 生成全排列
来源：http://uj.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://eo.shxzskj.cn

PHP:  // 手写递归交换
来源：http://qn.newstarts.cn

JS:   // 手写回溯递归
来源：http://zj.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://gc.haigaiapp.cn

Java: // 手写回溯递归
来源：http://ub.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://oj.jianghongdianzi.cn

Ruby: arr.permutation.to_a
来源：http://jd.hahajie.cn

C#:   // 手写回溯递归
来源：http://ax.hahajie.cn

[N09] 栈与队列
来源：http://sz.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://te.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nv.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zd.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lw.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rj.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oy.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vz.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wc.muxihuayi.cn

[N10] 链表节点定义
来源：http://xn.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://km.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://le.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dp.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cm.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://qe.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xb.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yo.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://aj.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://ad.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rw.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://uz.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jz.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dj.gzmigu.cn

Java: // 手写递归
来源：http://lk.lnxyls.cn

Go:   // 手写递归
来源：http://so.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zm.hahajie.cn

C#:   // 手写递归
来源：http://pk.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mr.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://er.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://po.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ql.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ym.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xn.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tg.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lg.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vi.szsharing.cn

================================================================================
来源：http://gw.hnjuh.cn

O. 并发与异步
来源：http://br.newstarts.cn

================================================================================
来源：http://xz.hahajie.cn

[O01] 启动一个线程
来源：http://iu.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rr.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lg.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bh.9csxet.cn

TS:   // 同 JS
来源：http://ll.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://hx.gzmigu.cn

Go:   go f()
来源：http://nm.szsharing.cn

Ruby: Thread.new { f }
来源：http://fi.szsharing.cn

C#:   Task.Run(() => F());
来源：http://vu.gzmigu.cn

[O02] 使用线程池
来源：http://lk.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gk.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://an.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://rp.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://xs.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qi.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yi.hahajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kr.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://km.hahajie.cn

[O03] 加锁保护共享数据
来源：http://lk.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://vj.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://gw.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kc.muxihuayi.cn

TS:   // 同 JS
来源：http://cn.shtwfgs.cn

Java: synchronized (this) { shared++; }
来源：http://kt.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nd.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wc.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://ci.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://cr.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://wp.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://le.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://bm.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uv.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xn.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dh.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yj.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://fy.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://vk.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://xb.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hp.521024.cn

JS:   await Promise.all(tasks)
来源：http://bh.huixiangedu.cn

TS:   await Promise.all(tasks)
来源：http://mt.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ww.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ly.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://by.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hx.9csxet.cn

[O06] 使用进程池
来源：http://dv.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gg.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hy.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://hn.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://ta.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jk.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tt.hahajie.cn

Ruby: // fork 块
来源：http://sj.chemitech.net.cn

C#:   Parallel.For
来源：http://zu.huixiangedu.cn

================================================================================
来源：http://ql.huixinmuqiang.cn

P. 常用工具函数
来源：http://sp.panjiajie.cn

================================================================================
来源：http://ej.chemitech.net.cn

[P01] 生成 UUID
来源：http://tf.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://zj.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wn.asd995.cn

JS:   crypto.randomUUID()
来源：http://bx.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://ym.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://bx.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://vg.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://wq.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://pe.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://km.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ks.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://by.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jt.szsharing.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gk.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aa.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://og.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bh.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://av.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://qt.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tn.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wi.hahajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://id.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rz.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://le.shxzskj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://en.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ot.bookmarksfly.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dl.bookmarksfly.cn

[P04] 求长度
来源：http://ko.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ap.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://om.nicolike.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://we.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cf.asd995.cn


<!-- 参考信息 -->