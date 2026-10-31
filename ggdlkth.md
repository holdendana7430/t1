代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://ww.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ng.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pc.lnxyls.cn

[L02] 发送 POST JSON
来源：http://hj.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gj.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://no.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://og.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fv.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ic.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gx.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://am.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xf.shxzukj.cn

[L03] 设置自定义请求头
来源：http://pl.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gh.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fa.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gz.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ng.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://io.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://un.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nl.bjjhwx.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://am.hnjuh.cn

[L04] 设置超时
来源：http://sw.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://vb.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fi.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://je.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ko.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zm.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qk.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ij.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ob.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://ce.9csxet.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zf.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bi.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qy.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://af.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cl.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ag.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rl.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ii.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://pb.szxytkj.cn

Py:   resp.json()
来源：http://ue.huanxung.cn

PHP:  json_decode($body, true);
来源：http://wf.chemitech.net.cn

JS:   await resp.json()
来源：http://ho.jianghongdianzi.cn

TS:   await resp.json()
来源：http://lg.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tb.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nt.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://zi.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jc.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://bb.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://li.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tv.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://mb.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://nd.nszjky.cn

Java: resp.statusCode()
来源：http://lw.nszjky.cn

Go:   resp.StatusCode
来源：http://sz.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://oa.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://tu.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://re.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fh.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://dj.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xp.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mm.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qj.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wn.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jo.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ma.hnjuh.cn

================================================================================
来源：http://sb.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://es.bookmarksfly.cn

================================================================================
来源：http://wa.hnjuh.cn

[M01] 读取命令行参数
来源：http://la.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://gb.nszjky.cn

PHP:  $argv;  $argc;
来源：http://bv.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://xv.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://ye.521024.cn

Java: args 数组（main 方法参数）
来源：http://dg.nszjky.cn

Go:   os.Args[1:]
来源：http://ep.9csxet.cn

Ruby: ARGV
来源：http://pw.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://ny.9csxet.cn

[M02] 读取环境变量
来源：http://kr.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://iz.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yo.huixiangedu.cn

JS:   process.env.HOME
来源：http://ns.shxzukj.cn

TS:   process.env.HOME
来源：http://lv.521024.cn

Java: System.getenv("HOME")
来源：http://hz.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cx.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://yu.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ml.jctech888.com.cn

[M03] 执行外部命令
来源：http://zq.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zw.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kc.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ro.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jx.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vt.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://no.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ha.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://ra.colortex.cn

[M04] 获取当前工作目录
来源：http://lj.bookmarksfly.cn

Py:   os.getcwd()
来源：http://km.newstarts.cn

PHP:  getcwd();
来源：http://lz.shxzskj.cn

JS:   process.cwd()
来源：http://ux.huanxung.cn

TS:   process.cwd()
来源：http://yh.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://rd.asd995.cn

Go:   os.Getwd()
来源：http://zn.lnxyls.cn

Ruby: Dir.pwd
来源：http://en.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wa.521024.cn

[M05] 设置退出码
来源：http://ut.panjiajie.cn

Py:   sys.exit(1)
来源：http://nb.huixinmuqiang.cn

PHP:  exit(1);
来源：http://qk.jctech888.com.cn

JS:   process.exit(1)
来源：http://mc.newstarts.cn

TS:   process.exit(1)
来源：http://gj.nszjky.cn

Java: System.exit(1)
来源：http://lb.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://tj.jianghongdianzi.cn

Ruby: exit 1
来源：http://rz.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ur.lnxyls.cn

[M06] 向标准错误输出
来源：http://mw.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://sr.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vh.shtwfgs.cn

JS:   console.error("err")
来源：http://sn.yuntaijiaju.cn

TS:   console.error("err")
来源：http://xa.newstarts.cn

Java: System.err.println("err")
来源：http://ye.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ca.muxihuayi.cn

Ruby: warn "err"
来源：http://kf.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://zp.shxzskj.cn

[M07] 判断是否为主入口
来源：http://ns.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://nh.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ly.szsharing.cn

JS:   require.main === module
来源：http://ve.huixiangedu.cn

TS:   require.main === module
来源：http://os.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://nm.gzmigu.cn

Go:   func main()
来源：http://ub.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zw.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://ss.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://or.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://mb.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://rn.szsharing.cn

