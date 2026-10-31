代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pe.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hm.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pu.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pr.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ms.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kj.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yz.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://qv.muxihuayi.cn

Py:   resp.json()
来源：http://tu.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://vo.yuexingan06.cn

JS:   await resp.json()
来源：http://ek.shtwfgs.cn

TS:   await resp.json()
来源：http://kn.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nv.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sl.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://yd.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://js.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://cm.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zg.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zl.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://sp.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://vp.gzmigu.cn

Java: resp.statusCode()
来源：http://uh.colortex.cn

Go:   resp.StatusCode
来源：http://uj.9csxet.cn

Ruby: resp.code.to_i
来源：http://ld.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://wq.asd995.cn

[L08] 并发请求多个地址
来源：http://qr.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rp.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://mc.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pr.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hd.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ee.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ke.nicolike.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ut.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nf.9csxet.cn

================================================================================
来源：http://lm.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://kj.nszjky.cn

================================================================================
来源：http://xz.hahajie.cn

[M01] 读取命令行参数
来源：http://ml.huanxung.cn

Py:   sys.argv[1:]
来源：http://vq.9csxet.cn

PHP:  $argv;  $argc;
来源：http://hn.nszjky.cn

JS:   process.argv.slice(2)
来源：http://bn.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://bp.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://py.gzmigu.cn

Go:   os.Args[1:]
来源：http://kw.shxzskj.cn

Ruby: ARGV
来源：http://nh.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://nj.nicolike.cn

[M02] 读取环境变量
来源：http://ee.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://ri.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dn.hnjuh.cn

JS:   process.env.HOME
来源：http://yw.shxzukj.cn

TS:   process.env.HOME
来源：http://ah.szxytkj.cn

Java: System.getenv("HOME")
来源：http://qk.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zr.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://bo.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ni.bjjhwx.cn

[M03] 执行外部命令
来源：http://po.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wn.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ah.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ze.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yp.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wj.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hf.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ud.yuntaijiaju.cn

C#:   Process.Start("ls", "-l");
来源：http://jg.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://dy.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://kb.huanxung.cn

PHP:  getcwd();
来源：http://xa.shxzskj.cn

JS:   process.cwd()
来源：http://ad.nszjky.cn

TS:   process.cwd()
来源：http://wj.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://aw.shxzskj.cn

Go:   os.Getwd()
来源：http://ob.wgjwhj.cn

Ruby: Dir.pwd
来源：http://wj.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qn.asd995.cn

[M05] 设置退出码
来源：http://yj.nszjky.cn

Py:   sys.exit(1)
来源：http://oi.chemitech.net.cn

PHP:  exit(1);
来源：http://ge.chemitech.net.cn

JS:   process.exit(1)
来源：http://ug.panjiajie.cn

TS:   process.exit(1)
来源：http://rh.shtwfgs.cn

Java: System.exit(1)
来源：http://ky.wgjwhj.cn

Go:   os.Exit(1)
来源：http://qa.szsharing.cn

Ruby: exit 1
来源：http://me.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ua.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://dd.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://mh.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bg.jianghongdianzi.cn

JS:   console.error("err")
来源：http://rk.jianghongdianzi.cn

TS:   console.error("err")
来源：http://qz.asd995.cn

Java: System.err.println("err")
来源：http://aa.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fm.yuntaijiaju.cn

Ruby: warn "err"
来源：http://fp.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://fv.shxzskj.cn

[M07] 判断是否为主入口
来源：http://ih.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://yb.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nl.haigaiapp.cn

JS:   require.main === module
来源：http://fy.bjjhwx.cn

TS:   require.main === module
来源：http://ix.nszjky.cn

Java: public static void main(String[] args)
来源：http://nm.hnjuh.cn

Go:   func main()
来源：http://xf.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ub.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://bv.hahajie.cn

[M08] 获取系统与运行时信息
来源：http://ka.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://iy.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://eu.huanxung.cn

JS:   process.platform;  process.version
来源：http://po.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://zm.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://un.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yk.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xx.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lo.yuexingan06.cn

================================================================================
来源：http://en.asd995.cn

N. 数据结构与算法
来源：http://re.lnxyls.cn

================================================================================
来源：http://bk.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://id.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ie.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ix.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xl.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cf.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://of.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://oc.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cu.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jt.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://fh.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://sn.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rm.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ep.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qi.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fq.colortex.cn

Go:   slices.Sort(arr)
来源：http://zm.jctech888.com.cn

Ruby: arr.sort
来源：http://bz.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nc.colortex.cn

[N03] 快速排序（分治示例）
来源：http://nk.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://uu.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pk.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cv.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yb.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zc.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://az.newstarts.cn

