代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://hb.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://ih.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://ev.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://zk.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://be.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ef.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yd.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oz.nicolike.cn

[K06] 解析 URL 查询串
来源：http://og.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://to.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fm.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ju.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hg.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://df.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pk.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uz.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vk.haigaiapp.cn

[K07] 进制转换
来源：http://bw.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ee.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vc.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mp.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lo.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aa.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oc.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nb.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rh.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://mh.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://rb.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jb.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://bu.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://it.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kf.yuntaijiaju.cn

Go:   encoding/gob
来源：http://dj.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://mn.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ek.newstarts.cn

================================================================================
来源：http://ci.yuexingan06.cn

L. 网络请求
来源：http://go.wgjwhj.cn

================================================================================
来源：http://dd.nicolike.cn

[L01] 发送 GET 请求
来源：http://gz.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qp.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ly.wgjwhj.cn

JS:   await fetch(url)
来源：http://dx.asd995.cn

TS:   await fetch(url)
来源：http://ro.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sy.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://bf.huixiangedu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vn.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fv.hnjuh.cn

[L02] 发送 POST JSON
来源：http://vu.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://me.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bk.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gd.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oy.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wt.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qa.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qo.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hf.9csxet.cn

[L03] 设置自定义请求头
来源：http://dw.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ui.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dx.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ai.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lf.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yp.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lf.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://br.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xi.jctech888.com.cn

[L04] 设置超时
来源：http://cj.jianghongdianzi.cn

Py:   requests.get(url, timeout=5)
来源：http://kc.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lq.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rq.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://js.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dm.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://so.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ah.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://we.hahajie.cn

[L05] 上传文件（multipart）
来源：http://lg.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wy.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://es.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qy.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hk.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bw.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vc.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oy.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lq.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://br.huixiangedu.cn

Py:   resp.json()
来源：http://hy.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://em.shxzukj.cn

JS:   await resp.json()
来源：http://wc.shxzukj.cn

TS:   await resp.json()
来源：http://je.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sq.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xy.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://fr.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hb.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://qa.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fi.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dz.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://tt.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://ra.nicolike.cn

Java: resp.statusCode()
来源：http://ug.nicolike.cn

Go:   resp.StatusCode
来源：http://cp.szxytkj.cn

Ruby: resp.code.to_i
来源：http://co.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://uw.newstarts.cn

[L08] 并发请求多个地址
来源：http://qk.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vk.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://dp.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ys.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://it.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wh.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vt.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uf.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qt.panjiajie.cn

================================================================================
来源：http://qf.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://zp.huixinmuqiang.cn

================================================================================
来源：http://ch.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://yv.shxzskj.cn

Py:   sys.argv[1:]
来源：http://xz.nicolike.cn

PHP:  $argv;  $argc;
来源：http://uv.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://uh.szsharing.cn

TS:   process.argv.slice(2)
来源：http://sl.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://mt.newstarts.cn

Go:   os.Args[1:]
来源：http://wa.panjiajie.cn

Ruby: ARGV
来源：http://xp.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://pa.szxytkj.cn

[M02] 读取环境变量
来源：http://ii.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://al.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zq.haigaiapp.cn

JS:   process.env.HOME
来源：http://yq.shxzskj.cn

TS:   process.env.HOME
来源：http://ni.9csxet.cn

Java: System.getenv("HOME")
来源：http://yt.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fh.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://vw.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ak.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://rm.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rx.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ov.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kj.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://di.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cx.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dv.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ry.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://yp.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://oe.newstarts.cn

Py:   os.getcwd()
来源：http://ps.shtwfgs.cn

PHP:  getcwd();
来源：http://nw.nszjky.cn

JS:   process.cwd()
来源：http://cu.chemitech.net.cn

TS:   process.cwd()
来源：http://hr.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://vn.jctech888.com.cn

Go:   os.Getwd()
来源：http://jc.panjiajie.cn

Ruby: Dir.pwd
来源：http://vd.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zd.newstarts.cn

[M05] 设置退出码
来源：http://sy.haigaiapp.cn

