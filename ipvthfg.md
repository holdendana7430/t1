代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bb.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gj.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ju.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wu.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qp.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zg.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jm.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://ls.jctech888.com.cn

Py:   resp.json()
来源：http://nj.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://zo.wgjwhj.cn

JS:   await resp.json()
来源：http://wj.panjiajie.cn

TS:   await resp.json()
来源：http://xx.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zt.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gs.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://da.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wz.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://oh.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://im.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ij.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://ym.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://ft.yuexingan06.cn

Java: resp.statusCode()
来源：http://ac.muxihuayi.cn

Go:   resp.StatusCode
来源：http://es.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://pt.521024.cn

C#:   (int)resp.StatusCode
来源：http://uh.9csxet.cn

[L08] 并发请求多个地址
来源：http://zf.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mn.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://vl.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pr.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rj.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hw.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hb.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ut.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ds.huanxung.cn

================================================================================
来源：http://cb.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://gd.nszjky.cn

================================================================================
来源：http://bp.9csxet.cn

[M01] 读取命令行参数
来源：http://iv.szsharing.cn

Py:   sys.argv[1:]
来源：http://oq.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://vc.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://pj.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://em.521024.cn

Java: args 数组（main 方法参数）
来源：http://ss.9csxet.cn

Go:   os.Args[1:]
来源：http://yh.hnjuh.cn

Ruby: ARGV
来源：http://wg.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://hz.newstarts.cn

[M02] 读取环境变量
来源：http://bf.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://fm.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hi.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://fe.colortex.cn

TS:   process.env.HOME
来源：http://bx.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://gd.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kp.newstarts.cn

Ruby: ENV["HOME"]
来源：http://mm.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rd.colortex.cn

[M03] 执行外部命令
来源：http://gg.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://at.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yg.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://eq.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cx.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xx.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tk.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kp.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://et.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://zb.shxzukj.cn

Py:   os.getcwd()
来源：http://pj.shtwfgs.cn

PHP:  getcwd();
来源：http://sk.yuntaijiaju.cn

JS:   process.cwd()
来源：http://hr.shxzskj.cn

TS:   process.cwd()
来源：http://bb.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://uu.wgjwhj.cn

Go:   os.Getwd()
来源：http://mq.9csxet.cn

Ruby: Dir.pwd
来源：http://om.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://us.szxytkj.cn

[M05] 设置退出码
来源：http://lp.shxzukj.cn

Py:   sys.exit(1)
来源：http://wc.yuntaijiaju.cn

PHP:  exit(1);
来源：http://yo.bjjhwx.cn

JS:   process.exit(1)
来源：http://ch.bookmarksfly.cn

TS:   process.exit(1)
来源：http://ph.shxzukj.cn

Java: System.exit(1)
来源：http://qg.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://ku.bookmarksfly.cn

Ruby: exit 1
来源：http://fa.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ih.panjiajie.cn

[M06] 向标准错误输出
来源：http://qg.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://df.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://la.huixinmuqiang.cn

JS:   console.error("err")
来源：http://dm.shxzukj.cn

TS:   console.error("err")
来源：http://ki.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://lz.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ff.huanxung.cn

Ruby: warn "err"
来源：http://hh.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://ti.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://nr.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://wx.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://km.lnxyls.cn

JS:   require.main === module
来源：http://ow.shxzskj.cn

TS:   require.main === module
来源：http://dm.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://vn.hnjuh.cn

Go:   func main()
来源：http://ua.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ef.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://aw.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://be.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://jz.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://bi.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://jb.newstarts.cn

TS:   process.platform;  process.version
来源：http://ry.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cd.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vt.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ic.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://if.newstarts.cn

================================================================================
来源：http://tz.bjjhwx.cn

N. 数据结构与算法
来源：http://gt.bjjhwx.cn

================================================================================
来源：http://jr.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://cp.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lr.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vv.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bi.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dg.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tc.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://vd.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hf.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zm.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://nh.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://kq.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ou.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wm.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zz.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ea.521024.cn

Go:   slices.Sort(arr)
来源：http://po.huixiangedu.cn

Ruby: arr.sort
来源：http://ie.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://un.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://ex.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jf.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://du.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://po.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bp.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xn.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dc.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fi.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cc.panjiajie.cn

[N04] 斐波那契数列
来源：http://jq.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xo.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qy.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ss.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pv.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kq.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ju.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://id.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ni.newstarts.cn

[N05] 最大公约数
来源：http://vm.colortex.cn

Py:   math.gcd(a, b)
来源：http://wk.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ig.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jp.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ly.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ou.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yo.hahajie.cn

