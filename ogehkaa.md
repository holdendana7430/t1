代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://ia.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://nk.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://qf.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://st.jianghongdianzi.cn

Go:   encoding/gob
来源：http://xt.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://gc.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ll.521024.cn

================================================================================
来源：http://tj.szxytkj.cn

L. 网络请求
来源：http://ov.bjjhwx.cn

================================================================================
来源：http://hc.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://fr.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://en.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qj.521024.cn

JS:   await fetch(url)
来源：http://lj.panjiajie.cn

TS:   await fetch(url)
来源：http://ts.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://az.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://mv.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vr.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kz.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://id.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zb.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jv.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nu.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kg.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ar.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eb.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jl.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ud.colortex.cn

[L03] 设置自定义请求头
来源：http://un.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uz.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://op.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wu.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nk.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wl.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dd.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ln.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ap.szxytkj.cn

[L04] 设置超时
来源：http://nv.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://lm.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zd.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ok.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kk.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pq.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wh.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://md.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zu.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://tv.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bq.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jj.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://di.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xw.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oj.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ur.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://js.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uf.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://xd.shxzukj.cn

Py:   resp.json()
来源：http://pa.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://pb.bjjhwx.cn

JS:   await resp.json()
来源：http://fn.gzmigu.cn

TS:   await resp.json()
来源：http://yr.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ea.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tx.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://xe.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bz.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://mm.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vs.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yj.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://gy.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://pm.panjiajie.cn

Java: resp.statusCode()
来源：http://uz.bjjhwx.cn

Go:   resp.StatusCode
来源：http://qs.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://vl.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://uo.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://xp.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rs.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://sd.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wu.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ew.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fc.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ve.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pv.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gt.hnjuh.cn

================================================================================
来源：http://rp.521024.cn

M. 命令行 / 进程 / 环境
来源：http://ld.hahajie.cn

================================================================================
来源：http://bo.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://ep.colortex.cn

Py:   sys.argv[1:]
来源：http://lm.hahajie.cn

PHP:  $argv;  $argc;
来源：http://xy.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://tt.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://ua.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://cj.colortex.cn

Go:   os.Args[1:]
来源：http://gq.huixinmuqiang.cn

Ruby: ARGV
来源：http://so.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://cg.szxytkj.cn

[M02] 读取环境变量
来源：http://as.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://vt.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hp.nicolike.cn

JS:   process.env.HOME
来源：http://hv.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://ue.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://ib.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dg.asd995.cn

Ruby: ENV["HOME"]
来源：http://gy.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xs.jctech888.com.cn

[M03] 执行外部命令
来源：http://ym.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dg.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uf.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jb.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ib.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://go.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lx.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vs.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://wo.asd995.cn

[M04] 获取当前工作目录
来源：http://ch.hnjuh.cn

Py:   os.getcwd()
来源：http://uw.hahajie.cn

PHP:  getcwd();
来源：http://gf.shtwfgs.cn

JS:   process.cwd()
来源：http://ro.huixinmuqiang.cn

TS:   process.cwd()
来源：http://vk.chemitech.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://py.chemitech.net.cn

Go:   os.Getwd()
来源：http://ui.nicolike.cn

Ruby: Dir.pwd
来源：http://bl.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://st.wgjwhj.cn

[M05] 设置退出码
来源：http://id.bjjhwx.cn

Py:   sys.exit(1)
来源：http://qm.bjjhwx.cn

PHP:  exit(1);
来源：http://ca.wgjwhj.cn

JS:   process.exit(1)
来源：http://sy.asd995.cn

TS:   process.exit(1)
来源：http://wh.chemitech.net.cn

Java: System.exit(1)
来源：http://ij.hahajie.cn

Go:   os.Exit(1)
来源：http://uy.newstarts.cn

Ruby: exit 1
来源：http://ok.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cf.9csxet.cn

[M06] 向标准错误输出
来源：http://oq.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://xk.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wi.bjjhwx.cn

JS:   console.error("err")
来源：http://tg.521024.cn

TS:   console.error("err")
来源：http://mx.muxihuayi.cn

Java: System.err.println("err")
来源：http://mb.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oo.521024.cn

Ruby: warn "err"
来源：http://yo.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://it.huanxung.cn

[M07] 判断是否为主入口
来源：http://sz.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://cr.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gb.yuexingan06.cn

