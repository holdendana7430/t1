代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jy.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rq.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kc.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jf.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zf.yuntaijiaju.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nn.nicolike.cn

[L05] 上传文件（multipart）
来源：http://tg.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wp.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qh.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rw.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gh.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gc.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://on.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zf.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dn.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://fn.muxihuayi.cn

Py:   resp.json()
来源：http://qb.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://tr.yuexingan06.cn

JS:   await resp.json()
来源：http://bo.shxzskj.cn

TS:   await resp.json()
来源：http://qc.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://di.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ch.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://dr.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://of.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://vm.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vg.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eb.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://mt.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://vw.shxzskj.cn

Java: resp.statusCode()
来源：http://vl.shxzskj.cn

Go:   resp.StatusCode
来源：http://aj.panjiajie.cn

Ruby: resp.code.to_i
来源：http://wg.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://hq.huanxung.cn

[L08] 并发请求多个地址
来源：http://pt.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yv.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://lw.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dh.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ui.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ir.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ju.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nl.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zc.asd995.cn

================================================================================
来源：http://yc.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://hz.shxzskj.cn

================================================================================
来源：http://ih.9csxet.cn

[M01] 读取命令行参数
来源：http://gk.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://dm.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://lr.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://mz.asd995.cn

TS:   process.argv.slice(2)
来源：http://fa.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://ps.huixiangedu.cn

Go:   os.Args[1:]
来源：http://tj.shtwfgs.cn

Ruby: ARGV
来源：http://kr.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://vc.jctech888.com.cn

[M02] 读取环境变量
来源：http://un.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://xw.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tx.jctech888.com.cn

JS:   process.env.HOME
来源：http://dq.szsharing.cn

TS:   process.env.HOME
来源：http://ys.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://ff.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ja.9csxet.cn

Ruby: ENV["HOME"]
来源：http://wk.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://id.haigaiapp.cn

[M03] 执行外部命令
来源：http://pu.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oq.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jh.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://as.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gh.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rs.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://io.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://up.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://uu.newstarts.cn

[M04] 获取当前工作目录
来源：http://fe.yuexingan06.cn

Py:   os.getcwd()
来源：http://ud.bookmarksfly.cn

PHP:  getcwd();
来源：http://ej.yuntaijiaju.cn

JS:   process.cwd()
来源：http://wz.shtwfgs.cn

TS:   process.cwd()
来源：http://aa.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://bn.jctech888.com.cn

Go:   os.Getwd()
来源：http://mk.chemitech.net.cn

Ruby: Dir.pwd
来源：http://tp.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ey.panjiajie.cn

[M05] 设置退出码
来源：http://ks.shxzukj.cn

Py:   sys.exit(1)
来源：http://ug.9csxet.cn

PHP:  exit(1);
来源：http://wk.szxytkj.cn

JS:   process.exit(1)
来源：http://jb.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://an.jctech888.com.cn

Java: System.exit(1)
来源：http://yw.hnjuh.cn

Go:   os.Exit(1)
来源：http://os.newstarts.cn

Ruby: exit 1
来源：http://dk.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hv.jctech888.com.cn

[M06] 向标准错误输出
来源：http://cl.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://gh.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gk.colortex.cn

JS:   console.error("err")
来源：http://ck.bjjhwx.cn

TS:   console.error("err")
来源：http://rp.9csxet.cn

Java: System.err.println("err")
来源：http://mx.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bx.huixiangedu.cn

Ruby: warn "err"
来源：http://mg.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://ze.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://fp.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://pk.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dm.huixinmuqiang.cn

JS:   require.main === module
来源：http://su.colortex.cn

TS:   require.main === module
来源：http://qz.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://lp.wgjwhj.cn

Go:   func main()
来源：http://gu.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sa.huanxung.cn

C#:   static void Main(string[] args)
来源：http://xj.colortex.cn

[M08] 获取系统与运行时信息
来源：http://sy.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://bf.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://yp.szxytkj.cn

JS:   process.platform;  process.version
来源：http://mg.hahajie.cn

TS:   process.platform;  process.version
来源：http://cn.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fu.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jh.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qh.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lm.huixinmuqiang.cn

================================================================================
来源：http://ze.newstarts.cn

N. 数据结构与算法
来源：http://jc.chemitech.net.cn

================================================================================
来源：http://oz.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://rw.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://da.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bb.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lg.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vj.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://eb.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://mq.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://za.521024.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ou.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://us.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://af.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ki.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gi.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://st.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ri.huanxung.cn

Go:   slices.Sort(arr)
来源：http://ng.szxytkj.cn

