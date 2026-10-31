代发 wailian999

Go:   encoding/gob
来源：http://dr.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://op.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mz.wgjwhj.cn

================================================================================
来源：http://zg.hahajie.cn

L. 网络请求
来源：http://ry.panjiajie.cn

================================================================================
来源：http://mw.szsharing.cn

[L01] 发送 GET 请求
来源：http://xp.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://la.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yg.colortex.cn

JS:   await fetch(url)
来源：http://sp.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://bk.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hi.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://ym.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dp.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ce.szxytkj.cn

[L02] 发送 POST JSON
来源：http://oz.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dm.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://um.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bq.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iq.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kq.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mu.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wd.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zh.gzmigu.cn

[L03] 设置自定义请求头
来源：http://sf.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mb.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://va.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hr.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hf.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ms.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nx.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://as.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mq.9csxet.cn

[L04] 设置超时
来源：http://ys.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://gf.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://di.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kr.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aj.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://da.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cp.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pj.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qy.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://cn.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mx.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jh.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uc.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oa.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://df.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://us.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mb.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gl.9csxet.cn

[L06] 解析响应为 JSON
来源：http://ni.szxytkj.cn

Py:   resp.json()
来源：http://gr.huanxung.cn

PHP:  json_decode($body, true);
来源：http://pg.hahajie.cn

JS:   await resp.json()
来源：http://lg.bjjhwx.cn

TS:   await resp.json()
来源：http://sc.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ud.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ph.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://wy.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rx.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://fl.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sb.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://th.asd995.cn

JS:   resp.ok;  resp.status
来源：http://ds.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://ek.shtwfgs.cn

Java: resp.statusCode()
来源：http://ow.lnxyls.cn

Go:   resp.StatusCode
来源：http://ja.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://cq.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://ro.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://ls.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ad.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://hb.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fk.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yp.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zy.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vm.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pc.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://em.huanxung.cn

================================================================================
来源：http://wx.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://gj.nicolike.cn

================================================================================
来源：http://en.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://yt.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://di.nszjky.cn

PHP:  $argv;  $argc;
来源：http://co.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://cn.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://np.asd995.cn

Java: args 数组（main 方法参数）
来源：http://sg.shtwfgs.cn

Go:   os.Args[1:]
来源：http://tp.panjiajie.cn

Ruby: ARGV
来源：http://ku.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://sj.panjiajie.cn

[M02] 读取环境变量
来源：http://tq.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://id.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mj.shtwfgs.cn

JS:   process.env.HOME
来源：http://uh.hahajie.cn

TS:   process.env.HOME
来源：http://py.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://te.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fn.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://sz.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rc.huixiangedu.cn

[M03] 执行外部命令
来源：http://hv.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ae.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lf.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gi.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xr.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://go.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cz.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ae.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://xr.shxzukj.cn

[M04] 获取当前工作目录
来源：http://xv.521024.cn

Py:   os.getcwd()
来源：http://fz.nicolike.cn

PHP:  getcwd();
来源：http://sk.newstarts.cn

JS:   process.cwd()
来源：http://se.szsharing.cn

TS:   process.cwd()
来源：http://rt.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://qq.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://nj.szxytkj.cn

Ruby: Dir.pwd
来源：http://sz.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mx.gzmigu.cn

[M05] 设置退出码
来源：http://co.huixiangedu.cn

Py:   sys.exit(1)
来源：http://uu.huanxung.cn

PHP:  exit(1);
来源：http://dx.shxzskj.cn

JS:   process.exit(1)
来源：http://rs.huanxung.cn

TS:   process.exit(1)
来源：http://bd.jianghongdianzi.cn

Java: System.exit(1)
来源：http://mg.yuexingan06.cn

Go:   os.Exit(1)
来源：http://cs.hnjuh.cn

Ruby: exit 1
来源：http://ol.wgjwhj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xb.9csxet.cn

[M06] 向标准错误输出
来源：http://qn.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://yk.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bp.haigaiapp.cn

JS:   console.error("err")
来源：http://qh.muxihuayi.cn

TS:   console.error("err")
来源：http://zh.nicolike.cn

Java: System.err.println("err")
来源：http://pv.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://en.chemitech.net.cn

Ruby: warn "err"
来源：http://ov.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://tq.asd995.cn

[M07] 判断是否为主入口
来源：http://rj.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://fq.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dv.shxzskj.cn

JS:   require.main === module
来源：http://wf.panjiajie.cn

