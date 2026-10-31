代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ro.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tv.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ir.wgjwhj.cn

[K05] 深拷贝对象
来源：http://ov.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://ff.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://hi.colortex.cn

JS:   structuredClone(obj)
来源：http://jl.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://yq.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://df.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ls.9csxet.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bt.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://aw.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://bx.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bc.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dj.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zn.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zx.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gf.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://iv.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lf.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zi.jianghongdianzi.cn

[K07] 进制转换
来源：http://yj.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bd.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lh.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uv.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xj.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nv.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zg.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wx.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ff.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ny.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://ow.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tt.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://ya.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://xj.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://co.9csxet.cn

Go:   encoding/gob
来源：http://dd.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://rv.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://an.yuntaijiaju.cn

================================================================================
来源：http://jv.panjiajie.cn

L. 网络请求
来源：http://hr.huixiangedu.cn

================================================================================
来源：http://rx.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://ye.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zs.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bd.huanxung.cn

JS:   await fetch(url)
来源：http://dq.newstarts.cn

TS:   await fetch(url)
来源：http://rt.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ry.521024.cn

Go:   resp, err := http.Get(url)
来源：http://dt.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://af.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tw.nicolike.cn

[L02] 发送 POST JSON
来源：http://sn.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ci.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sg.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zd.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cj.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ap.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jv.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dq.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hm.nicolike.cn

[L03] 设置自定义请求头
来源：http://tc.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vy.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://re.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xm.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ud.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uv.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://po.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ou.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mw.huixiangedu.cn

[L04] 设置超时
来源：http://eq.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://jb.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zm.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ls.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ik.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cm.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tq.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vy.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sy.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://fx.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ju.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kz.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wm.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sm.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tp.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eg.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lo.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lc.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://dd.asd995.cn

Py:   resp.json()
来源：http://pz.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://qz.shxzukj.cn

JS:   await resp.json()
来源：http://km.bjjhwx.cn

TS:   await resp.json()
来源：http://iv.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gv.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://id.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://jm.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vv.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://lw.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zj.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sl.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://en.521024.cn

TS:   resp.ok;  resp.status
来源：http://gt.huixiangedu.cn

Java: resp.statusCode()
来源：http://kl.hahajie.cn

Go:   resp.StatusCode
来源：http://ku.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://qo.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://ea.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://op.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cl.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://ya.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yr.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wk.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zx.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tt.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yn.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cf.jctech888.com.cn

================================================================================
来源：http://kw.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://bu.9csxet.cn

================================================================================
来源：http://sc.muxihuayi.cn

[M01] 读取命令行参数
来源：http://hq.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://ei.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://tg.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://ju.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://ww.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://rx.9csxet.cn

Go:   os.Args[1:]
来源：http://dp.jianghongdianzi.cn

Ruby: ARGV
来源：http://dq.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://ru.chemitech.net.cn

[M02] 读取环境变量
来源：http://rp.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://aq.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qw.nicolike.cn

JS:   process.env.HOME
来源：http://hr.shxzukj.cn

TS:   process.env.HOME
来源：http://wg.hahajie.cn

Java: System.getenv("HOME")
来源：http://dz.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uu.szsharing.cn

Ruby: ENV["HOME"]
来源：http://qi.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yp.yuexingan06.cn

[M03] 执行外部命令
来源：http://fg.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zz.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kz.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kg.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sb.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vp.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fu.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zu.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://ts.panjiajie.cn

[M04] 获取当前工作目录
来源：http://gr.szsharing.cn

Py:   os.getcwd()
来源：http://vs.haigaiapp.cn

PHP:  getcwd();
来源：http://gy.gzmigu.cn

JS:   process.cwd()
来源：http://kl.yuntaijiaju.cn

TS:   process.cwd()
来源：http://dl.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://qf.9csxet.cn

Go:   os.Getwd()
来源：http://pw.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://hl.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pg.panjiajie.cn

[M05] 设置退出码
来源：http://tx.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://lp.lnxyls.cn

