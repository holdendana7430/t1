代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://jd.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://ac.szsharing.cn

JS:   structuredClone(obj)
来源：http://xj.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://ce.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fn.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ac.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ub.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tt.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://yq.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iq.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kk.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kz.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ft.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bz.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sw.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kg.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ff.shtwfgs.cn

[K07] 进制转换
来源：http://zv.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rt.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hj.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eq.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ca.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ly.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yj.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tc.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zj.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://wn.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://tq.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lw.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://tx.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://zl.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xu.shxzskj.cn

Go:   encoding/gob
来源：http://gk.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://cp.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hr.jctech888.com.cn

================================================================================
来源：http://mn.huanxung.cn

L. 网络请求
来源：http://cw.panjiajie.cn

================================================================================
来源：http://hv.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://pp.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rj.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xp.szsharing.cn

JS:   await fetch(url)
来源：http://gc.nszjky.cn

TS:   await fetch(url)
来源：http://dj.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ug.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://tx.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yw.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dj.nszjky.cn

[L02] 发送 POST JSON
来源：http://ww.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ne.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sv.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ff.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ym.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xe.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kk.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fg.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oe.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://li.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pb.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fq.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lu.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://of.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eh.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hx.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zg.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fj.521024.cn

[L04] 设置超时
来源：http://vy.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://ux.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oy.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xo.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wn.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rq.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xh.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ey.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gw.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://ex.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vs.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zu.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uj.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kt.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dp.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sq.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fx.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yh.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://wy.jctech888.com.cn

Py:   resp.json()
来源：http://iy.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://dm.panjiajie.cn

JS:   await resp.json()
来源：http://ef.shxzskj.cn

TS:   await resp.json()
来源：http://rj.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://go.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cw.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://ml.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qx.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://pf.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ic.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nk.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://kz.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://zl.newstarts.cn

Java: resp.statusCode()
来源：http://cw.wgjwhj.cn

Go:   resp.StatusCode
来源：http://ri.gzmigu.cn

Ruby: resp.code.to_i
来源：http://dp.asd995.cn

C#:   (int)resp.StatusCode
来源：http://dd.asd995.cn

[L08] 并发请求多个地址
来源：http://cg.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lw.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://ms.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ch.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://od.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kq.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ko.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wh.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cv.haigaiapp.cn

================================================================================
来源：http://hu.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://bz.hahajie.cn

================================================================================
来源：http://bo.wgjwhj.cn

[M01] 读取命令行参数
来源：http://ta.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://db.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://ex.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://ws.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://oq.521024.cn

Java: args 数组（main 方法参数）
来源：http://jr.panjiajie.cn

Go:   os.Args[1:]
来源：http://wo.yuexingan06.cn

Ruby: ARGV
来源：http://lh.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://dc.521024.cn

[M02] 读取环境变量
来源：http://kw.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://sc.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ua.bjjhwx.cn

JS:   process.env.HOME
来源：http://oj.lnxyls.cn

TS:   process.env.HOME
来源：http://xd.nicolike.cn

Java: System.getenv("HOME")
来源：http://lh.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jx.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://wg.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gb.gzmigu.cn

[M03] 执行外部命令
来源：http://rh.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://si.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qs.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://eh.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jd.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oq.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xq.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oe.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://lf.szsharing.cn

[M04] 获取当前工作目录
来源：http://ii.szsharing.cn

Py:   os.getcwd()
来源：http://do.nicolike.cn

PHP:  getcwd();
来源：http://of.bjjhwx.cn

JS:   process.cwd()
来源：http://ha.huixiangedu.cn

TS:   process.cwd()
来源：http://lq.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://yo.yuexingan06.cn

Go:   os.Getwd()
来源：http://zp.shxzukj.cn

Ruby: Dir.pwd
来源：http://ru.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uu.muxihuayi.cn

[M05] 设置退出码
来源：http://tr.nicolike.cn

Py:   sys.exit(1)
来源：http://nx.yuntaijiaju.cn

PHP:  exit(1);
来源：http://kr.bookmarksfly.cn

JS:   process.exit(1)
来源：http://sh.521024.cn

TS:   process.exit(1)
来源：http://hn.jctech888.com.cn

Java: System.exit(1)
来源：http://jt.gzmigu.cn

