代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dz.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ji.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sc.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://js.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rb.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://io.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://us.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://co.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cp.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gl.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lb.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wy.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jl.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://su.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uy.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://hi.9csxet.cn

Py:   resp.json()
来源：http://ya.yuntaijiaju.cn

PHP:  json_decode($body, true);
来源：http://lm.shxzskj.cn

JS:   await resp.json()
来源：http://jk.9csxet.cn

TS:   await resp.json()
来源：http://lx.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cy.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://id.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://fl.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://du.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://pg.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dj.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bo.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://bg.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://yi.bookmarksfly.cn

Java: resp.statusCode()
来源：http://wr.huixiangedu.cn

Go:   resp.StatusCode
来源：http://hf.521024.cn

Ruby: resp.code.to_i
来源：http://zb.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://ew.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://go.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bw.521024.cn

PHP:  curl_multi_init() 系列
来源：http://yy.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fj.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sv.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ir.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xt.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ha.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://do.huixiangedu.cn

================================================================================
来源：http://ic.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://oy.nicolike.cn

================================================================================
来源：http://ib.muxihuayi.cn

[M01] 读取命令行参数
来源：http://pd.shxzskj.cn

Py:   sys.argv[1:]
来源：http://fl.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://vh.szsharing.cn

JS:   process.argv.slice(2)
来源：http://cf.521024.cn

TS:   process.argv.slice(2)
来源：http://dk.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://az.9csxet.cn

Go:   os.Args[1:]
来源：http://bh.colortex.cn

Ruby: ARGV
来源：http://uv.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://ln.muxihuayi.cn

[M02] 读取环境变量
来源：http://wv.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://lo.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://me.521024.cn

JS:   process.env.HOME
来源：http://ce.bjjhwx.cn

TS:   process.env.HOME
来源：http://zw.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://xr.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ia.nszjky.cn

Ruby: ENV["HOME"]
来源：http://cu.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fo.shxzukj.cn

[M03] 执行外部命令
来源：http://sv.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jk.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oi.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://om.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dc.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ij.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pc.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zz.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://zy.asd995.cn

[M04] 获取当前工作目录
来源：http://gt.muxihuayi.cn

Py:   os.getcwd()
来源：http://qa.jianghongdianzi.cn

PHP:  getcwd();
来源：http://ak.colortex.cn

JS:   process.cwd()
来源：http://hj.gzmigu.cn

TS:   process.cwd()
来源：http://ij.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://rp.gzmigu.cn

Go:   os.Getwd()
来源：http://gy.asd995.cn

Ruby: Dir.pwd
来源：http://dc.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yx.hnjuh.cn

[M05] 设置退出码
来源：http://ot.muxihuayi.cn

Py:   sys.exit(1)
来源：http://pr.haigaiapp.cn

PHP:  exit(1);
来源：http://ii.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://qp.nicolike.cn

TS:   process.exit(1)
来源：http://sz.gzmigu.cn

Java: System.exit(1)
来源：http://tz.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://ao.huixiangedu.cn

Ruby: exit 1
来源：http://dq.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wf.shxzskj.cn

[M06] 向标准错误输出
来源：http://gp.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://gc.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xh.wgjwhj.cn

JS:   console.error("err")
来源：http://ey.bjjhwx.cn

TS:   console.error("err")
来源：http://cj.521024.cn

Java: System.err.println("err")
来源：http://qs.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dh.bookmarksfly.cn

Ruby: warn "err"
来源：http://gy.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://ri.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://mf.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://um.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lh.panjiajie.cn

JS:   require.main === module
来源：http://pu.shxzskj.cn

TS:   require.main === module
来源：http://ww.asd995.cn

Java: public static void main(String[] args)
来源：http://yo.521024.cn

Go:   func main()
来源：http://bp.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fg.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://xj.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://ll.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://dx.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://ef.shxzskj.cn

JS:   process.platform;  process.version
来源：http://ct.panjiajie.cn

TS:   process.platform;  process.version
来源：http://me.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lk.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sb.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ti.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://or.bookmarksfly.cn

================================================================================
来源：http://sz.shxzskj.cn

N. 数据结构与算法
来源：http://es.nicolike.cn

================================================================================
来源：http://co.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://ea.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fr.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qu.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dy.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ea.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://md.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://pa.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gn.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ee.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://qo.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://eb.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jx.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://la.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xm.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lp.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://ja.colortex.cn

