代发 wailian999

[L03] 设置自定义请求头
来源：http://ba.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tl.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hq.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pl.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ce.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ya.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hb.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ra.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jb.521024.cn

[L04] 设置超时
来源：http://ng.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://so.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iy.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zc.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qt.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xg.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://on.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zf.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cw.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://pp.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sf.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cl.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gd.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fp.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lu.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fs.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ma.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bq.colortex.cn

[L06] 解析响应为 JSON
来源：http://th.newstarts.cn

Py:   resp.json()
来源：http://ar.nicolike.cn

PHP:  json_decode($body, true);
来源：http://jd.asd995.cn

JS:   await resp.json()
来源：http://jl.colortex.cn

TS:   await resp.json()
来源：http://ms.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tx.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iv.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://db.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iv.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://av.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bz.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ew.521024.cn

JS:   resp.ok;  resp.status
来源：http://lb.521024.cn

TS:   resp.ok;  resp.status
来源：http://eg.muxihuayi.cn

Java: resp.statusCode()
来源：http://aw.szxytkj.cn

Go:   resp.StatusCode
来源：http://uq.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://nm.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://pp.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://ol.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dd.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://lh.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ji.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pp.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ot.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lz.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ww.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tt.wgjwhj.cn

================================================================================
来源：http://fr.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://oc.haigaiapp.cn

================================================================================
来源：http://sc.asd995.cn

[M01] 读取命令行参数
来源：http://pm.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://cm.szsharing.cn

PHP:  $argv;  $argc;
来源：http://cw.colortex.cn

JS:   process.argv.slice(2)
来源：http://kk.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://ra.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://qt.szxytkj.cn

Go:   os.Args[1:]
来源：http://kj.newstarts.cn

Ruby: ARGV
来源：http://ff.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://qa.haigaiapp.cn

[M02] 读取环境变量
来源：http://jp.colortex.cn

Py:   os.environ.get("HOME")
来源：http://wm.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nk.nicolike.cn

JS:   process.env.HOME
来源：http://sn.hahajie.cn

TS:   process.env.HOME
来源：http://qo.shxzukj.cn

Java: System.getenv("HOME")
来源：http://uf.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jd.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://sj.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mm.szxytkj.cn

[M03] 执行外部命令
来源：http://nq.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xd.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cr.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jn.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ep.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ic.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sh.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xv.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://gh.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://ll.muxihuayi.cn

Py:   os.getcwd()
来源：http://ps.huixinmuqiang.cn

PHP:  getcwd();
来源：http://du.hnjuh.cn

JS:   process.cwd()
来源：http://sx.lnxyls.cn

TS:   process.cwd()
来源：http://oy.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://ic.nszjky.cn

Go:   os.Getwd()
来源：http://cb.nszjky.cn

Ruby: Dir.pwd
来源：http://hp.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://og.bookmarksfly.cn

[M05] 设置退出码
来源：http://jt.shtwfgs.cn

Py:   sys.exit(1)
来源：http://cg.yuntaijiaju.cn

PHP:  exit(1);
来源：http://fj.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://eb.jctech888.com.cn

TS:   process.exit(1)
来源：http://rj.muxihuayi.cn

Java: System.exit(1)
来源：http://ce.hahajie.cn

Go:   os.Exit(1)
来源：http://zk.jianghongdianzi.cn

Ruby: exit 1
来源：http://kw.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jj.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://on.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://dt.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mm.521024.cn

JS:   console.error("err")
来源：http://wz.colortex.cn

TS:   console.error("err")
来源：http://ya.lnxyls.cn

Java: System.err.println("err")
来源：http://fw.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vi.newstarts.cn

Ruby: warn "err"
来源：http://ug.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://pb.newstarts.cn

[M07] 判断是否为主入口
来源：http://hc.panjiajie.cn

Py:   if __name__ == "__main__":
来源：http://va.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qc.asd995.cn

JS:   require.main === module
来源：http://ku.szxytkj.cn

TS:   require.main === module
来源：http://zz.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://by.huanxung.cn

Go:   func main()
来源：http://wg.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xg.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://hz.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://nx.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://jd.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://vb.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://sa.colortex.cn

TS:   process.platform;  process.version
来源：http://om.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tw.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fo.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tm.huixinmuqiang.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jl.chemitech.net.cn

