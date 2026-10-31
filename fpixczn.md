代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://ow.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qx.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://th.521024.cn

[L02] 发送 POST JSON
来源：http://eo.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fi.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iw.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://py.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dt.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qq.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uq.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ap.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xv.gzmigu.cn

[L03] 设置自定义请求头
来源：http://ko.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://od.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cs.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ml.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fu.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mr.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bs.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lt.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rc.panjiajie.cn

[L04] 设置超时
来源：http://oz.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://ai.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vv.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://af.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ov.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ek.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ru.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ad.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iu.colortex.cn

[L05] 上传文件（multipart）
来源：http://pe.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lg.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yv.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gi.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ra.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yj.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qa.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dr.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xw.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://bc.bjjhwx.cn

Py:   resp.json()
来源：http://zs.hahajie.cn

PHP:  json_decode($body, true);
来源：http://es.muxihuayi.cn

JS:   await resp.json()
来源：http://qy.shtwfgs.cn

TS:   await resp.json()
来源：http://dx.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xg.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dt.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://do.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://np.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://sv.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lk.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hp.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://cr.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://wr.newstarts.cn

Java: resp.statusCode()
来源：http://fj.chemitech.net.cn

Go:   resp.StatusCode
来源：http://sj.521024.cn

Ruby: resp.code.to_i
来源：http://aw.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://mf.hnjuh.cn

[L08] 并发请求多个地址
来源：http://mo.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tm.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://zg.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nu.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xg.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://th.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zt.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://er.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zy.jianghongdianzi.cn

================================================================================
来源：http://mz.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://cs.newstarts.cn

================================================================================
来源：http://gu.colortex.cn

[M01] 读取命令行参数
来源：http://rb.szxytkj.cn

Py:   sys.argv[1:]
来源：http://gz.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://do.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://km.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://eb.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://ch.shxzskj.cn

Go:   os.Args[1:]
来源：http://yx.bookmarksfly.cn

Ruby: ARGV
来源：http://qx.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://xy.haigaiapp.cn

[M02] 读取环境变量
来源：http://kn.colortex.cn

Py:   os.environ.get("HOME")
来源：http://vp.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ft.szsharing.cn

JS:   process.env.HOME
来源：http://wl.hnjuh.cn

TS:   process.env.HOME
来源：http://im.nicolike.cn

Java: System.getenv("HOME")
来源：http://pd.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xp.hahajie.cn

Ruby: ENV["HOME"]
来源：http://qk.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ix.chemitech.net.cn

[M03] 执行外部命令
来源：http://ft.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://op.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jw.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ul.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dr.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gk.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qx.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nb.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://cz.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://wh.colortex.cn

Py:   os.getcwd()
来源：http://wf.gzmigu.cn

PHP:  getcwd();
来源：http://fm.shtwfgs.cn

JS:   process.cwd()
来源：http://gm.huanxung.cn

TS:   process.cwd()
来源：http://nf.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://yq.jctech888.com.cn

Go:   os.Getwd()
来源：http://zu.nicolike.cn

Ruby: Dir.pwd
来源：http://il.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dr.hahajie.cn

[M05] 设置退出码
来源：http://po.bjjhwx.cn

Py:   sys.exit(1)
来源：http://jn.huanxung.cn

PHP:  exit(1);
来源：http://rw.521024.cn

JS:   process.exit(1)
来源：http://wh.bookmarksfly.cn

TS:   process.exit(1)
来源：http://pz.haigaiapp.cn

Java: System.exit(1)
来源：http://cp.hahajie.cn

Go:   os.Exit(1)
来源：http://aq.wgjwhj.cn

Ruby: exit 1
来源：http://jv.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pl.hnjuh.cn

[M06] 向标准错误输出
来源：http://po.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://tu.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tv.jctech888.com.cn

JS:   console.error("err")
来源：http://qw.szsharing.cn

TS:   console.error("err")
来源：http://cg.nszjky.cn

Java: System.err.println("err")
来源：http://yu.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gj.szxytkj.cn

Ruby: warn "err"
来源：http://ew.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://be.shxzskj.cn

[M07] 判断是否为主入口
来源：http://ml.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://bm.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ri.panjiajie.cn

JS:   require.main === module
来源：http://wu.gzmigu.cn

TS:   require.main === module
来源：http://wn.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://lm.newstarts.cn

