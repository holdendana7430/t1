代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://xc.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wc.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oo.9csxet.cn

[L02] 发送 POST JSON
来源：http://hy.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ie.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pd.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tb.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ci.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ye.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ic.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ju.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wn.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://zc.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ks.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://di.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dq.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qh.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yt.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lw.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uf.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://at.bjjhwx.cn

[L04] 设置超时
来源：http://hl.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://ar.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xn.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qi.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wg.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lx.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ok.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yz.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vd.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://mt.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eo.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cs.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tl.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://py.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dp.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://br.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tp.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lu.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://pt.asd995.cn

Py:   resp.json()
来源：http://sz.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://ef.muxihuayi.cn

JS:   await resp.json()
来源：http://xf.bookmarksfly.cn

TS:   await resp.json()
来源：http://qy.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iv.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cz.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://np.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ej.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://gw.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://af.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://le.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://yp.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://av.shtwfgs.cn

Java: resp.statusCode()
来源：http://ba.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://et.hnjuh.cn

Ruby: resp.code.to_i
来源：http://qg.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://uq.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://dn.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ee.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://hp.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xs.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vc.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ze.yuntaijiaju.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pa.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qe.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lb.newstarts.cn

================================================================================
来源：http://ep.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://hz.nszjky.cn

================================================================================
来源：http://pv.haigaiapp.cn

[M01] 读取命令行参数
来源：http://ms.nicolike.cn

Py:   sys.argv[1:]
来源：http://vq.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://di.nicolike.cn

JS:   process.argv.slice(2)
来源：http://sa.newstarts.cn

TS:   process.argv.slice(2)
来源：http://ty.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://rr.colortex.cn

Go:   os.Args[1:]
来源：http://ro.shxzskj.cn

Ruby: ARGV
来源：http://hd.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://gq.shxzskj.cn

[M02] 读取环境变量
来源：http://cl.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://ea.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cl.gzmigu.cn

JS:   process.env.HOME
来源：http://hh.bjjhwx.cn

TS:   process.env.HOME
来源：http://ff.szsharing.cn

Java: System.getenv("HOME")
来源：http://qk.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mo.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://kx.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vm.wgjwhj.cn

[M03] 执行外部命令
来源：http://fg.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wd.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jv.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xt.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bq.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wh.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ow.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kz.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://mo.asd995.cn

[M04] 获取当前工作目录
来源：http://aq.chemitech.net.cn

Py:   os.getcwd()
来源：http://wz.szxytkj.cn

PHP:  getcwd();
来源：http://cm.hahajie.cn

JS:   process.cwd()
来源：http://ji.wgjwhj.cn

TS:   process.cwd()
来源：http://la.chemitech.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://lt.nszjky.cn

Go:   os.Getwd()
来源：http://wb.huanxung.cn

Ruby: Dir.pwd
来源：http://td.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://um.chemitech.net.cn

[M05] 设置退出码
来源：http://fn.szsharing.cn

Py:   sys.exit(1)
来源：http://ni.asd995.cn

PHP:  exit(1);
来源：http://oy.521024.cn

JS:   process.exit(1)
来源：http://io.newstarts.cn

TS:   process.exit(1)
来源：http://dx.lnxyls.cn

Java: System.exit(1)
来源：http://mv.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://od.gzmigu.cn

Ruby: exit 1
来源：http://hd.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ze.colortex.cn

[M06] 向标准错误输出
来源：http://am.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://rm.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ec.szsharing.cn

JS:   console.error("err")
来源：http://ct.haigaiapp.cn

TS:   console.error("err")
来源：http://hn.9csxet.cn

Java: System.err.println("err")
来源：http://jh.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://be.szsharing.cn

Ruby: warn "err"
来源：http://ps.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://xw.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://vt.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://jh.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xn.shtwfgs.cn

JS:   require.main === module
来源：http://za.muxihuayi.cn

TS:   require.main === module
来源：http://mr.szxytkj.cn

Java: public static void main(String[] args)
来源：http://tj.chemitech.net.cn

Go:   func main()
来源：http://fc.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mw.9csxet.cn

C#:   static void Main(string[] args)
来源：http://sn.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://so.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://lf.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://pq.shxzukj.cn

JS:   process.platform;  process.version
来源：http://va.huanxung.cn

TS:   process.platform;  process.version
来源：http://pa.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pe.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zv.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sv.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nr.huixinmuqiang.cn

