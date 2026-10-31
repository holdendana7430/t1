代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jy.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qk.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ya.colortex.cn

[L06] 解析响应为 JSON
来源：http://hn.newstarts.cn

Py:   resp.json()
来源：http://hs.hahajie.cn

PHP:  json_decode($body, true);
来源：http://jm.nszjky.cn

JS:   await resp.json()
来源：http://kf.bookmarksfly.cn

TS:   await resp.json()
来源：http://aq.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hk.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aq.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://nf.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eg.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://ab.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hv.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://su.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://tb.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://sf.shtwfgs.cn

Java: resp.statusCode()
来源：http://lj.szsharing.cn

Go:   resp.StatusCode
来源：http://kp.nszjky.cn

Ruby: resp.code.to_i
来源：http://aq.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://mj.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://ab.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dt.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://ep.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ay.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iy.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nl.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://md.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hp.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jk.chemitech.net.cn

================================================================================
来源：http://re.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://dr.shxzskj.cn

================================================================================
来源：http://dq.9csxet.cn

[M01] 读取命令行参数
来源：http://xp.shxzukj.cn

Py:   sys.argv[1:]
来源：http://mi.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://rm.huanxung.cn

JS:   process.argv.slice(2)
来源：http://ag.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://wu.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://gz.shxzskj.cn

Go:   os.Args[1:]
来源：http://re.szsharing.cn

Ruby: ARGV
来源：http://ee.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://np.muxihuayi.cn

[M02] 读取环境变量
来源：http://ey.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://ou.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zm.muxihuayi.cn

JS:   process.env.HOME
来源：http://iu.asd995.cn

TS:   process.env.HOME
来源：http://hu.shxzukj.cn

Java: System.getenv("HOME")
来源：http://za.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pv.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://jb.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lx.shxzskj.cn

[M03] 执行外部命令
来源：http://ir.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://se.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uk.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://md.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xy.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ow.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rf.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nf.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://cv.colortex.cn

[M04] 获取当前工作目录
来源：http://wx.jctech888.com.cn

Py:   os.getcwd()
来源：http://xm.jianghongdianzi.cn

PHP:  getcwd();
来源：http://ml.lnxyls.cn

JS:   process.cwd()
来源：http://tk.huixinmuqiang.cn

TS:   process.cwd()
来源：http://ot.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://ws.huixiangedu.cn

Go:   os.Getwd()
来源：http://qj.hnjuh.cn

Ruby: Dir.pwd
来源：http://io.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xu.shtwfgs.cn

[M05] 设置退出码
来源：http://qy.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://kj.bookmarksfly.cn

PHP:  exit(1);
来源：http://zo.jctech888.com.cn

JS:   process.exit(1)
来源：http://dr.lnxyls.cn

TS:   process.exit(1)
来源：http://pn.muxihuayi.cn

Java: System.exit(1)
来源：http://rb.gzmigu.cn

Go:   os.Exit(1)
来源：http://qz.hnjuh.cn

Ruby: exit 1
来源：http://wp.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qb.asd995.cn

[M06] 向标准错误输出
来源：http://hf.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://rg.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zf.asd995.cn

JS:   console.error("err")
来源：http://vd.shtwfgs.cn

TS:   console.error("err")
来源：http://py.colortex.cn

Java: System.err.println("err")
来源：http://bc.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vv.yuntaijiaju.cn

Ruby: warn "err"
来源：http://yl.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://ri.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://uu.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://cl.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yo.lnxyls.cn

JS:   require.main === module
来源：http://gk.lnxyls.cn

TS:   require.main === module
来源：http://ll.shxzskj.cn

Java: public static void main(String[] args)
来源：http://nz.yuntaijiaju.cn

Go:   func main()
来源：http://xg.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lw.colortex.cn

C#:   static void Main(string[] args)
来源：http://ja.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://mw.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://xj.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://nc.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://ox.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://nt.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vk.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yw.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://go.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fs.521024.cn

================================================================================
来源：http://vi.newstarts.cn

N. 数据结构与算法
来源：http://lp.muxihuayi.cn

================================================================================
来源：http://gi.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://tb.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cm.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pc.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wq.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://if.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://am.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://dq.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ot.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fd.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://gr.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://jv.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://if.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tk.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yn.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://di.521024.cn

Go:   slices.Sort(arr)
来源：http://aj.huanxung.cn

Ruby: arr.sort
来源：http://tp.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vi.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://xg.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kn.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://pa.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rl.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ny.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bo.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://au.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pc.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sr.gzmigu.cn

