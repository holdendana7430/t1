代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hy.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://il.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lz.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sf.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xh.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oz.9csxet.cn

[L05] 上传文件（multipart）
来源：http://vp.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://up.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pz.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mp.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ix.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zi.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lc.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ei.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ve.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://tr.asd995.cn

Py:   resp.json()
来源：http://ci.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://yk.lnxyls.cn

JS:   await resp.json()
来源：http://le.huixinmuqiang.cn

TS:   await resp.json()
来源：http://jv.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hl.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mj.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://ho.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uy.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://ns.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sw.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gv.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://pp.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://kp.yuexingan06.cn

Java: resp.statusCode()
来源：http://rx.muxihuayi.cn

Go:   resp.StatusCode
来源：http://mx.colortex.cn

Ruby: resp.code.to_i
来源：http://as.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://rz.szxytkj.cn

[L08] 并发请求多个地址
来源：http://lm.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qr.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://xk.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://de.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://by.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vf.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hy.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iy.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rs.panjiajie.cn

================================================================================
来源：http://sa.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://ip.bjjhwx.cn

================================================================================
来源：http://ew.shxzskj.cn

[M01] 读取命令行参数
来源：http://ao.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://nd.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://xr.szsharing.cn

JS:   process.argv.slice(2)
来源：http://sh.nicolike.cn

TS:   process.argv.slice(2)
来源：http://sx.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://iu.shxzskj.cn

Go:   os.Args[1:]
来源：http://kn.chemitech.net.cn

Ruby: ARGV
来源：http://eb.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://qh.lnxyls.cn

[M02] 读取环境变量
来源：http://du.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://ue.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://er.shtwfgs.cn

JS:   process.env.HOME
来源：http://bf.colortex.cn

TS:   process.env.HOME
来源：http://cn.gzmigu.cn

Java: System.getenv("HOME")
来源：http://qr.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bd.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://pt.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dt.bookmarksfly.cn

[M03] 执行外部命令
来源：http://ek.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eo.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://or.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gm.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wy.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cc.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gc.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ta.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://do.colortex.cn

[M04] 获取当前工作目录
来源：http://ho.asd995.cn

Py:   os.getcwd()
来源：http://ak.bookmarksfly.cn

PHP:  getcwd();
来源：http://mh.yuntaijiaju.cn

JS:   process.cwd()
来源：http://lm.yuexingan06.cn

TS:   process.cwd()
来源：http://yc.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://ww.gzmigu.cn

Go:   os.Getwd()
来源：http://zt.shxzukj.cn

Ruby: Dir.pwd
来源：http://nj.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fk.gzmigu.cn

[M05] 设置退出码
来源：http://zs.muxihuayi.cn

Py:   sys.exit(1)
来源：http://qu.jianghongdianzi.cn

PHP:  exit(1);
来源：http://wj.521024.cn

JS:   process.exit(1)
来源：http://sg.jctech888.com.cn

TS:   process.exit(1)
来源：http://ij.haigaiapp.cn

Java: System.exit(1)
来源：http://zt.bjjhwx.cn

Go:   os.Exit(1)
来源：http://kk.lnxyls.cn

Ruby: exit 1
来源：http://id.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hf.bjjhwx.cn

[M06] 向标准错误输出
来源：http://fg.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://so.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://aw.muxihuayi.cn

JS:   console.error("err")
来源：http://vr.asd995.cn

TS:   console.error("err")
来源：http://kf.gzmigu.cn

Java: System.err.println("err")
来源：http://gq.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zt.jianghongdianzi.cn

Ruby: warn "err"
来源：http://hc.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://pz.521024.cn

[M07] 判断是否为主入口
来源：http://yk.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://gp.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jh.hahajie.cn

JS:   require.main === module
来源：http://dn.yuntaijiaju.cn

TS:   require.main === module
来源：http://de.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://vj.9csxet.cn

Go:   func main()
来源：http://ch.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tj.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://ah.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://bk.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://zv.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://po.nszjky.cn

JS:   process.platform;  process.version
来源：http://fx.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://pi.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ak.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sm.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zn.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kt.chemitech.net.cn

================================================================================
来源：http://zb.muxihuayi.cn

N. 数据结构与算法
来源：http://gn.nicolike.cn

================================================================================
来源：http://tl.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://tm.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ib.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gf.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://py.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kx.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ao.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://aj.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jm.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aw.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://iq.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://yj.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kr.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cs.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xg.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ul.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://mn.shtwfgs.cn