Py:   sys.exit(1)
来源：http://hp.huanxung.cn

PHP:  exit(1);
来源：http://yp.shxzskj.cn

JS:   process.exit(1)
来源：http://nv.colortex.cn

TS:   process.exit(1)
来源：http://gp.hnjuh.cn

Java: System.exit(1)
来源：http://cq.szxytkj.cn

Go:   os.Exit(1)
来源：http://ep.wgjwhj.cn

Ruby: exit 1
来源：http://yn.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rj.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://eq.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://hn.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cy.szxytkj.cn

JS:   console.error("err")
来源：http://ss.szxytkj.cn

TS:   console.error("err")
来源：http://le.gzmigu.cn

Java: System.err.println("err")
来源：http://kq.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bm.muxihuayi.cn

Ruby: warn "err"
来源：http://gi.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://gs.shxzukj.cn

[M07] 判断是否为主入口
来源：http://ok.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://ha.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jh.muxihuayi.cn

JS:   require.main === module
来源：http://ll.asd995.cn

TS:   require.main === module
来源：http://ye.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://vd.jianghongdianzi.cn

Go:   func main()
来源：http://mo.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sa.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://ef.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://yl.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://ob.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://mr.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://zc.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://xc.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jl.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ig.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pb.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qb.shxzskj.cn

================================================================================
来源：http://fk.shxzskj.cn

N. 数据结构与算法
来源：http://oo.521024.cn

================================================================================
来源：http://ae.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://qb.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cw.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rg.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://li.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fu.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bl.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://xm.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vh.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kg.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://ec.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://fo.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vy.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bx.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nw.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gu.hahajie.cn

Go:   slices.Sort(arr)
来源：http://yh.chemitech.net.cn

Ruby: arr.sort
来源：http://va.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lz.colortex.cn

[N03] 快速排序（分治示例）
来源：http://pr.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ln.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://dd.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rd.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ld.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zp.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tp.huanxung.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ja.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pq.szxytkj.cn

[N04] 斐波那契数列
来源：http://fi.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bm.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iu.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lj.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://un.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jz.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sh.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zw.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cp.szsharing.cn

[N05] 最大公约数
来源：http://ev.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://kr.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mu.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dd.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sj.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lw.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xk.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://lj.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ll.muxihuayi.cn

[N06] 判断回文字符串
来源：http://pd.chemitech.net.cn

Py:   s == s[::-1]
来源：http://vm.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://fm.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://xb.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://zf.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://om.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://la.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://ui.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fi.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://gv.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gc.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rk.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qk.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://ob.nicolike.cn

Java: // 手写 HashMap
来源：http://iv.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://sq.9csxet.cn

Ruby: // 手写 Hash
来源：http://ka.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gp.lnxyls.cn

[N08] 生成全排列
来源：http://rb.521024.cn

Py:   itertools.permutations(arr)
来源：http://sy.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://kr.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://ji.shxzskj.cn

TS:   // 手写回溯递归
来源：http://ia.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://ba.asd995.cn

Go:   // 手写回溯递归
来源：http://cx.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://xj.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://ge.jctech888.com.cn

[N09] 栈与队列
来源：http://jt.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://es.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bc.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pb.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xi.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bg.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pp.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yx.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ub.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://bu.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nc.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://db.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ej.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vc.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://dw.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dx.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hx.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zz.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://cf.colortex.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tg.panjiajie.cn

PHP:  // 手写递归函数
来源：http://jm.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pa.jctech888.com.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aq.nszjky.cn

Java: // 手写递归
来源：http://gl.szxytkj.cn

Go:   // 手写递归
来源：http://dv.szsharing.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://be.huixiangedu.cn

C#:   // 手写递归
来源：http://fu.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://li.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pr.shtwfgs.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://il.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tj.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wi.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ck.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cx.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zt.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zj.9csxet.cn

================================================================================
来源：http://bm.9csxet.cn

O. 并发与异步
来源：http://qa.panjiajie.cn

================================================================================
来源：http://lm.szxytkj.cn

[O01] 启动一个线程
来源：http://yt.szsharing.cn


<!-- 参考信息 -->