Go:   os.Exit(1)
来源：http://pl.szxytkj.cn

Ruby: exit 1
来源：http://ty.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nl.haigaiapp.cn

[M06] 向标准错误输出
来源：http://hv.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://cd.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ek.nicolike.cn

JS:   console.error("err")
来源：http://ry.szsharing.cn

TS:   console.error("err")
来源：http://we.newstarts.cn

Java: System.err.println("err")
来源：http://lu.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jr.haigaiapp.cn

Ruby: warn "err"
来源：http://cs.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://lv.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://ms.panjiajie.cn

Py:   if __name__ == "__main__":
来源：http://dm.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iv.huanxung.cn

JS:   require.main === module
来源：http://ol.lnxyls.cn

TS:   require.main === module
来源：http://cd.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://hv.9csxet.cn

Go:   func main()
来源：http://gs.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lq.9csxet.cn

C#:   static void Main(string[] args)
来源：http://ee.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://ik.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://pj.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://kz.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://jm.gzmigu.cn

TS:   process.platform;  process.version
来源：http://jw.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tj.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vz.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mx.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bz.9csxet.cn

================================================================================
来源：http://vb.shxzskj.cn

N. 数据结构与算法
来源：http://qr.hnjuh.cn

================================================================================
来源：http://ju.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://xc.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uz.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fu.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ol.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nb.szxytkj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://an.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://xi.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ma.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vu.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://dy.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ks.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ss.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bh.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bb.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bx.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://tg.shxzskj.cn

Ruby: arr.sort
来源：http://on.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ji.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://ua.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ws.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://jv.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sy.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vm.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lc.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zm.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ec.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ab.shxzukj.cn

[N04] 斐波那契数列
来源：http://ts.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sa.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://im.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yh.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mc.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pr.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yu.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ge.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ps.9csxet.cn

[N05] 最大公约数
来源：http://zz.szsharing.cn

Py:   math.gcd(a, b)
来源：http://tu.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vr.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oj.jctech888.com.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sk.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kk.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pm.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://da.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ph.gzmigu.cn

[N06] 判断回文字符串
来源：http://uh.shtwfgs.cn

Py:   s == s[::-1]
来源：http://qs.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://rh.jctech888.com.cn

JS:   s === [...s].reverse().join("")
来源：http://yt.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://lb.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jc.nszjky.cn

Go:   // 双指针从两端比较
来源：http://qe.9csxet.cn

Ruby: s == s.reverse
来源：http://jh.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://az.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://cc.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tk.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fv.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zj.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://rh.yuexingan06.cn

Java: // 手写 HashMap
来源：http://kq.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://wv.shxzskj.cn

Ruby: // 手写 Hash
来源：http://lm.szxytkj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mp.huixiangedu.cn

[N08] 生成全排列
来源：http://ye.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://xl.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://yg.panjiajie.cn

JS:   // 手写回溯递归
来源：http://gs.521024.cn

TS:   // 手写回溯递归
来源：http://jx.wgjwhj.cn

Java: // 手写回溯递归
来源：http://xd.shxzukj.cn

Go:   // 手写回溯递归
来源：http://te.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://nt.gzmigu.cn

C#:   // 手写回溯递归
来源：http://nu.huanxung.cn

[N09] 栈与队列
来源：http://eu.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gm.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jn.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kz.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qc.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mi.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gu.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yk.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fn.nicolike.cn

[N10] 链表节点定义
来源：http://se.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ze.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://st.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://od.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ry.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://ub.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ou.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yz.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://al.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://pi.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ar.521024.cn

PHP:  // 手写递归函数
来源：http://em.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vr.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gm.jctech888.com.cn

Java: // 手写递归
来源：http://om.hahajie.cn

Go:   // 手写递归
来源：http://ld.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ht.9csxet.cn

C#:   // 手写递归
来源：http://av.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hy.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iw.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sr.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fi.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kq.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://st.bjjhwx.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://da.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rk.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zk.asd995.cn

================================================================================
来源：http://wd.szsharing.cn

O. 并发与异步
来源：http://nu.9csxet.cn

================================================================================
来源：http://jb.asd995.cn

[O01] 启动一个线程
来源：http://bk.gzmigu.cn


<!-- 参考信息 -->