Ruby: a.gcd(b)
来源：http://bw.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sg.hnjuh.cn

[N06] 判断回文字符串
来源：http://it.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://dx.newstarts.cn

PHP:  $s === strrev($s);
来源：http://wm.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://nf.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://uw.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bz.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://hd.chemitech.net.cn

Ruby: s == s.reverse
来源：http://rn.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gf.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://vr.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ln.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bi.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cg.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://iv.jctech888.com.cn

Java: // 手写 HashMap
来源：http://kb.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://hr.521024.cn

Ruby: // 手写 Hash
来源：http://sr.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://su.jianghongdianzi.cn

[N08] 生成全排列
来源：http://kt.yuexingan06.cn

Py:   itertools.permutations(arr)
来源：http://qy.nicolike.cn

PHP:  // 手写递归交换
来源：http://ne.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://tj.asd995.cn

TS:   // 手写回溯递归
来源：http://pi.9csxet.cn

Java: // 手写回溯递归
来源：http://ou.shxzukj.cn

Go:   // 手写回溯递归
来源：http://ci.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://fp.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://jm.jianghongdianzi.cn

[N09] 栈与队列
来源：http://ij.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ng.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lu.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gb.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sr.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rr.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qo.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pp.colortex.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gd.hahajie.cn

[N10] 链表节点定义
来源：http://qq.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gg.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bo.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mb.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ao.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://so.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jm.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pa.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bn.hahajie.cn

[N11] 二叉树中序遍历
来源：http://yb.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ky.muxihuayi.cn

PHP:  // 手写递归函数
来源：http://lx.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fb.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oi.yuexingan06.cn

Java: // 手写递归
来源：http://fl.muxihuayi.cn

Go:   // 手写递归
来源：http://xt.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wd.haigaiapp.cn

C#:   // 手写递归
来源：http://eg.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wx.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hi.nicolike.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hu.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vy.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mu.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ea.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://do.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hu.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fh.chemitech.net.cn

================================================================================
来源：http://at.nicolike.cn

O. 并发与异步
来源：http://dc.chemitech.net.cn

================================================================================
来源：http://vg.nszjky.cn

[O01] 启动一个线程
来源：http://po.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vr.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yr.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ky.huixiangedu.cn

TS:   // 同 JS
来源：http://dm.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://tw.szxytkj.cn

Go:   go f()
来源：http://up.shxzskj.cn

Ruby: Thread.new { f }
来源：http://zg.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://ko.hahajie.cn

[O02] 使用线程池
来源：http://jq.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ti.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hj.colortex.cn

JS:   // worker_threads 线程池
来源：http://xt.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://qy.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cg.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mj.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pn.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ve.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://lv.gzmigu.cn

Py:   with lock: shared += 1
来源：http://zv.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://tl.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sf.asd995.cn

TS:   // 同 JS
来源：http://ma.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://dv.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://en.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://le.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://gj.nicolike.cn

[O04] 定义异步函数并等待
来源：http://qx.asd995.cn

Py:   async def f():⏎    await g()
来源：http://cd.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pc.hahajie.cn

JS:   async function f() { await g(); }
来源：http://jn.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nj.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jg.nicolike.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://db.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lo.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://fv.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://fh.szxytkj.cn

Py:   asyncio.gather(*tasks)
来源：http://sb.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hp.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://bx.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://lk.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vl.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lv.huanxung.cn

Ruby: threads.map(&:join)
来源：http://ze.szxytkj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jm.asd995.cn

[O06] 使用进程池
来源：http://ip.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://es.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nf.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://vi.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://od.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bg.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qq.yuexingan06.cn

Ruby: // fork 块
来源：http://lj.jctech888.com.cn

C#:   Parallel.For
来源：http://zf.bookmarksfly.cn

================================================================================
来源：http://uw.huixinmuqiang.cn

P. 常用工具函数
来源：http://zg.panjiajie.cn

================================================================================
来源：http://lm.nszjky.cn

[P01] 生成 UUID
来源：http://cm.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://jv.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qc.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://ki.jctech888.com.cn

TS:   crypto.randomUUID()
来源：http://rm.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://jw.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://lg.asd995.cn

Ruby: SecureRandom.uuid
来源：http://pf.newstarts.cn

C#:   Guid.NewGuid().ToString()
来源：http://kg.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://eh.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hnjuh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gt.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gw.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tt.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kw.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://en.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iu.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ei.9csxet.cn

[P03] 生成短随机字符串
来源：http://ce.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://un.wgjwhj.cn


<!-- 参考信息 -->