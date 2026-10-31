代发 wailian999

Go:   encoding/gob
来源：http://bo.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://br.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xl.panjiajie.cn

================================================================================
来源：http://zv.jctech888.com.cn

L. 网络请求
来源：http://cw.colortex.cn

================================================================================
来源：http://wm.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://kc.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vv.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wz.newstarts.cn

JS:   await fetch(url)
来源：http://fk.yuexingan06.cn

TS:   await fetch(url)
来源：http://fj.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wq.521024.cn

Go:   resp, err := http.Get(url)
来源：http://al.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gl.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nn.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://at.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uh.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rl.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pv.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xn.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gg.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lu.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aq.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nq.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://om.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qn.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gx.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hs.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zu.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://om.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://az.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mt.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yy.yuntaijiaju.cn

[L04] 设置超时
来源：http://bf.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://we.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hk.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tt.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://id.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kg.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sr.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pd.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mr.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://ts.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yg.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ng.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://om.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cd.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rv.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qq.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ee.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fv.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://oh.jctech888.com.cn

Py:   resp.json()
来源：http://ti.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://ft.haigaiapp.cn

JS:   await resp.json()
来源：http://yw.szxytkj.cn

TS:   await resp.json()
来源：http://wj.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fo.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://py.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://an.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sx.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://wj.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sb.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oa.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://he.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://pt.yuexingan06.cn

Java: resp.statusCode()
来源：http://hs.bjjhwx.cn

Go:   resp.StatusCode
来源：http://cl.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://so.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://jt.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://yc.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gu.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://rx.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ft.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zm.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aw.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hl.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://am.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dw.9csxet.cn

================================================================================
来源：http://me.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://pf.wgjwhj.cn

================================================================================
来源：http://hl.haigaiapp.cn

[M01] 读取命令行参数
来源：http://pl.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://ld.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://ot.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://qw.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://yd.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://gy.chemitech.net.cn

Go:   os.Args[1:]
来源：http://wo.newstarts.cn

Ruby: ARGV
来源：http://mc.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://vk.jctech888.com.cn

[M02] 读取环境变量
来源：http://af.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://rh.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ek.nszjky.cn

JS:   process.env.HOME
来源：http://mq.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://fi.asd995.cn

Java: System.getenv("HOME")
来源：http://ow.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xp.colortex.cn

Ruby: ENV["HOME"]
来源：http://do.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wa.bjjhwx.cn

[M03] 执行外部命令
来源：http://hw.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pq.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ns.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://it.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ze.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zg.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dt.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://or.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://jd.huanxung.cn

[M04] 获取当前工作目录
来源：http://gw.shxzskj.cn

Py:   os.getcwd()
来源：http://ms.huixinmuqiang.cn

PHP:  getcwd();
来源：http://pt.521024.cn

JS:   process.cwd()
来源：http://tg.asd995.cn

TS:   process.cwd()
来源：http://nj.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://vm.panjiajie.cn

Go:   os.Getwd()
来源：http://wl.szxytkj.cn

Ruby: Dir.pwd
来源：http://vw.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lr.yuexingan06.cn

[M05] 设置退出码
来源：http://oq.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://wt.nszjky.cn

PHP:  exit(1);
来源：http://de.jctech888.com.cn

JS:   process.exit(1)
来源：http://di.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://gd.huixiangedu.cn

Java: System.exit(1)
来源：http://qu.hahajie.cn

Go:   os.Exit(1)
来源：http://bo.lnxyls.cn

Ruby: exit 1
来源：http://ya.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lm.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://zj.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://pa.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gg.bookmarksfly.cn

JS:   console.error("err")
来源：http://is.haigaiapp.cn

TS:   console.error("err")
来源：http://vi.nszjky.cn

Java: System.err.println("err")
来源：http://uu.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ua.lnxyls.cn

Ruby: warn "err"
来源：http://uf.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://lp.hnjuh.cn

[M07] 判断是否为主入口
来源：http://xd.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://se.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qc.bookmarksfly.cn

JS:   require.main === module
来源：http://fw.hahajie.cn

TS:   require.main === module
来源：http://ym.huanxung.cn

Java: public static void main(String[] args)
来源：http://ej.bookmarksfly.cn

Go:   func main()
来源：http://fl.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ry.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://vf.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://lz.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://nn.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://mk.shxzukj.cn