Go:   func main()
来源：http://it.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yr.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://xr.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://sm.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://pd.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://xv.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://jc.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://jl.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ig.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xw.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gp.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ut.huixinmuqiang.cn

================================================================================
来源：http://nr.huixiangedu.cn

N. 数据结构与算法
来源：http://lr.hnjuh.cn

================================================================================
来源：http://fv.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://wa.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yx.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mr.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ag.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://py.szxytkj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wq.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://fg.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cf.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qe.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://ea.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://ig.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ok.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lh.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dr.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://zm.nszjky.cn

Ruby: arr.sort
来源：http://ee.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mw.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://io.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ko.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://sa.shxzskj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iq.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hd.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aq.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://de.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ts.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ya.wgjwhj.cn

[N04] 斐波那契数列
来源：http://ch.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vg.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bu.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ec.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bs.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ik.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://am.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sa.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mf.szxytkj.cn

[N05] 最大公约数
来源：http://lt.colortex.cn

Py:   math.gcd(a, b)
来源：http://cd.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hk.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cn.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ns.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hq.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fk.shxzukj.cn

Ruby: a.gcd(b)
来源：http://qp.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://px.nszjky.cn

[N06] 判断回文字符串
来源：http://li.shtwfgs.cn

Py:   s == s[::-1]
来源：http://cq.nszjky.cn

PHP:  $s === strrev($s);
来源：http://ui.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://bs.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://qq.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cy.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://dd.muxihuayi.cn

Ruby: s == s.reverse
来源：http://ud.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mz.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://ca.muxihuayi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wr.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ct.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ms.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://fh.asd995.cn

Java: // 手写 HashMap
来源：http://sp.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://hk.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://cm.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sv.asd995.cn

[N08] 生成全排列
来源：http://ct.colortex.cn

Py:   itertools.permutations(arr)
来源：http://jh.lnxyls.cn

PHP:  // 手写递归交换
来源：http://ur.nicolike.cn

JS:   // 手写回溯递归
来源：http://ed.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://as.521024.cn

Java: // 手写回溯递归
来源：http://iy.huanxung.cn

Go:   // 手写回溯递归
来源：http://pt.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://lh.hahajie.cn

C#:   // 手写回溯递归
来源：http://hx.szsharing.cn

[N09] 栈与队列
来源：http://ba.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fv.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gf.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pc.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ms.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ij.haigaiapp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zo.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rq.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aw.newstarts.cn

[N10] 链表节点定义
来源：http://gl.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hl.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jf.szxytkj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aa.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pf.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://dl.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vk.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bg.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://en.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://wv.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xb.9csxet.cn

PHP:  // 手写递归函数
来源：http://jy.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bb.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sw.bjjhwx.cn

Java: // 手写递归
来源：http://yu.asd995.cn

Go:   // 手写递归
来源：http://wi.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ar.muxihuayi.cn

C#:   // 手写递归
来源：http://zf.colortex.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bx.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kl.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rb.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zy.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pl.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pk.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://de.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://es.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qp.huixiangedu.cn

================================================================================
来源：http://ub.9csxet.cn

O. 并发与异步
来源：http://jd.yuntaijiaju.cn

================================================================================
来源：http://es.szsharing.cn

[O01] 启动一个线程
来源：http://ha.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://za.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vc.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vr.9csxet.cn

TS:   // 同 JS
来源：http://kp.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://sq.jianghongdianzi.cn

Go:   go f()
来源：http://ad.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://xt.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://om.bookmarksfly.cn

[O02] 使用线程池
来源：http://vr.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eu.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iu.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://yt.colortex.cn

TS:   // worker_threads 线程池
来源：http://qs.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kw.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hu.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fk.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://og.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://im.nicolike.cn

Py:   with lock: shared += 1
来源：http://uo.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://qc.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cu.wgjwhj.cn

TS:   // 同 JS
来源：http://uy.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://lc.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bv.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fy.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://wq.nicolike.cn

[O04] 定义异步函数并等待
来源：http://kr.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://du.521024.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xa.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://tb.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dt.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jh.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vc.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://up.colortex.cn

C#:   async Task F() { await G(); }
来源：http://ub.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://ka.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://zx.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ui.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://vw.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://vy.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gj.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jx.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://ki.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ui.szxytkj.cn


<!-- 参考信息 -->