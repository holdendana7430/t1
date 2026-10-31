代发 wailian999

Py:   resp.json()
来源：http://yj.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://ae.panjiajie.cn

JS:   await resp.json()
来源：http://uh.panjiajie.cn

TS:   await resp.json()
来源：http://qv.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jl.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nf.asd995.cn

Ruby: JSON.parse(resp.body)
来源：http://jj.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zw.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://mx.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wf.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ts.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://ml.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://bn.jctech888.com.cn

Java: resp.statusCode()
来源：http://hf.chemitech.net.cn

Go:   resp.StatusCode
来源：http://mx.hnjuh.cn

Ruby: resp.code.to_i
来源：http://xk.colortex.cn

C#:   (int)resp.StatusCode
来源：http://xl.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://wa.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zn.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://bo.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://un.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tl.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gt.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rc.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cy.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eb.panjiajie.cn

================================================================================
来源：http://jh.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://ox.panjiajie.cn

================================================================================
来源：http://kt.nicolike.cn

[M01] 读取命令行参数
来源：http://qq.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://nw.asd995.cn

PHP:  $argv;  $argc;
来源：http://oh.hahajie.cn

JS:   process.argv.slice(2)
来源：http://eh.asd995.cn

TS:   process.argv.slice(2)
来源：http://ca.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://av.huixinmuqiang.cn

Go:   os.Args[1:]
来源：http://pb.9csxet.cn

Ruby: ARGV
来源：http://yu.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://gv.huanxung.cn

[M02] 读取环境变量
来源：http://nf.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://xc.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hl.haigaiapp.cn

JS:   process.env.HOME
来源：http://rt.nszjky.cn

TS:   process.env.HOME
来源：http://oq.newstarts.cn

Java: System.getenv("HOME")
来源：http://il.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bo.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://yv.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ug.shtwfgs.cn

[M03] 执行外部命令
来源：http://yf.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://es.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cb.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dp.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ol.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ke.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bg.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nx.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://ud.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://uv.nszjky.cn

Py:   os.getcwd()
来源：http://jv.lnxyls.cn

PHP:  getcwd();
来源：http://yo.9csxet.cn

JS:   process.cwd()
来源：http://cl.nicolike.cn

TS:   process.cwd()
来源：http://ak.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://vj.huanxung.cn

Go:   os.Getwd()
来源：http://fa.newstarts.cn

Ruby: Dir.pwd
来源：http://nq.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lz.jctech888.com.cn

[M05] 设置退出码
来源：http://rb.gzmigu.cn

Py:   sys.exit(1)
来源：http://th.huixiangedu.cn

PHP:  exit(1);
来源：http://xf.yuexingan06.cn

JS:   process.exit(1)
来源：http://nn.szxytkj.cn

TS:   process.exit(1)
来源：http://ck.hnjuh.cn

Java: System.exit(1)
来源：http://vd.newstarts.cn

Go:   os.Exit(1)
来源：http://fl.shxzskj.cn

Ruby: exit 1
来源：http://wa.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tk.muxihuayi.cn

[M06] 向标准错误输出
来源：http://xm.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://gm.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://th.haigaiapp.cn

JS:   console.error("err")
来源：http://yz.hnjuh.cn

TS:   console.error("err")
来源：http://uf.nicolike.cn

Java: System.err.println("err")
来源：http://jk.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hj.huixinmuqiang.cn

Ruby: warn "err"
来源：http://ul.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://ao.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://nz.asd995.cn

Py:   if __name__ == "__main__":
来源：http://or.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gd.yuexingan06.cn

JS:   require.main === module
来源：http://mq.yuexingan06.cn

TS:   require.main === module
来源：http://na.newstarts.cn

Java: public static void main(String[] args)
来源：http://ej.colortex.cn

Go:   func main()
来源：http://xu.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qv.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://ki.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://ni.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://ay.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://vy.huanxung.cn

JS:   process.platform;  process.version
来源：http://tb.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://wd.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://id.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gj.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lv.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tz.huixiangedu.cn

================================================================================
来源：http://wf.shtwfgs.cn

N. 数据结构与算法
来源：http://qx.521024.cn

================================================================================
来源：http://ed.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://tr.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ze.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gp.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tp.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ie.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yz.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://qg.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dc.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bp.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://wi.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://pq.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ac.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gm.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cg.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ln.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://qb.newstarts.cn

Ruby: arr.sort
来源：http://vd.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://av.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://rk.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://du.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://yu.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wu.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tc.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yi.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fk.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gn.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mj.gzmigu.cn