Ruby: arr.sort
来源：http://qv.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nm.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://dn.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bx.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://vx.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qr.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sq.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uk.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://um.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vh.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://os.nszjky.cn

[N04] 斐波那契数列
来源：http://si.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sg.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vo.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ag.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uz.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ho.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eq.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sa.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lk.yuntaijiaju.cn

[N05] 最大公约数
来源：http://ci.hahajie.cn

Py:   math.gcd(a, b)
来源：http://cm.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fu.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zv.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ds.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hs.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dm.gzmigu.cn

Ruby: a.gcd(b)
来源：http://jh.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jt.hahajie.cn

[N06] 判断回文字符串
来源：http://ub.muxihuayi.cn

Py:   s == s[::-1]
来源：http://md.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://ud.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://vr.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://cx.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yv.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://mx.newstarts.cn

Ruby: s == s.reverse
来源：http://kq.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ft.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://gk.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ak.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fy.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vo.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://dz.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://ut.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://uy.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://ns.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ac.shxzukj.cn

[N08] 生成全排列
来源：http://ii.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://kr.newstarts.cn

PHP:  // 手写递归交换
来源：http://bw.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://ae.hnjuh.cn

TS:   // 手写回溯递归
来源：http://ju.shxzskj.cn

Java: // 手写回溯递归
来源：http://la.szsharing.cn

Go:   // 手写回溯递归
来源：http://dj.shxzskj.cn

Ruby: arr.permutation.to_a
来源：http://md.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://vl.hahajie.cn

[N09] 栈与队列
来源：http://dl.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bk.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://em.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cx.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ml.panjiajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dt.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rl.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wt.nszjky.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oq.panjiajie.cn

[N10] 链表节点定义
来源：http://cr.hahajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gs.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gl.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fe.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ev.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://wd.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ks.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wo.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mv.nszjky.cn

[N11] 二叉树中序遍历
来源：http://pl.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dr.szsharing.cn

PHP:  // 手写递归函数
来源：http://lf.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dy.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://be.lnxyls.cn

Java: // 手写递归
来源：http://ld.chemitech.net.cn

Go:   // 手写递归
来源：http://wx.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kk.bjjhwx.cn

C#:   // 手写递归
来源：http://oe.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tu.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wr.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cp.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lx.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lz.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://my.asd995.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ui.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ur.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ks.panjiajie.cn

================================================================================
来源：http://hg.szsharing.cn

O. 并发与异步
来源：http://ui.szsharing.cn

================================================================================
来源：http://xt.muxihuayi.cn

[O01] 启动一个线程
来源：http://sp.lnxyls.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xp.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xr.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://an.haigaiapp.cn

TS:   // 同 JS
来源：http://jy.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://mj.newstarts.cn

Go:   go f()
来源：http://qz.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://bw.newstarts.cn

C#:   Task.Run(() => F());
来源：http://ef.nicolike.cn

[O02] 使用线程池
来源：http://jw.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hb.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sf.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://gw.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://ce.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cz.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bm.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://af.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aa.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://fr.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://rk.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://qn.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cr.lnxyls.cn

TS:   // 同 JS
来源：http://dv.521024.cn

Java: synchronized (this) { shared++; }
来源：http://dn.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wf.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://si.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://gx.9csxet.cn

[O04] 定义异步函数并等待
来源：http://zi.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://sy.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bk.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://wp.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vf.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gq.yuntaijiaju.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ue.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gg.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://np.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://xz.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://ae.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ag.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://cj.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://av.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ii.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cw.huanxung.cn

Ruby: threads.map(&:join)
来源：http://mg.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ca.asd995.cn

[O06] 使用进程池
来源：http://vx.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ba.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sk.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://ac.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://ag.bookmarksfly.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fu.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sj.newstarts.cn

Ruby: // fork 块
来源：http://by.chemitech.net.cn

C#:   Parallel.For
来源：http://mq.nicolike.cn

================================================================================
来源：http://zf.bjjhwx.cn

P. 常用工具函数
来源：http://yl.szsharing.cn

================================================================================
来源：http://jq.haigaiapp.cn

[P01] 生成 UUID
来源：http://ot.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://ab.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bl.nicolike.cn

JS:   crypto.randomUUID()
来源：http://db.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://sx.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://xl.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://rr.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://hp.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://ay.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://br.bookmarksfly.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lh.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tu.nicolike.cn


<!-- 参考信息 -->