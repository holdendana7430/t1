代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cn.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oi.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://at.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://fn.yuexingan06.cn

Py:   resp.json()
来源：http://wz.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://yd.bookmarksfly.cn

JS:   await resp.json()
来源：http://mx.hahajie.cn

TS:   await resp.json()
来源：http://db.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wz.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xz.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://rw.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hg.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://mr.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gz.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://io.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://ed.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://bi.panjiajie.cn

Java: resp.statusCode()
来源：http://dk.szxytkj.cn

Go:   resp.StatusCode
来源：http://qn.huanxung.cn

Ruby: resp.code.to_i
来源：http://ly.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://nn.colortex.cn

[L08] 并发请求多个地址
来源：http://co.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oq.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://fi.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mp.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yt.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hi.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ge.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sx.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xu.wgjwhj.cn

================================================================================
来源：http://mr.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://wx.gzmigu.cn

================================================================================
来源：http://yw.nicolike.cn

[M01] 读取命令行参数
来源：http://ro.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://re.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://ba.huanxung.cn

JS:   process.argv.slice(2)
来源：http://hv.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://hj.521024.cn

Java: args 数组（main 方法参数）
来源：http://aw.wgjwhj.cn

Go:   os.Args[1:]
来源：http://sm.bjjhwx.cn

Ruby: ARGV
来源：http://nb.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://nh.nszjky.cn

[M02] 读取环境变量
来源：http://di.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://vi.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ik.521024.cn

JS:   process.env.HOME
来源：http://wx.shtwfgs.cn

TS:   process.env.HOME
来源：http://wt.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://vj.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://au.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://ya.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ki.nicolike.cn

[M03] 执行外部命令
来源：http://ny.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cf.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xw.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ca.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jo.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://da.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://oo.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oe.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://nt.szsharing.cn

[M04] 获取当前工作目录
来源：http://ki.bookmarksfly.cn

Py:   os.getcwd()
来源：http://mr.nszjky.cn

PHP:  getcwd();
来源：http://rh.bjjhwx.cn

JS:   process.cwd()
来源：http://rg.colortex.cn

TS:   process.cwd()
来源：http://sp.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://yh.nszjky.cn

Go:   os.Getwd()
来源：http://io.haigaiapp.cn

Ruby: Dir.pwd
来源：http://uz.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xp.haigaiapp.cn

[M05] 设置退出码
来源：http://cx.haigaiapp.cn

Py:   sys.exit(1)
来源：http://sa.newstarts.cn

PHP:  exit(1);
来源：http://vp.521024.cn

JS:   process.exit(1)
来源：http://lw.shxzskj.cn

TS:   process.exit(1)
来源：http://kk.hnjuh.cn

Java: System.exit(1)
来源：http://os.9csxet.cn

Go:   os.Exit(1)
来源：http://ua.panjiajie.cn

Ruby: exit 1
来源：http://hu.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bx.colortex.cn

[M06] 向标准错误输出
来源：http://ng.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://na.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://og.asd995.cn

JS:   console.error("err")
来源：http://zl.nszjky.cn

TS:   console.error("err")
来源：http://kn.521024.cn

Java: System.err.println("err")
来源：http://gy.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mz.szxytkj.cn

Ruby: warn "err"
来源：http://nu.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://gk.lnxyls.cn

[M07] 判断是否为主入口
来源：http://nl.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://ni.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wy.nszjky.cn

JS:   require.main === module
来源：http://lg.nicolike.cn

TS:   require.main === module
来源：http://nj.lnxyls.cn

Java: public static void main(String[] args)
来源：http://ku.hahajie.cn

Go:   func main()
来源：http://rp.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xk.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://vs.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://kg.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://ft.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://nk.lnxyls.cn

JS:   process.platform;  process.version
来源：http://av.nicolike.cn

TS:   process.platform;  process.version
来源：http://ce.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qg.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://is.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rj.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dl.jianghongdianzi.cn

================================================================================
来源：http://qu.521024.cn

N. 数据结构与算法
来源：http://ma.szxytkj.cn

================================================================================
来源：http://iv.colortex.cn

[N01] 二分查找（有序数组）
来源：http://qg.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uc.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fp.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rg.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dn.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pg.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://sf.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rv.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lf.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://we.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://fi.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://un.shxzukj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://se.huixinmuqiang.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cz.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ce.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://ax.9csxet.cn

Ruby: arr.sort
来源：http://ld.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://on.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://nu.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ni.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://lg.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wb.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://da.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xy.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rb.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fh.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://py.colortex.cn

