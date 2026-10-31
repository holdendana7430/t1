代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ij.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nq.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vu.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zg.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zv.huanxung.cn

[L04] 设置超时
来源：http://ug.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://eu.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ui.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cz.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ke.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yf.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vg.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qr.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uw.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://md.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ap.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gq.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ib.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://id.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vd.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ek.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mo.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sp.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://rp.bookmarksfly.cn

Py:   resp.json()
来源：http://bc.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://pw.szsharing.cn

JS:   await resp.json()
来源：http://id.chemitech.net.cn

TS:   await resp.json()
来源：http://ty.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kp.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ac.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://ko.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ud.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://gw.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://es.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ku.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://bm.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://nv.shtwfgs.cn

Java: resp.statusCode()
来源：http://qk.newstarts.cn

Go:   resp.StatusCode
来源：http://ij.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://tb.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://mc.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://nj.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ij.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://ko.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xd.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qt.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hv.yuntaijiaju.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hl.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vz.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yb.nszjky.cn

================================================================================
来源：http://dr.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://yi.shxzukj.cn

================================================================================
来源：http://bw.lnxyls.cn

[M01] 读取命令行参数
来源：http://he.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://yx.nszjky.cn

PHP:  $argv;  $argc;
来源：http://hl.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://rm.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://sw.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://wt.bjjhwx.cn

Go:   os.Args[1:]
来源：http://xa.lnxyls.cn

Ruby: ARGV
来源：http://yq.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://ns.nicolike.cn

[M02] 读取环境变量
来源：http://ql.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://dm.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ms.szsharing.cn

JS:   process.env.HOME
来源：http://it.jctech888.com.cn

TS:   process.env.HOME
来源：http://zb.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://no.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aw.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://md.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wa.chemitech.net.cn

[M03] 执行外部命令
来源：http://kw.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fw.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uh.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qw.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vw.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ki.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pk.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ol.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://ag.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://zm.hahajie.cn

Py:   os.getcwd()
来源：http://xq.huixiangedu.cn

PHP:  getcwd();
来源：http://fs.shxzskj.cn

JS:   process.cwd()
来源：http://zb.huixinmuqiang.cn

TS:   process.cwd()
来源：http://jq.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://am.haigaiapp.cn

Go:   os.Getwd()
来源：http://di.newstarts.cn

Ruby: Dir.pwd
来源：http://al.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yb.huixinmuqiang.cn

[M05] 设置退出码
来源：http://nc.muxihuayi.cn

Py:   sys.exit(1)
来源：http://tz.muxihuayi.cn

PHP:  exit(1);
来源：http://ly.bookmarksfly.cn

JS:   process.exit(1)
来源：http://wo.newstarts.cn

TS:   process.exit(1)
来源：http://sj.asd995.cn

Java: System.exit(1)
来源：http://ir.hahajie.cn

Go:   os.Exit(1)
来源：http://wo.nszjky.cn

Ruby: exit 1
来源：http://ns.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rw.panjiajie.cn

[M06] 向标准错误输出
来源：http://bo.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://jh.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ja.9csxet.cn

JS:   console.error("err")
来源：http://xv.huanxung.cn

TS:   console.error("err")
来源：http://li.nicolike.cn

Java: System.err.println("err")
来源：http://wn.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cz.jianghongdianzi.cn

Ruby: warn "err"
来源：http://jm.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://oq.szxytkj.cn

[M07] 判断是否为主入口
来源：http://ld.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://fr.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rw.9csxet.cn

JS:   require.main === module
来源：http://fj.shxzukj.cn

TS:   require.main === module
来源：http://wy.szxytkj.cn

Java: public static void main(String[] args)
来源：http://cq.newstarts.cn

Go:   func main()
来源：http://is.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vh.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://rb.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://ur.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://ow.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://rr.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://dt.szsharing.cn

TS:   process.platform;  process.version
来源：http://mk.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xd.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qv.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rm.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gt.jianghongdianzi.cn

================================================================================
来源：http://ap.nszjky.cn

N. 数据结构与算法
来源：http://zv.yuntaijiaju.cn

================================================================================
来源：http://id.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://rb.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fh.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rk.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uo.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mm.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mn.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://cb.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uk.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qv.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://km.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://tc.jianghongdianzi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xp.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zg.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zr.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yx.nicolike.cn

Go:   slices.Sort(arr)
来源：http://in.chemitech.net.cn

