代发 wailian999

L. 网络请求
来源：http://sx.bookmarksfly.cn

================================================================================
来源：http://wc.huanxung.cn

[L01] 发送 GET 请求
来源：http://oq.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rq.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eu.nicolike.cn

JS:   await fetch(url)
来源：http://dh.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://pm.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ed.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://ta.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fg.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sm.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://yc.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sk.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vg.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zs.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kd.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://av.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lw.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://be.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dq.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://wo.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://af.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uf.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ev.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rd.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ov.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mp.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dn.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qk.wgjwhj.cn

[L04] 设置超时
来源：http://ul.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://ca.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uv.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yy.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mw.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vj.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ye.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bw.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wp.asd995.cn

[L05] 上传文件（multipart）
来源：http://ti.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gn.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://en.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ly.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tq.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kf.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nb.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bd.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yv.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://af.asd995.cn

Py:   resp.json()
来源：http://gl.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://ej.yuexingan06.cn

JS:   await resp.json()
来源：http://on.521024.cn

TS:   await resp.json()
来源：http://cs.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tl.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ry.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://xs.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fz.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://oc.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ci.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yc.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://js.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://nx.jctech888.com.cn

Java: resp.statusCode()
来源：http://hj.lnxyls.cn

Go:   resp.StatusCode
来源：http://qy.huanxung.cn

Ruby: resp.code.to_i
来源：http://we.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://rn.asd995.cn

[L08] 并发请求多个地址
来源：http://jr.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jt.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://ii.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sw.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ho.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kh.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jd.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ef.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ae.jctech888.com.cn

================================================================================
来源：http://si.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://xv.nicolike.cn

================================================================================
来源：http://hh.muxihuayi.cn

[M01] 读取命令行参数
来源：http://hl.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://oc.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://yy.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://xw.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://gm.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://pz.shxzskj.cn

Go:   os.Args[1:]
来源：http://xf.szxytkj.cn

Ruby: ARGV
来源：http://wg.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://ry.haigaiapp.cn

[M02] 读取环境变量
来源：http://zy.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://wj.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cn.nszjky.cn

JS:   process.env.HOME
来源：http://qt.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://hw.asd995.cn

Java: System.getenv("HOME")
来源：http://th.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bz.asd995.cn

Ruby: ENV["HOME"]
来源：http://fj.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hl.haigaiapp.cn

[M03] 执行外部命令
来源：http://eo.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dg.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kr.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kt.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vp.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xa.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ke.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hk.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://zy.nszjky.cn

[M04] 获取当前工作目录
来源：http://mm.haigaiapp.cn

Py:   os.getcwd()
来源：http://wd.chemitech.net.cn

PHP:  getcwd();
来源：http://be.lnxyls.cn

JS:   process.cwd()
来源：http://kb.huixiangedu.cn

TS:   process.cwd()
来源：http://at.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://fw.szsharing.cn

Go:   os.Getwd()
来源：http://xs.shtwfgs.cn

Ruby: Dir.pwd
来源：http://im.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ak.huixinmuqiang.cn

[M05] 设置退出码
来源：http://ml.muxihuayi.cn

Py:   sys.exit(1)
来源：http://ix.hahajie.cn

PHP:  exit(1);
来源：http://wp.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://kx.gzmigu.cn

TS:   process.exit(1)
来源：http://tu.panjiajie.cn

Java: System.exit(1)
来源：http://ef.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://tm.9csxet.cn

Ruby: exit 1
来源：http://vd.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pg.asd995.cn

[M06] 向标准错误输出
来源：http://av.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://sj.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wh.nicolike.cn

JS:   console.error("err")
来源：http://qz.yuntaijiaju.cn

TS:   console.error("err")
来源：http://zr.bjjhwx.cn

Java: System.err.println("err")
来源：http://tf.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ki.colortex.cn

Ruby: warn "err"
来源：http://jb.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://vi.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://fi.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://ih.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fc.szxytkj.cn

JS:   require.main === module
来源：http://td.szxytkj.cn

TS:   require.main === module
来源：http://ja.hahajie.cn

Java: public static void main(String[] args)
来源：http://rw.9csxet.cn

Go:   func main()
来源：http://cv.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://il.huanxung.cn

