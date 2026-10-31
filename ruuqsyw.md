代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mp.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lf.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fy.asd995.cn

[L06] 解析响应为 JSON
来源：http://kt.lnxyls.cn

Py:   resp.json()
来源：http://bv.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://ml.521024.cn

JS:   await resp.json()
来源：http://ca.gzmigu.cn

TS:   await resp.json()
来源：http://aq.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qb.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jk.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://ia.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gb.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://gu.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mm.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ue.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://hm.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://kt.newstarts.cn

Java: resp.statusCode()
来源：http://it.shtwfgs.cn

Go:   resp.StatusCode
来源：http://br.hnjuh.cn

Ruby: resp.code.to_i
来源：http://dg.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://uh.hahajie.cn

[L08] 并发请求多个地址
来源：http://vh.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ye.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://zz.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gm.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ha.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rt.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dp.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sn.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ys.asd995.cn

================================================================================
来源：http://vr.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://ji.bookmarksfly.cn

================================================================================
来源：http://aq.szsharing.cn

[M01] 读取命令行参数
来源：http://vr.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://yf.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://ku.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://vo.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://ur.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://au.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://mc.haigaiapp.cn

Ruby: ARGV
来源：http://an.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://qm.shxzskj.cn

[M02] 读取环境变量
来源：http://oj.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://of.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lp.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://rw.szxytkj.cn

TS:   process.env.HOME
来源：http://ut.nicolike.cn

Java: System.getenv("HOME")
来源：http://fj.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vi.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://aj.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dg.chemitech.net.cn

[M03] 执行外部命令
来源：http://vt.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://go.muxihuayi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ow.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tk.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zs.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yn.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://iw.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yv.shxzukj.cn

C#:   Process.Start("ls", "-l");
来源：http://ik.lnxyls.cn

[M04] 获取当前工作目录
来源：http://yf.asd995.cn

Py:   os.getcwd()
来源：http://sy.hnjuh.cn

PHP:  getcwd();
来源：http://ma.chemitech.net.cn

JS:   process.cwd()
来源：http://iw.panjiajie.cn

TS:   process.cwd()
来源：http://dg.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://tb.muxihuayi.cn

Go:   os.Getwd()
来源：http://xq.nicolike.cn

Ruby: Dir.pwd
来源：http://gd.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hc.yuexingan06.cn

[M05] 设置退出码
来源：http://ob.haigaiapp.cn

Py:   sys.exit(1)
来源：http://mj.yuexingan06.cn

PHP:  exit(1);
来源：http://zs.chemitech.net.cn

JS:   process.exit(1)
来源：http://ww.asd995.cn

TS:   process.exit(1)
来源：http://wp.bjjhwx.cn

Java: System.exit(1)
来源：http://tl.nszjky.cn

Go:   os.Exit(1)
来源：http://zl.yuexingan06.cn

Ruby: exit 1
来源：http://wv.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cs.shtwfgs.cn

[M06] 向标准错误输出
来源：http://py.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://xe.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hk.jianghongdianzi.cn

JS:   console.error("err")
来源：http://bs.panjiajie.cn

TS:   console.error("err")
来源：http://wo.muxihuayi.cn

Java: System.err.println("err")
来源：http://hp.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://za.yuntaijiaju.cn

Ruby: warn "err"
来源：http://dx.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://yc.asd995.cn

[M07] 判断是否为主入口
来源：http://yl.asd995.cn

Py:   if __name__ == "__main__":
来源：http://ej.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kt.bookmarksfly.cn

JS:   require.main === module
来源：http://ru.bjjhwx.cn

TS:   require.main === module
来源：http://nd.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://lj.yuexingan06.cn

Go:   func main()
来源：http://zg.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wm.asd995.cn

C#:   static void Main(string[] args)
来源：http://fe.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://sc.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://dc.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://xv.colortex.cn

JS:   process.platform;  process.version
来源：http://xl.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://kw.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zv.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mq.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ip.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ee.521024.cn

================================================================================
来源：http://tr.huixinmuqiang.cn

N. 数据结构与算法
来源：http://zx.jianghongdianzi.cn

================================================================================
来源：http://pf.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://kb.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uo.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ny.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jv.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sy.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qm.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://nu.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ch.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yf.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://yj.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ht.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cf.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wq.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hd.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zv.521024.cn

Go:   slices.Sort(arr)
来源：http://cb.muxihuayi.cn

Ruby: arr.sort
来源：http://qp.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dh.asd995.cn