JS:   process.platform;  process.version
来源：http://ml.huanxung.cn

TS:   process.platform;  process.version
来源：http://nh.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bx.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fn.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qp.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qr.bjjhwx.cn

================================================================================
来源：http://kd.nszjky.cn

N. 数据结构与算法
来源：http://tl.hnjuh.cn

================================================================================
来源：http://zf.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://hg.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qs.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ue.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vl.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mh.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ob.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://gw.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ca.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://so.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://qk.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://bg.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pt.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hi.huixinmuqiang.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fq.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fk.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://wn.jctech888.com.cn

Ruby: arr.sort
来源：http://ov.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lx.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://ty.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zq.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://qf.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qz.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eh.newstarts.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bn.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gg.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://af.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tc.asd995.cn

[N04] 斐波那契数列
来源：http://wx.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ql.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pr.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gv.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qt.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ld.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rc.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wc.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pw.shxzukj.cn

[N05] 最大公约数
来源：http://bs.newstarts.cn

Py:   math.gcd(a, b)
来源：http://zs.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ln.nicolike.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hu.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pw.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lc.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ke.lnxyls.cn

Ruby: a.gcd(b)
来源：http://ro.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://am.huixiangedu.cn

[N06] 判断回文字符串
来源：http://sb.shxzskj.cn

Py:   s == s[::-1]
来源：http://zn.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://ca.panjiajie.cn

JS:   s === [...s].reverse().join("")
来源：http://ut.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://cm.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://on.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://ur.huanxung.cn

Ruby: s == s.reverse
来源：http://ai.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ky.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://da.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ks.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hq.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xd.huixinmuqiang.cn

TS:   // 手写 Map<string, number>
来源：http://qd.yuexingan06.cn

Java: // 手写 HashMap
来源：http://sy.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://ed.hnjuh.cn

Ruby: // 手写 Hash
来源：http://zw.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rs.szsharing.cn

[N08] 生成全排列
来源：http://hx.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://ys.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://bf.asd995.cn

JS:   // 手写回溯递归
来源：http://sj.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://cc.bjjhwx.cn

Java: // 手写回溯递归
来源：http://nk.panjiajie.cn

Go:   // 手写回溯递归
来源：http://qw.colortex.cn

Ruby: arr.permutation.to_a
来源：http://wr.521024.cn

C#:   // 手写回溯递归
来源：http://vu.shxzukj.cn

[N09] 栈与队列
来源：http://nx.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ai.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lr.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gb.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zl.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ov.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ep.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kz.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sp.521024.cn

[N10] 链表节点定义
来源：http://ef.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hm.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ih.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rt.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hj.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://eo.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rk.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hr.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jq.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://kk.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://an.hahajie.cn

PHP:  // 手写递归函数
来源：http://mx.shxzskj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nd.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qc.lnxyls.cn

Java: // 手写递归
来源：http://ky.muxihuayi.cn

Go:   // 手写递归
来源：http://de.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wb.haigaiapp.cn

C#:   // 手写递归
来源：http://th.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cn.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lc.nicolike.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://eg.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xr.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oe.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fm.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qd.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ls.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ky.shxzskj.cn

================================================================================
来源：http://gy.shtwfgs.cn

O. 并发与异步
来源：http://ao.colortex.cn

================================================================================
来源：http://fc.shxzskj.cn

[O01] 启动一个线程
来源：http://db.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pm.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wd.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ny.huixiangedu.cn

TS:   // 同 JS
来源：http://jn.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://sx.chemitech.net.cn

Go:   go f()
来源：http://im.panjiajie.cn

Ruby: Thread.new { f }
来源：http://py.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://pd.521024.cn

[O02] 使用线程池
来源：http://oj.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ro.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kq.colortex.cn

JS:   // worker_threads 线程池
来源：http://cb.szxytkj.cn

TS:   // worker_threads 线程池
来源：http://po.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kk.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://br.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ym.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wn.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://uc.lnxyls.cn

Py:   with lock: shared += 1
来源：http://oq.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://mu.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://he.hnjuh.cn

TS:   // 同 JS
来源：http://ar.huanxung.cn

Java: synchronized (this) { shared++; }
来源：http://ij.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bw.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vq.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://os.colortex.cn

[O04] 定义异步函数并等待
来源：http://zc.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://yz.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wf.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://ko.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zk.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sl.gzmigu.cn


<!-- 参考信息 -->