================================================================================
来源：http://tm.nszjky.cn

N. 数据结构与算法
来源：http://ec.gzmigu.cn

================================================================================
来源：http://zh.asd995.cn

[N01] 二分查找（有序数组）
来源：http://uh.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vg.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://if.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://li.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gz.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xh.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://yo.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lp.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://no.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://ig.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://fi.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ww.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qw.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zl.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ms.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://ch.newstarts.cn

Ruby: arr.sort
来源：http://gd.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mh.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://vz.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hf.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://tg.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://po.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ha.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zd.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ks.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oo.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nl.szxytkj.cn

[N04] 斐波那契数列
来源：http://na.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aw.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hx.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fl.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fl.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ld.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fh.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fp.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sb.nicolike.cn

[N05] 最大公约数
来源：http://cs.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://cw.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vu.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hs.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ed.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cf.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vl.gzmigu.cn

Ruby: a.gcd(b)
来源：http://ou.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xs.shxzskj.cn

[N06] 判断回文字符串
来源：http://wx.asd995.cn

Py:   s == s[::-1]
来源：http://yw.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://df.panjiajie.cn

JS:   s === [...s].reverse().join("")
来源：http://rx.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://jd.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mz.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://fz.521024.cn

Ruby: s == s.reverse
来源：http://bi.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cd.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://vd.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ub.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yt.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xc.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://yd.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://tf.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://yx.nicolike.cn

Ruby: // 手写 Hash
来源：http://zq.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qj.yuntaijiaju.cn

[N08] 生成全排列
来源：http://oh.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://me.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://rt.nszjky.cn

JS:   // 手写回溯递归
来源：http://dx.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://yw.gzmigu.cn

Java: // 手写回溯递归
来源：http://wi.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://mq.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://el.szsharing.cn

C#:   // 手写回溯递归
来源：http://pc.jctech888.com.cn

[N09] 栈与队列
来源：http://ca.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yx.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gn.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ll.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pb.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mv.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tw.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xr.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rh.szxytkj.cn

[N10] 链表节点定义
来源：http://ny.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bs.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://li.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sr.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xh.521024.cn

Java: class Node { int v; Node next; }
来源：http://wu.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hy.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qh.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ra.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://zi.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cx.newstarts.cn

PHP:  // 手写递归函数
来源：http://tk.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://il.szsharing.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kl.wgjwhj.cn

Java: // 手写递归
来源：http://xd.521024.cn

Go:   // 手写递归
来源：http://uy.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dn.haigaiapp.cn

C#:   // 手写递归
来源：http://ee.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jn.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wl.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://eu.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ec.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ru.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ve.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ob.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fs.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kc.huanxung.cn

================================================================================
来源：http://yw.yuntaijiaju.cn

O. 并发与异步
来源：http://xu.szsharing.cn

================================================================================
来源：http://bh.chemitech.net.cn

[O01] 启动一个线程
来源：http://nd.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fl.bookmarksfly.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zo.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kk.wgjwhj.cn

TS:   // 同 JS
来源：http://fa.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://fc.gzmigu.cn

Go:   go f()
来源：http://vl.gzmigu.cn

Ruby: Thread.new { f }
来源：http://kl.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://ra.shxzukj.cn

[O02] 使用线程池
来源：http://ip.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ju.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rh.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://ns.nicolike.cn

TS:   // worker_threads 线程池
来源：http://bm.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uw.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://af.huanxung.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rb.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zs.521024.cn

[O03] 加锁保护共享数据
来源：http://pe.panjiajie.cn

Py:   with lock: shared += 1
来源：http://dc.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ug.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sm.muxihuayi.cn

TS:   // 同 JS
来源：http://vh.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://mw.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cd.szsharing.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://so.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://vw.hahajie.cn

[O04] 定义异步函数并等待
来源：http://bf.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://mi.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ey.nicolike.cn

JS:   async function f() { await g(); }
来源：http://ey.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kd.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ii.yuntaijiaju.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dj.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nu.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://vx.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://mh.yuexingan06.cn

Py:   asyncio.gather(*tasks)
来源：http://bm.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rx.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://qi.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://em.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tx.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ab.colortex.cn

Ruby: threads.map(&:join)
来源：http://vy.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kc.szxytkj.cn


<!-- 参考信息 -->