[N03] 快速排序（分治示例）
来源：http://hn.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vb.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://ae.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dn.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qn.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xw.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eh.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ja.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qq.haigaiapp.cn

[N04] 斐波那契数列
来源：http://ac.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tk.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fs.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bv.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zn.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fd.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://br.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ez.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://px.shxzskj.cn

[N05] 最大公约数
来源：http://iq.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://jy.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ns.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gv.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xc.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qv.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gj.gzmigu.cn

Ruby: a.gcd(b)
来源：http://pr.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ur.newstarts.cn

[N06] 判断回文字符串
来源：http://ou.shtwfgs.cn

Py:   s == s[::-1]
来源：http://oy.9csxet.cn

PHP:  $s === strrev($s);
来源：http://zc.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://so.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://sq.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://in.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://dr.9csxet.cn

Ruby: s == s.reverse
来源：http://oo.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zx.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://hc.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iw.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pr.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fn.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://jo.521024.cn

Java: // 手写 HashMap
来源：http://jf.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://tk.hahajie.cn

Ruby: // 手写 Hash
来源：http://ut.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xs.bookmarksfly.cn

[N08] 生成全排列
来源：http://mm.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://ov.lnxyls.cn

PHP:  // 手写递归交换
来源：http://gc.colortex.cn

JS:   // 手写回溯递归
来源：http://ei.colortex.cn

TS:   // 手写回溯递归
来源：http://qh.jctech888.com.cn

Java: // 手写回溯递归
来源：http://hy.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://os.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://hu.colortex.cn

C#:   // 手写回溯递归
来源：http://co.jianghongdianzi.cn

[N09] 栈与队列
来源：http://un.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yg.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://en.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mh.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://er.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://im.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hy.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ks.szsharing.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cn.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://wo.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://il.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fc.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kh.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hw.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://qe.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dg.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kt.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zq.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://gj.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wn.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://di.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ry.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zf.jianghongdianzi.cn

Java: // 手写递归
来源：http://nc.nszjky.cn

Go:   // 手写递归
来源：http://un.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ei.szsharing.cn

C#:   // 手写递归
来源：http://mr.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ng.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ph.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vm.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xq.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ku.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bl.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ue.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://im.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zl.521024.cn

================================================================================
来源：http://bq.muxihuayi.cn

O. 并发与异步
来源：http://hn.jianghongdianzi.cn

================================================================================
来源：http://ck.hnjuh.cn

[O01] 启动一个线程
来源：http://gg.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pe.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://as.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bg.bookmarksfly.cn

TS:   // 同 JS
来源：http://yh.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://jk.yuntaijiaju.cn

Go:   go f()
来源：http://gt.szsharing.cn

Ruby: Thread.new { f }
来源：http://iq.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://uf.bjjhwx.cn

[O02] 使用线程池
来源：http://fw.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vt.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wh.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://hr.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://ou.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://px.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fb.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zv.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gv.asd995.cn

[O03] 加锁保护共享数据
来源：http://fx.newstarts.cn

Py:   with lock: shared += 1
来源：http://uh.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://zz.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bt.chemitech.net.cn

TS:   // 同 JS
来源：http://gd.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://rk.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qk.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ug.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://jy.newstarts.cn

[O04] 定义异步函数并等待
来源：http://ty.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://rc.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://so.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://at.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yr.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ov.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rb.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ag.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://vu.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://lx.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://pa.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xq.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://ix.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://js.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ww.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qw.shxzskj.cn

Ruby: threads.map(&:join)
来源：http://eq.lnxyls.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bu.hahajie.cn

[O06] 使用进程池
来源：http://gn.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cv.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tt.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://ds.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://mg.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dc.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ma.yuntaijiaju.cn

Ruby: // fork 块
来源：http://tn.9csxet.cn

C#:   Parallel.For
来源：http://uk.huixinmuqiang.cn

================================================================================
来源：http://ad.hnjuh.cn

P. 常用工具函数
来源：http://ml.bjjhwx.cn

================================================================================
来源：http://jg.jctech888.com.cn

[P01] 生成 UUID
来源：http://jr.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://sa.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pr.szsharing.cn

JS:   crypto.randomUUID()
来源：http://jt.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://ob.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://ni.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://sf.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://vi.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://ae.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://nw.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sk.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://va.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ba.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rp.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tp.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ba.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ay.hahajie.cn

[P03] 生成短随机字符串
来源：http://wj.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mj.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xv.gzmigu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lf.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mj.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ur.jianghongdianzi.cn


<!-- 参考信息 -->