C#:   static void Main(string[] args)
来源：http://tq.colortex.cn

[M08] 获取系统与运行时信息
来源：http://zb.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://pt.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://ap.lnxyls.cn

JS:   process.platform;  process.version
来源：http://oi.asd995.cn

TS:   process.platform;  process.version
来源：http://at.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wg.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pf.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yi.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fk.nszjky.cn

================================================================================
来源：http://wi.jianghongdianzi.cn

N. 数据结构与算法
来源：http://cn.haigaiapp.cn

================================================================================
来源：http://md.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://rq.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sq.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xp.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ql.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nd.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jr.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://br.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yv.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cd.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://bz.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://kw.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wx.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://up.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lc.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gh.9csxet.cn

Go:   slices.Sort(arr)
来源：http://eg.panjiajie.cn

Ruby: arr.sort
来源：http://tp.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kh.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://pr.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rz.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://sl.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yl.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oa.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hw.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ji.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ia.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vy.shxzukj.cn

[N04] 斐波那契数列
来源：http://kf.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qy.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kx.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yh.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ym.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xt.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vf.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://up.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lb.lnxyls.cn

[N05] 最大公约数
来源：http://ro.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://fc.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cp.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nh.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aj.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://es.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ko.panjiajie.cn

Ruby: a.gcd(b)
来源：http://pm.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fh.shxzskj.cn

[N06] 判断回文字符串
来源：http://iu.chemitech.net.cn

Py:   s == s[::-1]
来源：http://kq.yuntaijiaju.cn

PHP:  $s === strrev($s);
来源：http://gn.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://tf.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://kx.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pj.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://ve.hahajie.cn

Ruby: s == s.reverse
来源：http://qn.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ti.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://cx.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ic.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ha.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ov.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://gf.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://fj.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://bw.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://br.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gs.lnxyls.cn

[N08] 生成全排列
来源：http://uw.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://nu.colortex.cn

PHP:  // 手写递归交换
来源：http://xi.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://ph.521024.cn

TS:   // 手写回溯递归
来源：http://ox.panjiajie.cn

Java: // 手写回溯递归
来源：http://ce.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://bc.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://qq.szxytkj.cn

C#:   // 手写回溯递归
来源：http://vw.chemitech.net.cn

[N09] 栈与队列
来源：http://wl.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vu.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xx.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ed.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dl.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mh.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://we.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zf.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://od.huanxung.cn

[N10] 链表节点定义
来源：http://ch.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tw.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hv.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jc.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mb.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://zn.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ht.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://el.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yp.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://bb.jctech888.com.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qx.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://oe.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mm.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bd.bookmarksfly.cn

Java: // 手写递归
来源：http://hj.chemitech.net.cn

Go:   // 手写递归
来源：http://mg.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://co.jianghongdianzi.cn

C#:   // 手写递归
来源：http://uj.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nu.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sy.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gt.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lj.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://if.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://la.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iz.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ju.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://te.yuntaijiaju.cn

================================================================================
来源：http://yo.gzmigu.cn

O. 并发与异步
来源：http://ye.nicolike.cn

================================================================================
来源：http://jg.szsharing.cn

[O01] 启动一个线程
来源：http://re.lnxyls.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bt.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pa.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cx.huixinmuqiang.cn

TS:   // 同 JS
来源：http://ti.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://zq.chemitech.net.cn

Go:   go f()
来源：http://aw.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://yq.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://yu.gzmigu.cn

[O02] 使用线程池
来源：http://zq.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jn.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rh.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://lj.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://ob.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://va.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bm.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sh.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tf.nicolike.cn

[O03] 加锁保护共享数据
来源：http://cr.szsharing.cn

Py:   with lock: shared += 1
来源：http://hz.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://ad.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gl.colortex.cn

TS:   // 同 JS
来源：http://cm.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://es.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kj.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sg.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://eb.asd995.cn

[O04] 定义异步函数并等待
来源：http://re.521024.cn

Py:   async def f():⏎    await g()
来源：http://po.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vl.colortex.cn

JS:   async function f() { await g(); }
来源：http://qd.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ub.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sh.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zg.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ew.521024.cn

C#:   async Task F() { await G(); }
来源：http://xh.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://yx.shxzskj.cn


<!-- 参考信息 -->