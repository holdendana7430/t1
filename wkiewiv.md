代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iy.yuntaijiaju.cn

[L04] 设置超时
来源：http://rm.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://mp.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nn.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://td.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nq.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cc.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://my.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ag.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vx.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://wd.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sg.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fg.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zp.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nj.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zr.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kv.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mv.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://st.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://rl.huixinmuqiang.cn

Py:   resp.json()
来源：http://ls.nszjky.cn

PHP:  json_decode($body, true);
来源：http://qu.wgjwhj.cn

JS:   await resp.json()
来源：http://ym.yuntaijiaju.cn

TS:   await resp.json()
来源：http://ll.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ze.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jb.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://ta.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zk.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://ct.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cm.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sz.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://xz.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://dr.newstarts.cn

Java: resp.statusCode()
来源：http://mf.colortex.cn

Go:   resp.StatusCode
来源：http://wr.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://cm.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://pi.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://oo.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cw.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://hv.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://px.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qe.nicolike.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rk.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dn.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://us.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ve.asd995.cn

================================================================================
来源：http://cb.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://ha.jianghongdianzi.cn

================================================================================
来源：http://fy.haigaiapp.cn

[M01] 读取命令行参数
来源：http://qh.shxzukj.cn

Py:   sys.argv[1:]
来源：http://rx.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://vx.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://gg.asd995.cn

TS:   process.argv.slice(2)
来源：http://io.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://qw.asd995.cn

Go:   os.Args[1:]
来源：http://pw.gzmigu.cn

Ruby: ARGV
来源：http://tc.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://np.asd995.cn

[M02] 读取环境变量
来源：http://nn.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://by.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pd.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://ro.hahajie.cn

TS:   process.env.HOME
来源：http://ni.huanxung.cn

Java: System.getenv("HOME")
来源：http://zn.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oj.9csxet.cn

Ruby: ENV["HOME"]
来源：http://uu.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sm.hahajie.cn

[M03] 执行外部命令
来源：http://ov.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ia.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jc.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lb.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://is.521024.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ht.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cn.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dt.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://qi.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://qi.shxzukj.cn

Py:   os.getcwd()
来源：http://cn.muxihuayi.cn

PHP:  getcwd();
来源：http://bh.newstarts.cn

JS:   process.cwd()
来源：http://yh.jianghongdianzi.cn

TS:   process.cwd()
来源：http://ei.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://zv.colortex.cn

Go:   os.Getwd()
来源：http://ab.wgjwhj.cn

Ruby: Dir.pwd
来源：http://cp.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xa.huixinmuqiang.cn

[M05] 设置退出码
来源：http://gu.shtwfgs.cn

Py:   sys.exit(1)
来源：http://th.bjjhwx.cn

PHP:  exit(1);
来源：http://iq.szsharing.cn

JS:   process.exit(1)
来源：http://xk.bookmarksfly.cn

TS:   process.exit(1)
来源：http://pb.chemitech.net.cn

Java: System.exit(1)
来源：http://ip.521024.cn

Go:   os.Exit(1)
来源：http://ez.shxzukj.cn

Ruby: exit 1
来源：http://wk.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ka.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://tr.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://zm.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fv.nicolike.cn

JS:   console.error("err")
来源：http://je.huanxung.cn

TS:   console.error("err")
来源：http://qx.wgjwhj.cn

Java: System.err.println("err")
来源：http://va.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dc.huixiangedu.cn

Ruby: warn "err"
来源：http://ou.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://sr.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://te.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://ie.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wd.nicolike.cn

JS:   require.main === module
来源：http://ve.nicolike.cn

TS:   require.main === module
来源：http://ug.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://ru.muxihuayi.cn

Go:   func main()
来源：http://vw.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ja.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://qp.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://na.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://hc.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://lz.szxytkj.cn

JS:   process.platform;  process.version
来源：http://tc.521024.cn

TS:   process.platform;  process.version
来源：http://yt.jctech888.com.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ms.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nq.huixinmuqiang.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ug.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sj.jianghongdianzi.cn

================================================================================
来源：http://kt.hahajie.cn

N. 数据结构与算法
来源：http://un.gzmigu.cn

================================================================================
来源：http://ct.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://ea.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://de.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wm.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eu.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vr.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zi.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://hi.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zp.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sq.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://dc.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://aj.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gf.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://au.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bg.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eo.newstarts.cn

Go:   slices.Sort(arr)
来源：http://gb.panjiajie.cn