[N04] 斐波那契数列
来源：http://xr.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qf.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pi.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hy.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mq.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bb.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lo.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wy.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://op.jianghongdianzi.cn

[N05] 最大公约数
来源：http://ak.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://ur.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kn.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://um.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://am.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://be.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://th.lnxyls.cn

Ruby: a.gcd(b)
来源：http://wk.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qx.huixiangedu.cn

[N06] 判断回文字符串
来源：http://gx.chemitech.net.cn

Py:   s == s[::-1]
来源：http://hw.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://gk.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://nw.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://wm.wgjwhj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vn.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://mq.huanxung.cn

Ruby: s == s.reverse
来源：http://xs.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qi.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://qt.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ae.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gq.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xq.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://jt.shtwfgs.cn

Java: // 手写 HashMap
来源：http://gf.huanxung.cn

Go:   // 手写 map[int]int
来源：http://mn.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://hc.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ct.shtwfgs.cn

[N08] 生成全排列
来源：http://vb.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://sg.asd995.cn

PHP:  // 手写递归交换
来源：http://aj.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://kv.szsharing.cn

TS:   // 手写回溯递归
来源：http://pq.szxytkj.cn

Java: // 手写回溯递归
来源：http://ut.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://ns.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://rd.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://au.colortex.cn

[N09] 栈与队列
来源：http://kz.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gh.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://db.bjjhwx.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ef.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://je.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ej.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uz.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gf.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zw.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://lc.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ek.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kw.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bd.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lw.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://bb.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hz.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xz.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cv.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://fw.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dq.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://fd.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pl.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jd.chemitech.net.cn

Java: // 手写递归
来源：http://kn.hahajie.cn

Go:   // 手写递归
来源：http://wx.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eo.haigaiapp.cn

C#:   // 手写递归
来源：http://rv.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gg.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kz.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zx.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dx.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wy.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mj.bjjhwx.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://al.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hu.haigaiapp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uj.nszjky.cn

================================================================================
来源：http://ql.521024.cn

O. 并发与异步
来源：http://kp.9csxet.cn

================================================================================
来源：http://xo.yuexingan06.cn

[O01] 启动一个线程
来源：http://gt.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vd.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ey.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ki.huanxung.cn

TS:   // 同 JS
来源：http://gk.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://rn.jianghongdianzi.cn

Go:   go f()
来源：http://vh.huanxung.cn

Ruby: Thread.new { f }
来源：http://ul.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://en.lnxyls.cn

[O02] 使用线程池
来源：http://dk.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rp.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pp.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://oh.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://uk.chemitech.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oc.gzmigu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cs.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ps.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hl.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://pl.asd995.cn

Py:   with lock: shared += 1
来源：http://xq.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://qc.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xi.muxihuayi.cn

TS:   // 同 JS
来源：http://qn.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://kr.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://al.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sd.lnxyls.cn

C#:   lock (gate) { shared++; }
来源：http://ag.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://vp.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://za.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tk.hahajie.cn

JS:   async function f() { await g(); }
来源：http://zl.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zr.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aw.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cr.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gm.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://au.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://bp.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://ry.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nn.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://eo.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://vm.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fi.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ss.9csxet.cn

Ruby: threads.map(&:join)
来源：http://ks.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zn.nicolike.cn

[O06] 使用进程池
来源：http://hb.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rt.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zs.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://dj.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://gn.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pb.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://an.asd995.cn

Ruby: // fork 块
来源：http://zb.huanxung.cn

C#:   Parallel.For
来源：http://wh.panjiajie.cn

================================================================================
来源：http://em.muxihuayi.cn

P. 常用工具函数
来源：http://tp.huanxung.cn

================================================================================
来源：http://yg.bookmarksfly.cn

[P01] 生成 UUID
来源：http://kl.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://ow.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ob.asd995.cn

JS:   crypto.randomUUID()
来源：http://rr.nszjky.cn

TS:   crypto.randomUUID()
来源：http://fn.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://zi.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://ty.colortex.cn

Ruby: SecureRandom.uuid
来源：http://uc.szxytkj.cn

C#:   Guid.NewGuid().ToString()
来源：http://jr.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://ep.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eb.chemitech.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rd.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eh.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fc.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rk.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gl.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hl.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gd.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://nq.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yr.chemitech.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://al.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pu.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hd.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wq.521024.cn


<!-- 参考信息 -->