[N04] 斐波那契数列
来源：http://ss.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vv.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cl.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mp.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rj.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sa.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zw.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://px.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pg.szsharing.cn

[N05] 最大公约数
来源：http://fz.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://jg.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xx.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rx.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oz.yuexingan06.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dm.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qc.hahajie.cn

Ruby: a.gcd(b)
来源：http://du.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lx.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://mk.bjjhwx.cn

Py:   s == s[::-1]
来源：http://yo.colortex.cn

PHP:  $s === strrev($s);
来源：http://bs.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://bb.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://fw.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qq.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://zf.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://rc.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rl.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://zd.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://to.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vw.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dr.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://nk.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://gi.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://mu.colortex.cn

Ruby: // 手写 Hash
来源：http://mo.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nc.bjjhwx.cn

[N08] 生成全排列
来源：http://cs.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://li.panjiajie.cn

PHP:  // 手写递归交换
来源：http://ya.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://rc.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://zr.gzmigu.cn

Java: // 手写回溯递归
来源：http://ct.9csxet.cn

Go:   // 手写回溯递归
来源：http://fp.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://xa.shxzukj.cn

C#:   // 手写回溯递归
来源：http://tf.nicolike.cn

[N09] 栈与队列
来源：http://pc.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ps.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hl.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hp.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zr.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ie.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vd.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://by.colortex.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://st.hnjuh.cn

[N10] 链表节点定义
来源：http://nn.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hs.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zk.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ec.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lg.szxytkj.cn

Java: class Node { int v; Node next; }
来源：http://tm.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nu.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hh.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qq.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://pe.lnxyls.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zi.huanxung.cn

PHP:  // 手写递归函数
来源：http://xp.521024.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ba.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lf.panjiajie.cn

Java: // 手写递归
来源：http://yw.asd995.cn

Go:   // 手写递归
来源：http://wf.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uz.shxzskj.cn

C#:   // 手写递归
来源：http://zw.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://so.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jr.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ac.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hd.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ol.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ox.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ac.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lq.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ab.521024.cn

================================================================================
来源：http://hi.shxzskj.cn

O. 并发与异步
来源：http://qu.newstarts.cn

================================================================================
来源：http://bc.shxzskj.cn

[O01] 启动一个线程
来源：http://wp.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dc.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bl.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ss.hahajie.cn

TS:   // 同 JS
来源：http://la.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://zt.yuexingan06.cn

Go:   go f()
来源：http://wv.gzmigu.cn

Ruby: Thread.new { f }
来源：http://tf.nszjky.cn

C#:   Task.Run(() => F());
来源：http://eu.9csxet.cn

[O02] 使用线程池
来源：http://xs.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xi.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ue.nszjky.cn

JS:   // worker_threads 线程池
来源：http://nj.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://oh.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://em.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xm.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ds.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uf.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://eh.newstarts.cn

Py:   with lock: shared += 1
来源：http://oy.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://zb.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gb.lnxyls.cn

TS:   // 同 JS
来源：http://ig.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://iw.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ew.muxihuayi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kp.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://df.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://va.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://nk.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dc.nszjky.cn

JS:   async function f() { await g(); }
来源：http://fw.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hj.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://id.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ar.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hy.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://eo.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://yt.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://jl.muxihuayi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qv.asd995.cn

JS:   await Promise.all(tasks)
来源：http://nc.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://uq.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iq.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xp.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://il.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nl.shtwfgs.cn

[O06] 使用进程池
来源：http://an.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hu.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qb.huanxung.cn

JS:   // child_process / cluster 模块
来源：http://jw.bookmarksfly.cn

TS:   // child_process / cluster 模块
来源：http://dv.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lw.haigaiapp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lk.lnxyls.cn

Ruby: // fork 块
来源：http://wl.jianghongdianzi.cn

C#:   Parallel.For
来源：http://np.asd995.cn

================================================================================
来源：http://kn.shxzskj.cn

P. 常用工具函数
来源：http://xd.gzmigu.cn

================================================================================
来源：http://ni.521024.cn

[P01] 生成 UUID
来源：http://cb.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://gs.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tu.asd995.cn

JS:   crypto.randomUUID()
来源：http://fw.nicolike.cn

TS:   crypto.randomUUID()
来源：http://ed.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://du.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://wy.asd995.cn

Ruby: SecureRandom.uuid
来源：http://vh.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://ub.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://ah.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pq.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ht.521024.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pz.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ii.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qu.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hh.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cd.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pk.nszjky.cn

[P03] 生成短随机字符串
来源：http://yk.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ww.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mm.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zm.shtwfgs.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ck.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ah.nicolike.cn


<!-- 参考信息 -->