Ruby: arr.sort
来源：http://yp.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mf.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://ho.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bm.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://wk.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gv.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yc.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vc.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gu.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ij.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://up.newstarts.cn

[N04] 斐波那契数列
来源：http://wk.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ry.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lx.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xr.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gb.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qe.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pd.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mj.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zr.jianghongdianzi.cn

[N05] 最大公约数
来源：http://hq.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://pp.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tp.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ya.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://je.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nt.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wd.nszjky.cn

Ruby: a.gcd(b)
来源：http://ft.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://le.colortex.cn

[N06] 判断回文字符串
来源：http://yz.asd995.cn

Py:   s == s[::-1]
来源：http://cg.hahajie.cn

PHP:  $s === strrev($s);
来源：http://rm.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://js.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://ne.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fd.asd995.cn

Go:   // 双指针从两端比较
来源：http://rk.hnjuh.cn

Ruby: s == s.reverse
来源：http://uy.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cj.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://pt.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lv.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bi.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lx.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://lq.9csxet.cn

Java: // 手写 HashMap
来源：http://rd.nszjky.cn

Go:   // 手写 map[int]int
来源：http://ci.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://ie.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zy.huixiangedu.cn

[N08] 生成全排列
来源：http://hl.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://dt.panjiajie.cn

PHP:  // 手写递归交换
来源：http://nn.panjiajie.cn

JS:   // 手写回溯递归
来源：http://fm.nszjky.cn

TS:   // 手写回溯递归
来源：http://dg.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://fs.newstarts.cn

Go:   // 手写回溯递归
来源：http://kv.521024.cn

Ruby: arr.permutation.to_a
来源：http://gm.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://kx.asd995.cn

[N09] 栈与队列
来源：http://xc.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nf.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yo.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ce.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ek.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hm.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jw.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kp.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tc.nicolike.cn

[N10] 链表节点定义
来源：http://ij.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://md.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://si.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xe.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cz.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://vz.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vg.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rx.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ps.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://uc.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gb.newstarts.cn

PHP:  // 手写递归函数
来源：http://pg.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fq.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ps.huixinmuqiang.cn

Java: // 手写递归
来源：http://vb.haigaiapp.cn

Go:   // 手写递归
来源：http://ii.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ka.shtwfgs.cn

C#:   // 手写递归
来源：http://jv.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pk.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pf.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uu.yuntaijiaju.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mp.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yf.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://im.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cl.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cv.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hp.shtwfgs.cn

================================================================================
来源：http://wa.panjiajie.cn

O. 并发与异步
来源：http://ws.colortex.cn

================================================================================
来源：http://ky.colortex.cn

[O01] 启动一个线程
来源：http://gp.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gy.haigaiapp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://er.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xx.jctech888.com.cn

TS:   // 同 JS
来源：http://ma.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://rf.yuexingan06.cn

Go:   go f()
来源：http://hm.newstarts.cn

Ruby: Thread.new { f }
来源：http://ug.nszjky.cn

C#:   Task.Run(() => F());
来源：http://ct.9csxet.cn

[O02] 使用线程池
来源：http://ha.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fj.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gx.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://rh.szsharing.cn

TS:   // worker_threads 线程池
来源：http://gi.chemitech.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ng.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tx.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tj.hnjuh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dm.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://ky.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://fa.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://iz.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gc.panjiajie.cn

TS:   // 同 JS
来源：http://vu.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://qy.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zf.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uo.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://tl.nszjky.cn

[O04] 定义异步函数并等待
来源：http://yz.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://dj.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jy.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://pj.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://za.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lt.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rs.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://eo.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://zf.521024.cn

[O05] 并发执行并等待全部完成
来源：http://vj.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://by.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vp.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://uw.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://aa.szsharing.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ot.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bf.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://ep.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jh.szsharing.cn

[O06] 使用进程池
来源：http://ne.nszjky.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lv.huanxung.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uw.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://jz.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://ql.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lw.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ow.jianghongdianzi.cn

Ruby: // fork 块
来源：http://nk.bookmarksfly.cn

C#:   Parallel.For
来源：http://ir.haigaiapp.cn

================================================================================
来源：http://dd.bjjhwx.cn

P. 常用工具函数
来源：http://jp.hahajie.cn

================================================================================
来源：http://ig.hnjuh.cn

[P01] 生成 UUID
来源：http://fq.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://xe.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hd.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://hc.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://cc.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://ln.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://yi.asd995.cn

Ruby: SecureRandom.uuid
来源：http://gm.bjjhwx.cn

C#:   Guid.NewGuid().ToString()
来源：http://cg.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://xp.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xm.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mj.9csxet.cn


<!-- 参考信息 -->