JS:   process.platform;  process.version
来源：http://xh.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://cb.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lq.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wx.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mz.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://za.shtwfgs.cn

================================================================================
来源：http://ak.lnxyls.cn

N. 数据结构与算法
来源：http://dl.jianghongdianzi.cn

================================================================================
来源：http://sy.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://zh.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zz.szxytkj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sn.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dr.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pd.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ks.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://pv.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cg.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ik.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://ha.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://sk.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://po.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cg.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nz.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gc.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://um.bjjhwx.cn

Ruby: arr.sort
来源：http://yn.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kb.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://jk.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wf.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://qs.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bl.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lr.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mf.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uf.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bs.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tv.nszjky.cn

[N04] 斐波那契数列
来源：http://pl.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mj.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kf.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lj.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xw.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oe.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wz.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://io.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eg.colortex.cn

[N05] 最大公约数
来源：http://bx.521024.cn

Py:   math.gcd(a, b)
来源：http://el.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://er.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yg.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ul.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ev.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zx.shxzskj.cn

Ruby: a.gcd(b)
来源：http://lm.521024.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bh.szsharing.cn

[N06] 判断回文字符串
来源：http://tk.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://le.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://yo.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://sa.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://yf.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ed.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://wr.hnjuh.cn

Ruby: s == s.reverse
来源：http://gi.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ok.521024.cn

[N07] 两数之和（返回下标）
来源：http://bj.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gr.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ag.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bs.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://lt.huixiangedu.cn

Java: // 手写 HashMap
来源：http://ua.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://qj.szxytkj.cn

Ruby: // 手写 Hash
来源：http://ft.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dw.wgjwhj.cn

[N08] 生成全排列
来源：http://vl.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://ya.panjiajie.cn

PHP:  // 手写递归交换
来源：http://uu.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://nc.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://xd.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://gd.hahajie.cn

Go:   // 手写回溯递归
来源：http://xu.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://jd.521024.cn

C#:   // 手写回溯递归
来源：http://ts.bjjhwx.cn

[N09] 栈与队列
来源：http://tu.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dx.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://br.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nd.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ad.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qc.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yw.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://at.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vn.lnxyls.cn

[N10] 链表节点定义
来源：http://oa.chemitech.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://db.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://io.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pr.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dw.nszjky.cn

Java: class Node { int v; Node next; }
来源：http://io.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qt.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xe.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zg.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://fw.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gn.gzmigu.cn

PHP:  // 手写递归函数
来源：http://aq.jianghongdianzi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://id.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lm.gzmigu.cn

Java: // 手写递归
来源：http://mu.huanxung.cn

Go:   // 手写递归
来源：http://sr.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tq.newstarts.cn

C#:   // 手写递归
来源：http://fl.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gq.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tf.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gy.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xe.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yw.shxzskj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wl.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pu.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xk.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gh.nszjky.cn

================================================================================
来源：http://yw.asd995.cn

O. 并发与异步
来源：http://rr.521024.cn

================================================================================
来源：http://xv.chemitech.net.cn

[O01] 启动一个线程
来源：http://bp.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nz.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zy.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mz.jianghongdianzi.cn

TS:   // 同 JS
来源：http://ce.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://dn.shxzskj.cn

Go:   go f()
来源：http://zv.newstarts.cn

Ruby: Thread.new { f }
来源：http://id.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://cz.gzmigu.cn

[O02] 使用线程池
来源：http://od.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rw.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lb.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://sx.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://tl.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qy.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hm.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://td.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gl.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://dn.szxytkj.cn

Py:   with lock: shared += 1
来源：http://ch.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://dm.szxytkj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uy.shxzskj.cn

TS:   // 同 JS
来源：http://ss.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://ua.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ec.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jw.huixinmuqiang.cn

C#:   lock (gate) { shared++; }
来源：http://vd.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://iy.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://ad.521024.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pd.hahajie.cn

JS:   async function f() { await g(); }
来源：http://lg.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rd.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jp.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tz.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://va.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://nr.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://da.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://yl.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bk.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://zj.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://qu.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://as.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ot.521024.cn

Ruby: threads.map(&:join)
来源：http://ig.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dx.colortex.cn


<!-- 参考信息 -->