PHP:  exit(1);
来源：http://ei.lnxyls.cn

JS:   process.exit(1)
来源：http://wn.shxzskj.cn

TS:   process.exit(1)
来源：http://ju.jianghongdianzi.cn

Java: System.exit(1)
来源：http://ft.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://yz.bookmarksfly.cn

Ruby: exit 1
来源：http://kd.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ol.wgjwhj.cn

[M06] 向标准错误输出
来源：http://kx.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://qf.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ot.yuexingan06.cn

JS:   console.error("err")
来源：http://jg.shxzskj.cn

TS:   console.error("err")
来源：http://gp.hahajie.cn

Java: System.err.println("err")
来源：http://hd.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ae.jctech888.com.cn

Ruby: warn "err"
来源：http://sc.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://ud.hahajie.cn

[M07] 判断是否为主入口
来源：http://mf.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://vn.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://be.nszjky.cn

JS:   require.main === module
来源：http://yd.gzmigu.cn

TS:   require.main === module
来源：http://mk.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://ig.lnxyls.cn

Go:   func main()
来源：http://by.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qy.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://ii.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://du.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://cf.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://nj.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://nz.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://af.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ba.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cl.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qr.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cp.shxzukj.cn

================================================================================
来源：http://lj.muxihuayi.cn

N. 数据结构与算法
来源：http://mi.wgjwhj.cn

================================================================================
来源：http://mo.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://mv.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jx.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iy.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ij.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vt.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ax.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://ww.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ie.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hg.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://fb.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ie.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fe.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sp.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ta.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sw.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://zo.shxzskj.cn

Ruby: arr.sort
来源：http://rr.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ae.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://gj.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xe.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://qn.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qc.wgjwhj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ar.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hx.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ns.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zd.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ki.lnxyls.cn

[N04] 斐波那契数列
来源：http://up.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hl.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pw.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://db.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xo.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ii.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xh.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hh.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://up.gzmigu.cn

[N05] 最大公约数
来源：http://ci.colortex.cn

Py:   math.gcd(a, b)
来源：http://qp.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ab.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ly.huixiangedu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ol.wgjwhj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oq.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ot.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://tn.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hx.huixiangedu.cn

[N06] 判断回文字符串
来源：http://hk.hnjuh.cn

Py:   s == s[::-1]
来源：http://hv.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://mi.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://xw.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://ma.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zd.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://oh.huixiangedu.cn

Ruby: s == s.reverse
来源：http://ac.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://el.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://ca.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vl.asd995.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bc.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sa.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://jl.newstarts.cn

Java: // 手写 HashMap
来源：http://hl.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://eu.hnjuh.cn

Ruby: // 手写 Hash
来源：http://vf.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://af.panjiajie.cn

[N08] 生成全排列
来源：http://ba.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://if.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://pb.shxzskj.cn

JS:   // 手写回溯递归
来源：http://uv.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://ot.huixinmuqiang.cn

Java: // 手写回溯递归
来源：http://qy.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://ev.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://fh.hnjuh.cn

C#:   // 手写回溯递归
来源：http://hq.szxytkj.cn

[N09] 栈与队列
来源：http://zm.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ae.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ku.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zq.shtwfgs.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xk.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yj.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tg.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eh.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wz.chemitech.net.cn

[N10] 链表节点定义
来源：http://tz.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kp.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://iz.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dv.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bh.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://sy.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ew.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fj.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://su.521024.cn

[N11] 二叉树中序遍历
来源：http://be.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cx.hnjuh.cn

PHP:  // 手写递归函数
来源：http://vj.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zo.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nv.newstarts.cn

Java: // 手写递归
来源：http://fm.szxytkj.cn

Go:   // 手写递归
来源：http://as.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uk.bjjhwx.cn

C#:   // 手写递归
来源：http://yr.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lg.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tb.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tj.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ck.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gu.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zo.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hk.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yx.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ow.yuexingan06.cn


<!-- 参考信息 -->