C#:   // 手写递归，或 Array.Sort
来源：http://am.lnxyls.cn

[N04] 斐波那契数列
来源：http://pw.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zw.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kb.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lw.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qg.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ex.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ov.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eh.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dg.bjjhwx.cn

[N05] 最大公约数
来源：http://fy.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://hf.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://st.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bh.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uu.bookmarksfly.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ol.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://js.nicolike.cn

Ruby: a.gcd(b)
来源：http://fm.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lk.wgjwhj.cn

[N06] 判断回文字符串
来源：http://kd.wgjwhj.cn

Py:   s == s[::-1]
来源：http://wx.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://xy.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://md.bjjhwx.cn

TS:   s === [...s].reverse().join("")
来源：http://aa.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uq.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://uu.bookmarksfly.cn

Ruby: s == s.reverse
来源：http://rj.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lo.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://wo.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xy.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uc.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bc.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://hd.lnxyls.cn

Java: // 手写 HashMap
来源：http://vv.hahajie.cn

Go:   // 手写 map[int]int
来源：http://tm.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://wc.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://aw.yuexingan06.cn

[N08] 生成全排列
来源：http://ay.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://ol.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://ux.hahajie.cn

JS:   // 手写回溯递归
来源：http://uy.9csxet.cn

TS:   // 手写回溯递归
来源：http://wv.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://qv.huanxung.cn

Go:   // 手写回溯递归
来源：http://kr.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://se.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://tj.colortex.cn

[N09] 栈与队列
来源：http://tg.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dg.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eg.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tc.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://se.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hd.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ej.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ek.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xy.hahajie.cn

[N10] 链表节点定义
来源：http://hw.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vp.muxihuayi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dl.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ug.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xx.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://bu.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yu.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cm.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ee.hahajie.cn

[N11] 二叉树中序遍历
来源：http://bg.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ye.lnxyls.cn

PHP:  // 手写递归函数
来源：http://qx.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oi.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nh.521024.cn

Java: // 手写递归
来源：http://fh.huixiangedu.cn

Go:   // 手写递归
来源：http://th.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vq.haigaiapp.cn

C#:   // 手写递归
来源：http://iu.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tq.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gx.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tp.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gy.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nu.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nk.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fa.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rj.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://si.shtwfgs.cn

================================================================================
来源：http://yl.hnjuh.cn

O. 并发与异步
来源：http://ch.bjjhwx.cn

================================================================================
来源：http://vl.szxytkj.cn

[O01] 启动一个线程
来源：http://fq.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fx.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://at.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ru.colortex.cn

TS:   // 同 JS
来源：http://zp.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://ox.shtwfgs.cn

Go:   go f()
来源：http://tm.szsharing.cn

Ruby: Thread.new { f }
来源：http://sa.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://na.colortex.cn

[O02] 使用线程池
来源：http://aq.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ky.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lx.szxytkj.cn

JS:   // worker_threads 线程池
来源：http://le.nicolike.cn

TS:   // worker_threads 线程池
来源：http://zd.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nc.jctech888.com.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cq.huixinmuqiang.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uo.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wy.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://wn.lnxyls.cn

Py:   with lock: shared += 1
来源：http://gq.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://zf.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fq.haigaiapp.cn

TS:   // 同 JS
来源：http://nf.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://zi.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bn.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://so.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://vn.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://ev.asd995.cn

Py:   async def f():⏎    await g()
来源：http://wn.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wu.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://uf.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://us.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wf.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oo.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nn.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://uh.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://ch.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://tj.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://du.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://wg.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://jx.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ov.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://na.newstarts.cn

Ruby: threads.map(&:join)
来源：http://sk.521024.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jt.szxytkj.cn

[O06] 使用进程池
来源：http://yh.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mq.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dp.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://cn.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://hg.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gr.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qw.bjjhwx.cn

Ruby: // fork 块
来源：http://da.yuntaijiaju.cn

C#:   Parallel.For
来源：http://th.jianghongdianzi.cn

================================================================================
来源：http://se.haigaiapp.cn

P. 常用工具函数
来源：http://cc.newstarts.cn

================================================================================
来源：http://qq.shxzskj.cn

[P01] 生成 UUID
来源：http://dk.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://sk.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dq.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://vx.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://wk.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://zh.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://qd.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://in.szxytkj.cn

C#:   Guid.NewGuid().ToString()
来源：http://ky.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://ma.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mz.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yq.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qj.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bh.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mv.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ov.haigaiapp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xp.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ws.panjiajie.cn

[P03] 生成短随机字符串
来源：http://yo.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lg.chemitech.net.cn


<!-- 参考信息 -->