[N04] 斐波那契数列
来源：http://ck.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cu.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ow.yuexingan06.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zw.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pk.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://po.nszjky.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jx.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sf.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yw.shtwfgs.cn

[N05] 最大公约数
来源：http://bg.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://dn.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iw.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://we.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xa.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wg.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pw.asd995.cn

Ruby: a.gcd(b)
来源：http://xt.521024.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nh.shxzukj.cn

[N06] 判断回文字符串
来源：http://qq.bjjhwx.cn

Py:   s == s[::-1]
来源：http://lf.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://xm.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://lz.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://tx.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vo.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://nr.szxytkj.cn

Ruby: s == s.reverse
来源：http://bk.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kg.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://me.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ra.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pa.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sk.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://xz.shxzukj.cn

Java: // 手写 HashMap
来源：http://qy.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://xf.hnjuh.cn

Ruby: // 手写 Hash
来源：http://vr.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hl.jctech888.com.cn

[N08] 生成全排列
来源：http://ig.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://fl.szxytkj.cn

PHP:  // 手写递归交换
来源：http://oq.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://wy.yuexingan06.cn

TS:   // 手写回溯递归
来源：http://cz.gzmigu.cn

Java: // 手写回溯递归
来源：http://ta.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://xg.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://yl.szsharing.cn

C#:   // 手写回溯递归
来源：http://sx.gzmigu.cn

[N09] 栈与队列
来源：http://jy.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oz.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ux.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rn.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zt.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lj.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oy.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://in.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qe.nszjky.cn

[N10] 链表节点定义
来源：http://fw.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://km.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mx.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ce.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wv.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://cq.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fx.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qm.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ai.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://ek.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jr.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://bw.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ko.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ky.asd995.cn

Java: // 手写递归
来源：http://qs.muxihuayi.cn

Go:   // 手写递归
来源：http://ig.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kv.yuexingan06.cn

C#:   // 手写递归
来源：http://ru.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jg.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xz.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://en.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qh.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ch.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cn.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xs.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hs.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qh.nicolike.cn

================================================================================
来源：http://uf.bjjhwx.cn

O. 并发与异步
来源：http://kv.colortex.cn

================================================================================
来源：http://jx.shxzukj.cn

[O01] 启动一个线程
来源：http://sc.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gu.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ws.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://br.wgjwhj.cn

TS:   // 同 JS
来源：http://fw.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://qv.szxytkj.cn

Go:   go f()
来源：http://ka.nszjky.cn

Ruby: Thread.new { f }
来源：http://uz.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://zm.lnxyls.cn

[O02] 使用线程池
来源：http://kd.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cf.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yo.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://vf.huanxung.cn

TS:   // worker_threads 线程池
来源：http://zh.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zc.gzmigu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xc.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dd.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zu.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://ds.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://ia.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://mf.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ud.521024.cn

TS:   // 同 JS
来源：http://in.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://uv.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eb.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://iy.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://mc.nszjky.cn

[O04] 定义异步函数并等待
来源：http://tv.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://pk.nicolike.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hg.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://it.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fi.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hp.wgjwhj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sf.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://aw.colortex.cn

C#:   async Task F() { await G(); }
来源：http://gt.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://ch.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://ff.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vi.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://df.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://sv.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gx.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mh.colortex.cn

Ruby: threads.map(&:join)
来源：http://zv.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://il.szxytkj.cn

[O06] 使用进程池
来源：http://yr.shxzskj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hp.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kd.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://lf.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://pc.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cn.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ay.521024.cn

Ruby: // fork 块
来源：http://qa.panjiajie.cn

C#:   Parallel.For
来源：http://pz.chemitech.net.cn

================================================================================
来源：http://db.gzmigu.cn

P. 常用工具函数
来源：http://jt.jianghongdianzi.cn

================================================================================
来源：http://cl.yuntaijiaju.cn

[P01] 生成 UUID
来源：http://nt.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://wx.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jh.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://fp.9csxet.cn

TS:   crypto.randomUUID()
来源：http://pp.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://aq.shtwfgs.cn

Go:   // 用 github.com/google/uuid
来源：http://bv.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://tf.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://ko.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://yh.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vq.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jq.asd995.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vw.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ws.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://px.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ln.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tg.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dt.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://fs.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://so.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sr.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wd.wgjwhj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dm.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wy.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://um.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mz.yuexingan06.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://il.szxytkj.cn

[P04] 求长度
来源：http://um.bjjhwx.cn


<!-- 参考信息 -->