代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oq.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rv.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uj.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pq.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vi.bjjhwx.cn

[L04] 设置超时
来源：http://ex.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://ua.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rz.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ke.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ez.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://is.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gj.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://of.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ju.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://ck.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dy.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xq.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://au.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rr.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ec.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://da.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://if.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xq.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://lu.huanxung.cn

Py:   resp.json()
来源：http://lm.nszjky.cn

PHP:  json_decode($body, true);
来源：http://fd.huixiangedu.cn

JS:   await resp.json()
来源：http://dl.521024.cn

TS:   await resp.json()
来源：http://hf.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://id.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kb.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://fg.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zl.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://ez.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ly.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yo.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://aj.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://cv.jctech888.com.cn

Java: resp.statusCode()
来源：http://al.bjjhwx.cn

Go:   resp.StatusCode
来源：http://qb.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://ql.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://oi.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://wf.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bp.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://dq.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://om.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ig.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dg.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pu.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ka.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dz.nszjky.cn

================================================================================
来源：http://cu.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://xw.muxihuayi.cn

================================================================================
来源：http://bg.chemitech.net.cn

[M01] 读取命令行参数
来源：http://rz.9csxet.cn

Py:   sys.argv[1:]
来源：http://gw.colortex.cn

PHP:  $argv;  $argc;
来源：http://iq.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://bs.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://nu.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://lz.hahajie.cn

Go:   os.Args[1:]
来源：http://iu.gzmigu.cn

Ruby: ARGV
来源：http://el.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://ir.hnjuh.cn

[M02] 读取环境变量
来源：http://ub.521024.cn

Py:   os.environ.get("HOME")
来源：http://pp.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lb.wgjwhj.cn

JS:   process.env.HOME
来源：http://md.nszjky.cn

TS:   process.env.HOME
来源：http://dw.szxytkj.cn

Java: System.getenv("HOME")
来源：http://bw.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aj.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://ss.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ss.lnxyls.cn

[M03] 执行外部命令
来源：http://rx.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ut.muxihuayi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rb.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pf.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ip.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yo.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mc.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wl.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://zg.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://hi.gzmigu.cn

Py:   os.getcwd()
来源：http://uk.nszjky.cn

PHP:  getcwd();
来源：http://qg.huixinmuqiang.cn

JS:   process.cwd()
来源：http://yx.nicolike.cn

TS:   process.cwd()
来源：http://yt.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://fr.hnjuh.cn

Go:   os.Getwd()
来源：http://fj.asd995.cn

Ruby: Dir.pwd
来源：http://fd.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hq.gzmigu.cn

[M05] 设置退出码
来源：http://qf.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://yk.gzmigu.cn

PHP:  exit(1);
来源：http://wq.chemitech.net.cn

JS:   process.exit(1)
来源：http://oc.nszjky.cn

TS:   process.exit(1)
来源：http://cv.muxihuayi.cn

Java: System.exit(1)
来源：http://mz.asd995.cn

Go:   os.Exit(1)
来源：http://wa.szxytkj.cn

Ruby: exit 1
来源：http://bq.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pt.shxzukj.cn

[M06] 向标准错误输出
来源：http://xo.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://iq.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hx.newstarts.cn

JS:   console.error("err")
来源：http://ng.shxzukj.cn

TS:   console.error("err")
来源：http://ak.newstarts.cn

Java: System.err.println("err")
来源：http://eh.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://al.9csxet.cn

Ruby: warn "err"
来源：http://tb.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://ck.asd995.cn

[M07] 判断是否为主入口
来源：http://ao.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://mx.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ja.hahajie.cn

JS:   require.main === module
来源：http://dz.nicolike.cn

TS:   require.main === module
来源：http://qx.panjiajie.cn

Java: public static void main(String[] args)
来源：http://qf.jianghongdianzi.cn

Go:   func main()
来源：http://bi.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vw.newstarts.cn

C#:   static void Main(string[] args)
来源：http://bl.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://sw.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://xs.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://jj.szxytkj.cn

JS:   process.platform;  process.version
来源：http://ht.521024.cn

TS:   process.platform;  process.version
来源：http://nn.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://he.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yn.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dw.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uc.yuexingan06.cn

================================================================================
来源：http://xg.huixinmuqiang.cn

N. 数据结构与算法
来源：http://jz.shxzukj.cn

================================================================================
来源：http://li.asd995.cn