JS:   require.main === module
来源：http://gt.nszjky.cn

TS:   require.main === module
来源：http://iq.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://ed.jctech888.com.cn

Go:   func main()
来源：http://mq.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ev.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://if.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://ff.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://eq.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://ma.gzmigu.cn

JS:   process.platform;  process.version
来源：http://ex.gzmigu.cn

TS:   process.platform;  process.version
来源：http://qt.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xv.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fe.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ty.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sy.bjjhwx.cn

================================================================================
来源：http://yw.hahajie.cn

N. 数据结构与算法
来源：http://gr.newstarts.cn

================================================================================
来源：http://kh.521024.cn

[N01] 二分查找（有序数组）
来源：http://qm.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pj.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://po.gzmigu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fr.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ep.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zr.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://ei.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wr.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pc.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://jb.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://xm.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xk.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://on.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ih.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vo.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://vh.wgjwhj.cn

Ruby: arr.sort
来源：http://fl.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://or.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://ut.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mg.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://wk.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nj.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ou.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jl.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mr.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qq.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dh.huixiangedu.cn

[N04] 斐波那契数列
来源：http://rk.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xb.chemitech.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://an.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xy.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rg.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://br.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jj.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kn.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zc.szxytkj.cn

[N05] 最大公约数
来源：http://ni.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://xl.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sn.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gi.asd995.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oy.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://il.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ay.gzmigu.cn

Ruby: a.gcd(b)
来源：http://qe.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://as.lnxyls.cn

[N06] 判断回文字符串
来源：http://an.szsharing.cn

Py:   s == s[::-1]
来源：http://ro.9csxet.cn

PHP:  $s === strrev($s);
来源：http://sg.jctech888.com.cn

JS:   s === [...s].reverse().join("")
来源：http://bl.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://mn.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gp.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://vm.gzmigu.cn

Ruby: s == s.reverse
来源：http://zg.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zt.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://lw.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xz.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xa.nicolike.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hp.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://wl.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://xm.colortex.cn

Go:   // 手写 map[int]int
来源：http://tm.gzmigu.cn

Ruby: // 手写 Hash
来源：http://kg.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://li.gzmigu.cn

[N08] 生成全排列
来源：http://mn.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://nu.newstarts.cn

PHP:  // 手写递归交换
来源：http://mv.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://xf.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://le.jctech888.com.cn

Java: // 手写回溯递归
来源：http://bt.nicolike.cn

Go:   // 手写回溯递归
来源：http://bi.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://fr.szxytkj.cn

C#:   // 手写回溯递归
来源：http://zt.bjjhwx.cn

[N09] 栈与队列
来源：http://ay.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gi.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://az.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nh.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vp.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mc.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://du.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qa.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cn.shxzukj.cn

[N10] 链表节点定义
来源：http://av.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ap.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://iu.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kt.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vd.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://mf.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qb.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://if.huanxung.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bz.nszjky.cn

[N11] 二叉树中序遍历
来源：http://za.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://py.panjiajie.cn

PHP:  // 手写递归函数
来源：http://dm.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rt.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fe.gzmigu.cn

Java: // 手写递归
来源：http://ib.szsharing.cn

Go:   // 手写递归
来源：http://pw.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qi.gzmigu.cn

C#:   // 手写递归
来源：http://dd.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vt.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ms.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kj.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cr.nszjky.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cy.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nb.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rr.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cr.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ss.wgjwhj.cn

================================================================================
来源：http://xu.szxytkj.cn

O. 并发与异步
来源：http://qn.huixiangedu.cn

================================================================================
来源：http://qx.bookmarksfly.cn

[O01] 启动一个线程
来源：http://zz.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bb.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ct.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gt.wgjwhj.cn

TS:   // 同 JS
来源：http://sy.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://pu.huixinmuqiang.cn

Go:   go f()
来源：http://nw.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://zv.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://st.wgjwhj.cn

[O02] 使用线程池
来源：http://ha.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xj.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cg.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://xs.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://pk.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qs.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nr.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nv.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iu.bookmarksfly.cn

[O03] 加锁保护共享数据
来源：http://ix.9csxet.cn

Py:   with lock: shared += 1
来源：http://qw.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://my.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bh.bookmarksfly.cn

TS:   // 同 JS
来源：http://ft.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://ds.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sd.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tv.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://kl.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://ym.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://zg.newstarts.cn


<!-- 参考信息 -->