Ruby: arr.sort
来源：http://el.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bp.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://ta.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ic.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://jf.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qm.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hn.newstarts.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sa.shxzskj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lu.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nt.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nm.asd995.cn

[N04] 斐波那契数列
来源：http://oj.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hm.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ql.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tq.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nm.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vs.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hl.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fk.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ja.panjiajie.cn

[N05] 最大公约数
来源：http://hq.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://oe.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bw.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qz.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qu.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fr.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ag.szsharing.cn

Ruby: a.gcd(b)
来源：http://ts.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xy.newstarts.cn

[N06] 判断回文字符串
来源：http://zq.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://kq.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://ec.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://lf.wgjwhj.cn

TS:   s === [...s].reverse().join("")
来源：http://qk.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hx.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://vi.yuexingan06.cn

Ruby: s == s.reverse
来源：http://qr.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ih.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://eg.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oy.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nr.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rz.huixinmuqiang.cn

TS:   // 手写 Map<string, number>
来源：http://bt.521024.cn

Java: // 手写 HashMap
来源：http://rv.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://yw.gzmigu.cn

Ruby: // 手写 Hash
来源：http://ey.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ci.yuntaijiaju.cn

[N08] 生成全排列
来源：http://ov.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://xl.lnxyls.cn

PHP:  // 手写递归交换
来源：http://sz.hnjuh.cn

JS:   // 手写回溯递归
来源：http://lc.nicolike.cn

TS:   // 手写回溯递归
来源：http://iq.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://qc.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://hj.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://yg.panjiajie.cn

C#:   // 手写回溯递归
来源：http://tx.wgjwhj.cn

[N09] 栈与队列
来源：http://xt.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hy.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jl.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wt.shxzskj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cf.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ks.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ra.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ia.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://or.asd995.cn

[N10] 链表节点定义
来源：http://xf.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wk.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tf.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gw.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ze.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://ca.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xf.colortex.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gi.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mf.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://tg.bookmarksfly.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pm.shxzskj.cn

PHP:  // 手写递归函数
来源：http://bf.521024.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kl.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hs.haigaiapp.cn

Java: // 手写递归
来源：http://rb.jctech888.com.cn

Go:   // 手写递归
来源：http://kr.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://us.bjjhwx.cn

C#:   // 手写递归
来源：http://la.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://be.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://il.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tz.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tr.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zm.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jg.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dm.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xw.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bk.jianghongdianzi.cn

================================================================================
来源：http://un.lnxyls.cn

O. 并发与异步
来源：http://vb.bookmarksfly.cn

================================================================================
来源：http://sc.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://fn.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mx.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://do.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rj.bjjhwx.cn

TS:   // 同 JS
来源：http://al.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://xg.chemitech.net.cn

Go:   go f()
来源：http://tv.asd995.cn

Ruby: Thread.new { f }
来源：http://eg.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://jf.bjjhwx.cn

[O02] 使用线程池
来源：http://gi.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oy.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bh.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://ud.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://nl.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wa.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wx.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ns.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://td.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://hp.szsharing.cn

Py:   with lock: shared += 1
来源：http://vi.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://my.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://no.chemitech.net.cn

TS:   // 同 JS
来源：http://hg.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://gc.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pt.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rg.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://ap.9csxet.cn

[O04] 定义异步函数并等待
来源：http://gv.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://nr.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vb.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://aj.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vp.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gn.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://le.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wn.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://ex.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://jh.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://mm.wgjwhj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pa.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://yp.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://za.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tz.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pg.shxzskj.cn

Ruby: threads.map(&:join)
来源：http://om.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kx.asd995.cn

[O06] 使用进程池
来源：http://bz.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ed.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vg.asd995.cn

JS:   // child_process / cluster 模块
来源：http://da.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://xu.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ui.haigaiapp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jh.lnxyls.cn

Ruby: // fork 块
来源：http://ql.yuexingan06.cn

C#:   Parallel.For
来源：http://sg.shxzskj.cn

================================================================================
来源：http://cx.jctech888.com.cn

P. 常用工具函数
来源：http://qc.yuexingan06.cn

================================================================================
来源：http://vl.521024.cn

[P01] 生成 UUID
来源：http://of.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://nn.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jx.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://iq.521024.cn

TS:   crypto.randomUUID()
来源：http://cw.521024.cn

Java: UUID.randomUUID().toString()
来源：http://zv.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://jb.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://eb.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://ti.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://oh.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yp.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://za.chemitech.net.cn


<!-- 参考信息 -->