================================================================================
来源：http://sf.bookmarksfly.cn

N. 数据结构与算法
来源：http://ae.gzmigu.cn

================================================================================
来源：http://va.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://ut.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sr.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lq.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://na.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://au.szxytkj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ou.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://wu.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kn.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xs.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://lu.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://cd.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mu.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://st.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ln.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ri.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://li.huixinmuqiang.cn

Ruby: arr.sort
来源：http://kn.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qw.521024.cn

[N03] 快速排序（分治示例）
来源：http://nm.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://na.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://gm.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hl.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tl.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cc.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gt.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wa.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gh.huanxung.cn

[N04] 斐波那契数列
来源：http://rw.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ib.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hu.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ca.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bz.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rk.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oo.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ad.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://az.asd995.cn

[N05] 最大公约数
来源：http://oe.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://rx.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qk.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wq.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jb.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://it.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://io.colortex.cn

Ruby: a.gcd(b)
来源：http://gp.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sc.wgjwhj.cn

[N06] 判断回文字符串
来源：http://nr.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://uo.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://xj.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://eh.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://yw.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nz.nszjky.cn

Go:   // 双指针从两端比较
来源：http://mi.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://mc.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wd.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://bb.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://js.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://er.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gt.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://is.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://kt.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://ch.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://ai.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vt.huanxung.cn

[N08] 生成全排列
来源：http://pw.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://jh.hahajie.cn

PHP:  // 手写递归交换
来源：http://gv.hahajie.cn

JS:   // 手写回溯递归
来源：http://rx.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://ul.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://cq.huanxung.cn

Go:   // 手写回溯递归
来源：http://hq.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://na.szsharing.cn

C#:   // 手写回溯递归
来源：http://jb.jctech888.com.cn

[N09] 栈与队列
来源：http://ub.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://co.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ep.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sf.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tf.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jt.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wn.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://en.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jl.shxzukj.cn

[N10] 链表节点定义
来源：http://qd.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yh.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fz.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://il.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ua.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://ig.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://im.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ys.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ba.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://nu.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ac.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://in.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sc.jctech888.com.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dc.huixinmuqiang.cn

Java: // 手写递归
来源：http://sr.huixinmuqiang.cn

Go:   // 手写递归
来源：http://xu.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ax.nszjky.cn

C#:   // 手写递归
来源：http://ar.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://up.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cg.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jn.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fx.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bi.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ux.bookmarksfly.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yp.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dc.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ha.muxihuayi.cn

================================================================================
来源：http://od.wgjwhj.cn

O. 并发与异步
来源：http://km.9csxet.cn

================================================================================
来源：http://oj.yuexingan06.cn

[O01] 启动一个线程
来源：http://om.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lo.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dt.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ua.colortex.cn

TS:   // 同 JS
来源：http://qc.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://oc.colortex.cn

Go:   go f()
来源：http://tf.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://mo.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://tb.nicolike.cn

[O02] 使用线程池
来源：http://gt.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gb.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ji.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://bv.lnxyls.cn

TS:   // worker_threads 线程池
来源：http://yk.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pk.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oi.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ai.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mk.huanxung.cn

[O03] 加锁保护共享数据
来源：http://nf.szxytkj.cn

Py:   with lock: shared += 1
来源：http://lf.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://md.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wz.shxzukj.cn

TS:   // 同 JS
来源：http://fr.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://ye.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ta.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rs.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://fe.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://tj.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://an.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vn.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://lx.nicolike.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pq.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xn.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dl.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pz.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://bp.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://qr.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://zz.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vz.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://gf.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://mo.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bb.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gd.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://qx.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fi.9csxet.cn

[O06] 使用进程池
来源：http://qd.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sd.huanxung.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://if.521024.cn

JS:   // child_process / cluster 模块
来源：http://gc.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://rh.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rh.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nh.shxzukj.cn

Ruby: // fork 块
来源：http://ar.chemitech.net.cn

C#:   Parallel.For
来源：http://pi.huanxung.cn

================================================================================
来源：http://xd.huixiangedu.cn

P. 常用工具函数
来源：http://ta.panjiajie.cn

================================================================================
来源：http://su.shxzskj.cn


<!-- 参考信息 -->