TS:   require.main === module
来源：http://ct.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://lg.gzmigu.cn

Go:   func main()
来源：http://pa.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://va.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://sl.colortex.cn

[M08] 获取系统与运行时信息
来源：http://cg.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://ps.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://uy.szsharing.cn

JS:   process.platform;  process.version
来源：http://kr.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://ig.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yt.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oy.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mq.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://um.szxytkj.cn

================================================================================
来源：http://zd.shxzukj.cn

N. 数据结构与算法
来源：http://sl.521024.cn

================================================================================
来源：http://ge.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://fe.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fm.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mn.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xc.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pk.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ch.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ma.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gx.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://il.nszjky.cn

[N02] 排序（工程实践用内置实现）
来源：http://gz.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://pg.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ur.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pp.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rj.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gg.huanxung.cn

Go:   slices.Sort(arr)
来源：http://it.bookmarksfly.cn

Ruby: arr.sort
来源：http://sd.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://js.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://tl.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://st.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://op.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mm.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sx.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jc.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://om.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fy.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pi.nicolike.cn

[N04] 斐波那契数列
来源：http://ih.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://st.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ia.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dp.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tc.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vo.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eq.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zx.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hu.nszjky.cn

[N05] 最大公约数
来源：http://ml.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://aw.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sv.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eo.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zc.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cr.newstarts.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kd.huanxung.cn

Ruby: a.gcd(b)
来源：http://pv.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dc.nicolike.cn

[N06] 判断回文字符串
来源：http://ga.colortex.cn

Py:   s == s[::-1]
来源：http://jq.hahajie.cn

PHP:  $s === strrev($s);
来源：http://ap.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://qg.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://zu.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qh.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://gj.gzmigu.cn

Ruby: s == s.reverse
来源：http://uz.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jr.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://gp.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bi.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bz.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tu.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://sa.nszjky.cn

Java: // 手写 HashMap
来源：http://be.521024.cn

Go:   // 手写 map[int]int
来源：http://ho.panjiajie.cn

Ruby: // 手写 Hash
来源：http://ug.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cr.huanxung.cn

[N08] 生成全排列
来源：http://bu.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://gw.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://jc.asd995.cn

JS:   // 手写回溯递归
来源：http://vo.panjiajie.cn

TS:   // 手写回溯递归
来源：http://ih.szxytkj.cn

Java: // 手写回溯递归
来源：http://fa.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://gz.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://fv.panjiajie.cn

C#:   // 手写回溯递归
来源：http://mu.panjiajie.cn

[N09] 栈与队列
来源：http://gj.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lb.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fe.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rd.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ag.colortex.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uq.jctech888.com.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ba.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wj.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ba.nicolike.cn

[N10] 链表节点定义
来源：http://ik.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vs.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bo.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cw.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cx.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://ac.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://li.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cl.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fu.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://cf.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cg.szxytkj.cn

PHP:  // 手写递归函数
来源：http://kw.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wh.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lq.shxzskj.cn

Java: // 手写递归
来源：http://dy.szxytkj.cn

Go:   // 手写递归
来源：http://px.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nb.huixiangedu.cn

C#:   // 手写递归
来源：http://nl.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dp.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ja.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ur.huanxung.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gb.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ac.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lq.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vo.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vt.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vv.bookmarksfly.cn

================================================================================
来源：http://vg.shtwfgs.cn

O. 并发与异步
来源：http://wz.colortex.cn

================================================================================
来源：http://ow.newstarts.cn

[O01] 启动一个线程
来源：http://rj.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sf.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ot.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zg.bookmarksfly.cn

TS:   // 同 JS
来源：http://nq.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://dn.jctech888.com.cn

Go:   go f()
来源：http://kl.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://oe.huanxung.cn

C#:   Task.Run(() => F());
来源：http://cl.yuexingan06.cn

[O02] 使用线程池
来源：http://ua.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gl.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://px.nicolike.cn

JS:   // worker_threads 线程池
来源：http://ib.521024.cn

TS:   // worker_threads 线程池
来源：http://wk.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ms.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qj.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vb.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ua.bookmarksfly.cn

[O03] 加锁保护共享数据
来源：http://qr.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://fw.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://cx.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://so.huixinmuqiang.cn

TS:   // 同 JS
来源：http://re.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://uc.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mb.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nd.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://jn.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://sk.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://gn.521024.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sa.huanxung.cn

JS:   async function f() { await g(); }
来源：http://ex.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://se.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://km.asd995.cn


<!-- 参考信息 -->