Ruby: arr.sort
来源：http://zj.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jm.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://cf.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vk.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://pe.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lp.panjiajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kz.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://av.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pv.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yc.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ua.shtwfgs.cn

[N04] 斐波那契数列
来源：http://zu.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ny.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bn.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ua.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wi.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yz.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ov.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cv.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ac.muxihuayi.cn

[N05] 最大公约数
来源：http://vk.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://pq.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ul.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ol.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rf.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zo.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://my.szsharing.cn

Ruby: a.gcd(b)
来源：http://be.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ek.haigaiapp.cn

[N06] 判断回文字符串
来源：http://pb.szxytkj.cn

Py:   s == s[::-1]
来源：http://ym.szsharing.cn

PHP:  $s === strrev($s);
来源：http://ub.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://uh.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://hz.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pl.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://mf.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://zm.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cx.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://we.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qb.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nt.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://la.521024.cn

TS:   // 手写 Map<string, number>
来源：http://iv.jctech888.com.cn

Java: // 手写 HashMap
来源：http://kb.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://be.shxzskj.cn

Ruby: // 手写 Hash
来源：http://tx.shxzskj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sm.yuexingan06.cn

[N08] 生成全排列
来源：http://yn.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://qi.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://kc.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://in.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://rd.nicolike.cn

Java: // 手写回溯递归
来源：http://jj.gzmigu.cn

Go:   // 手写回溯递归
来源：http://id.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://ht.szsharing.cn

C#:   // 手写回溯递归
来源：http://gd.jctech888.com.cn

[N09] 栈与队列
来源：http://rm.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nv.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kr.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://da.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ik.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jy.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ty.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://no.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kn.huanxung.cn

[N10] 链表节点定义
来源：http://iw.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lh.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wd.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nl.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ue.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://ge.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gn.colortex.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vp.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mm.9csxet.cn

[N11] 二叉树中序遍历
来源：http://xy.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ry.nszjky.cn

PHP:  // 手写递归函数
来源：http://uh.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sg.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xi.lnxyls.cn

Java: // 手写递归
来源：http://tv.bjjhwx.cn

Go:   // 手写递归
来源：http://eg.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fq.asd995.cn

C#:   // 手写递归
来源：http://ds.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://af.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dn.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://na.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://at.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gt.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://df.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zm.jianghongdianzi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vf.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xq.haigaiapp.cn

================================================================================
来源：http://sq.nszjky.cn

O. 并发与异步
来源：http://uh.szsharing.cn

================================================================================
来源：http://jk.nicolike.cn

[O01] 启动一个线程
来源：http://sq.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mt.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yx.huixinmuqiang.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rm.wgjwhj.cn

TS:   // 同 JS
来源：http://nd.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://cl.jianghongdianzi.cn

Go:   go f()
来源：http://ox.panjiajie.cn

Ruby: Thread.new { f }
来源：http://gk.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://hn.newstarts.cn

[O02] 使用线程池
来源：http://fu.wgjwhj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tc.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oo.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://nf.szsharing.cn

TS:   // worker_threads 线程池
来源：http://qb.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ic.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wn.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://is.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rs.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://nm.szsharing.cn

Py:   with lock: shared += 1
来源：http://fp.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://fc.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gy.yuntaijiaju.cn

TS:   // 同 JS
来源：http://ni.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://kx.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qa.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cl.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://cw.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://mj.asd995.cn

Py:   async def f():⏎    await g()
来源：http://ff.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rc.nszjky.cn

JS:   async function f() { await g(); }
来源：http://mg.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ph.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nm.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mb.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://my.colortex.cn

C#:   async Task F() { await G(); }
来源：http://lo.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://uo.panjiajie.cn

Py:   asyncio.gather(*tasks)
来源：http://et.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qk.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://on.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://zk.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bg.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zl.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://cw.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fb.huixinmuqiang.cn

[O06] 使用进程池
来源：http://jm.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://za.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xp.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://zu.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://tu.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ty.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fl.yuntaijiaju.cn

Ruby: // fork 块
来源：http://iu.gzmigu.cn

C#:   Parallel.For
来源：http://yx.lnxyls.cn

================================================================================
来源：http://ju.yuntaijiaju.cn

P. 常用工具函数
来源：http://cl.shxzukj.cn

================================================================================
来源：http://st.jctech888.com.cn

[P01] 生成 UUID
来源：http://px.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://zm.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dp.9csxet.cn

JS:   crypto.randomUUID()
来源：http://cq.yuexingan06.cn


<!-- 参考信息 -->