Ruby: arr.sort
来源：http://nt.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gv.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://de.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ls.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://fq.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wk.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kp.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tn.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jf.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gu.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hm.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://sp.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vy.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uw.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wf.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fx.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dx.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nj.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://op.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ih.asd995.cn

[N05] 最大公约数
来源：http://ad.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://jp.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vk.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dj.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://on.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cr.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xo.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://qq.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zg.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://lz.newstarts.cn

Py:   s == s[::-1]
来源：http://ql.szsharing.cn

PHP:  $s === strrev($s);
来源：http://uh.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://sl.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://xe.huanxung.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zb.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://az.chemitech.net.cn

Ruby: s == s.reverse
来源：http://tz.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tv.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://rf.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://io.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://la.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hh.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://in.szsharing.cn

Java: // 手写 HashMap
来源：http://jd.huanxung.cn

Go:   // 手写 map[int]int
来源：http://xa.haigaiapp.cn

Ruby: // 手写 Hash
来源：http://pe.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ed.nicolike.cn

[N08] 生成全排列
来源：http://ze.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://lr.panjiajie.cn

PHP:  // 手写递归交换
来源：http://mx.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://ka.asd995.cn

TS:   // 手写回溯递归
来源：http://kn.9csxet.cn

Java: // 手写回溯递归
来源：http://am.9csxet.cn

Go:   // 手写回溯递归
来源：http://dz.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://wt.hnjuh.cn

C#:   // 手写回溯递归
来源：http://sn.shtwfgs.cn

[N09] 栈与队列
来源：http://ph.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cw.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://il.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yd.9csxet.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ku.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zu.szsharing.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gl.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xp.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uw.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://uo.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hb.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yk.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ik.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ho.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://pb.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://el.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sc.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pq.nicolike.cn

[N11] 二叉树中序遍历
来源：http://rg.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lx.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://rx.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wa.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kq.colortex.cn

Java: // 手写递归
来源：http://li.huanxung.cn

Go:   // 手写递归
来源：http://ss.9csxet.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wg.wgjwhj.cn

C#:   // 手写递归
来源：http://pl.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jk.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yq.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://od.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ya.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://km.wgjwhj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ja.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ya.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cm.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cv.bjjhwx.cn

================================================================================
来源：http://gr.muxihuayi.cn

O. 并发与异步
来源：http://hh.muxihuayi.cn

================================================================================
来源：http://st.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://kp.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ih.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uv.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fx.hahajie.cn

TS:   // 同 JS
来源：http://qb.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://pu.huanxung.cn

Go:   go f()
来源：http://yr.nicolike.cn

Ruby: Thread.new { f }
来源：http://om.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://gg.bookmarksfly.cn

[O02] 使用线程池
来源：http://vv.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gq.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nu.asd995.cn

JS:   // worker_threads 线程池
来源：http://sd.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://xm.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nr.jctech888.com.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ts.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tj.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ih.huixiangedu.cn

[O03] 加锁保护共享数据
来源：http://ha.newstarts.cn

Py:   with lock: shared += 1
来源：http://xn.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://tr.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yv.521024.cn

TS:   // 同 JS
来源：http://tm.huanxung.cn

Java: synchronized (this) { shared++; }
来源：http://tb.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wh.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vm.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://tc.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://we.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://cz.huixiangedu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ei.huanxung.cn

JS:   async function f() { await g(); }
来源：http://sd.nicolike.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ii.szxytkj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vk.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tt.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jr.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://lk.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://qi.panjiajie.cn

Py:   asyncio.gather(*tasks)
来源：http://fw.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gn.panjiajie.cn

JS:   await Promise.all(tasks)
来源：http://jt.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://wj.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mu.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lw.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://ek.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://io.huixinmuqiang.cn

[O06] 使用进程池
来源：http://eq.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nw.shxzskj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ok.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://dd.521024.cn

TS:   // child_process / cluster 模块
来源：http://jm.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ov.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://to.huixiangedu.cn

Ruby: // fork 块
来源：http://no.hnjuh.cn

C#:   Parallel.For
来源：http://oe.hahajie.cn

================================================================================
来源：http://fc.hnjuh.cn

P. 常用工具函数
来源：http://yh.shtwfgs.cn

================================================================================
来源：http://hr.shxzskj.cn

[P01] 生成 UUID
来源：http://hw.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://aw.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jx.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://di.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://zb.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://wn.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://wo.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://sc.9csxet.cn


<!-- 参考信息 -->