[N01] 二分查找（有序数组）
来源：http://de.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mv.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://us.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oi.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bq.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ea.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://zg.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gl.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xs.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://km.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://rr.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qm.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dq.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pq.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ex.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://bn.bjjhwx.cn

Ruby: arr.sort
来源：http://dn.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yd.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://ot.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ku.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://dj.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fm.wgjwhj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bj.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ej.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eh.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ak.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rq.panjiajie.cn

[N04] 斐波那契数列
来源：http://ws.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hq.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xu.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ux.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ul.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ya.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uy.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ec.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gn.bjjhwx.cn

[N05] 最大公约数
来源：http://dp.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://ij.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://il.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zz.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dp.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cv.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lp.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://rj.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jn.panjiajie.cn

[N06] 判断回文字符串
来源：http://ve.521024.cn

Py:   s == s[::-1]
来源：http://xw.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://id.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://av.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://im.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hw.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://lg.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://uk.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zq.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://co.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fq.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yt.bookmarksfly.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cd.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://pj.hnjuh.cn

Java: // 手写 HashMap
来源：http://ah.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://lk.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://wg.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wn.hahajie.cn

[N08] 生成全排列
来源：http://ox.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://pt.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://km.colortex.cn

JS:   // 手写回溯递归
来源：http://cr.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://gm.shxzskj.cn

Java: // 手写回溯递归
来源：http://sd.shxzukj.cn

Go:   // 手写回溯递归
来源：http://yo.jianghongdianzi.cn

Ruby: arr.permutation.to_a
来源：http://qc.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://be.yuexingan06.cn

[N09] 栈与队列
来源：http://tr.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tc.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qv.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ha.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iz.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pp.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ft.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jg.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ib.9csxet.cn

[N10] 链表节点定义
来源：http://xh.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kv.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fs.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nz.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wf.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://wf.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fv.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qu.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tm.huanxung.cn

[N11] 二叉树中序遍历
来源：http://hj.bookmarksfly.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ju.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://ng.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ys.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gg.haigaiapp.cn

Java: // 手写递归
来源：http://az.asd995.cn

Go:   // 手写递归
来源：http://tu.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zx.shxzskj.cn

C#:   // 手写递归
来源：http://mi.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hq.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eu.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://du.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qn.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xh.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qq.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://an.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ss.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qd.shxzskj.cn

================================================================================
来源：http://ns.bookmarksfly.cn

O. 并发与异步
来源：http://wg.jianghongdianzi.cn

================================================================================
来源：http://km.bookmarksfly.cn

[O01] 启动一个线程
来源：http://vd.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kb.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ye.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rk.colortex.cn

TS:   // 同 JS
来源：http://rs.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://bn.shtwfgs.cn

Go:   go f()
来源：http://zz.9csxet.cn

Ruby: Thread.new { f }
来源：http://ku.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://gt.huixiangedu.cn

[O02] 使用线程池
来源：http://af.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tt.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://em.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://mo.huixiangedu.cn

TS:   // worker_threads 线程池
来源：http://ru.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yr.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sh.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fh.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gi.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://mr.newstarts.cn

Py:   with lock: shared += 1
来源：http://ov.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://lj.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wg.nicolike.cn

TS:   // 同 JS
来源：http://hv.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://mw.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pt.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kc.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://sn.521024.cn

[O04] 定义异步函数并等待
来源：http://hg.asd995.cn

Py:   async def f():⏎    await g()
来源：http://ae.gzmigu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bj.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://im.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nv.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://je.yuntaijiaju.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nw.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xj.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://dj.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://qy.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://sj.muxihuayi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sp.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://hr.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://ey.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iy.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nc.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://cl.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hh.newstarts.cn

[O06] 使用进程池
来源：http://fr.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cl.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://oh.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://ui.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://yc.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tj.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cc.szsharing.cn

Ruby: // fork 块
来源：http://cj.521024.cn

C#:   Parallel.For
来源：http://bs.9csxet.cn

================================================================================
来源：http://pz.yuexingan06.cn

P. 常用工具函数
来源：http://zq.colortex.cn

================================================================================
来源：http://rp.9csxet.cn

[P01] 生成 UUID
来源：http://pe.jctech888.com.cn

Py:   str(uuid.uuid4())
来源：http://np.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gt.nszjky.cn

JS:   crypto.randomUUID()
来源：http://ws.panjiajie.cn


<!-- 参考信息 -->