代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nj.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rz.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yp.asd995.cn

[K05] 深拷贝对象
来源：http://ng.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://zp.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://vs.nicolike.cn

JS:   structuredClone(obj)
来源：http://lc.szxytkj.cn

TS:   structuredClone(obj)
来源：http://uf.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wx.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hb.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sn.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rs.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://vs.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tn.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nm.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zp.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hb.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cj.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hq.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wr.huixinmuqiang.cn

[K07] 进制转换
来源：http://ii.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fx.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hy.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wo.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xz.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ta.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cu.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zs.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qd.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://me.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://rp.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fc.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://oo.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://ol.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://he.newstarts.cn

Go:   encoding/gob
来源：http://sd.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://zg.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cw.nszjky.cn

================================================================================
来源：http://ic.szsharing.cn

L. 网络请求
来源：http://pr.muxihuayi.cn

================================================================================
来源：http://kv.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://mq.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ca.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ll.hnjuh.cn

JS:   await fetch(url)
来源：http://jt.521024.cn

TS:   await fetch(url)
来源：http://dx.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jf.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://lu.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rd.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rc.nicolike.cn

[L02] 发送 POST JSON
来源：http://tw.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ut.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://si.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hc.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cs.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bx.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://py.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vv.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zm.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://kl.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yj.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hn.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qi.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mb.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mj.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gn.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yc.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nx.hahajie.cn

[L04] 设置超时
来源：http://ek.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://au.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oq.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://je.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uo.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://re.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tk.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kn.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nz.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://yj.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dc.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lm.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fc.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qs.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dt.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pw.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cy.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kg.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://gn.szsharing.cn

Py:   resp.json()
来源：http://uh.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://gc.colortex.cn

JS:   await resp.json()
来源：http://bk.szxytkj.cn

TS:   await resp.json()
来源：http://ac.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uk.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ed.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://ha.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rm.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://cj.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hn.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ph.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://fu.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://ux.muxihuayi.cn

Java: resp.statusCode()
来源：http://mo.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://kz.szxytkj.cn

Ruby: resp.code.to_i
来源：http://hz.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://wz.shxzskj.cn

[L08] 并发请求多个地址
来源：http://wf.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cn.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://hm.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sb.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nr.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fu.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cv.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wb.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uf.bookmarksfly.cn

================================================================================
来源：http://of.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://qz.muxihuayi.cn

================================================================================
来源：http://ho.newstarts.cn

[M01] 读取命令行参数
来源：http://uu.521024.cn

Py:   sys.argv[1:]
来源：http://qe.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://oy.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://wg.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://si.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://vm.shxzukj.cn

Go:   os.Args[1:]
来源：http://es.nszjky.cn

Ruby: ARGV
来源：http://bb.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://mu.chemitech.net.cn

[M02] 读取环境变量
来源：http://bj.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://ua.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uo.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://re.colortex.cn

TS:   process.env.HOME
来源：http://cz.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://ez.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gx.hahajie.cn

Ruby: ENV["HOME"]
来源：http://rj.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vc.bjjhwx.cn

[M03] 执行外部命令
来源：http://dk.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hd.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yv.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ye.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://db.shxzskj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://de.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ap.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kv.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://ca.nszjky.cn

[M04] 获取当前工作目录
来源：http://dx.huanxung.cn

Py:   os.getcwd()
来源：http://qo.9csxet.cn

PHP:  getcwd();
来源：http://ex.wgjwhj.cn

JS:   process.cwd()
来源：http://pf.nszjky.cn

TS:   process.cwd()
来源：http://ia.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://lw.hahajie.cn

Go:   os.Getwd()
来源：http://db.haigaiapp.cn

Ruby: Dir.pwd
来源：http://as.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wv.haigaiapp.cn

[M05] 设置退出码
来源：http://im.9csxet.cn

Py:   sys.exit(1)
来源：http://sb.yuexingan06.cn

PHP:  exit(1);
来源：http://fl.asd995.cn

JS:   process.exit(1)
来源：http://qq.muxihuayi.cn

TS:   process.exit(1)
来源：http://vr.yuexingan06.cn

Java: System.exit(1)
来源：http://xi.huixiangedu.cn

Go:   os.Exit(1)
来源：http://vu.asd995.cn

Ruby: exit 1
来源：http://jr.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dy.shtwfgs.cn

[M06] 向标准错误输出
来源：http://xy.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://qq.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fa.asd995.cn

JS:   console.error("err")
来源：http://hi.asd995.cn

TS:   console.error("err")
来源：http://yu.nszjky.cn

Java: System.err.println("err")
来源：http://lh.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ns.chemitech.net.cn

Ruby: warn "err"
来源：http://dk.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://sw.gzmigu.cn

[M07] 判断是否为主入口
来源：http://ia.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://fc.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jt.chemitech.net.cn

JS:   require.main === module
来源：http://na.haigaiapp.cn

TS:   require.main === module
来源：http://jp.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://ul.bookmarksfly.cn

Go:   func main()
来源：http://av.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fv.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://ct.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://ta.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://iv.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://gz.521024.cn

JS:   process.platform;  process.version
来源：http://zh.newstarts.cn

TS:   process.platform;  process.version
来源：http://rh.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xv.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yg.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tk.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jo.shxzukj.cn

================================================================================
来源：http://kf.jianghongdianzi.cn

N. 数据结构与算法
来源：http://ts.bjjhwx.cn

================================================================================
来源：http://ty.colortex.cn

[N01] 二分查找（有序数组）
来源：http://hg.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qn.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sv.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gs.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mp.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ui.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://vv.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ot.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ju.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://gg.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://zt.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hc.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gv.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mr.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nd.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://nb.gzmigu.cn

Ruby: arr.sort
来源：http://gu.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rq.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://gd.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pi.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://zb.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ut.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lp.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gk.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sl.bjjhwx.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iv.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sz.jctech888.com.cn

[N04] 斐波那契数列
来源：http://fm.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qt.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vk.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kg.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yq.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zw.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://di.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pl.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mi.yuntaijiaju.cn

[N05] 最大公约数
来源：http://ro.huanxung.cn

Py:   math.gcd(a, b)
来源：http://xo.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ty.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kg.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pn.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://no.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://va.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://cy.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ev.jctech888.com.cn

[N06] 判断回文字符串
来源：http://jr.bjjhwx.cn

Py:   s == s[::-1]
来源：http://zr.huanxung.cn

PHP:  $s === strrev($s);
来源：http://nd.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://sd.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://ll.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://su.521024.cn

Go:   // 双指针从两端比较
来源：http://nn.haigaiapp.cn

Ruby: s == s.reverse
来源：http://kh.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lc.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://he.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hr.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xw.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://es.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://xz.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://tq.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://ti.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://bt.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ue.jianghongdianzi.cn

[N08] 生成全排列
来源：http://ow.jianghongdianzi.cn

Py:   itertools.permutations(arr)
来源：http://vi.newstarts.cn

PHP:  // 手写递归交换
来源：http://dl.hnjuh.cn

JS:   // 手写回溯递归
来源：http://jb.colortex.cn

TS:   // 手写回溯递归
来源：http://sh.huixiangedu.cn

Java: // 手写回溯递归
来源：http://tf.hnjuh.cn

Go:   // 手写回溯递归
来源：http://sd.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://ci.asd995.cn

C#:   // 手写回溯递归
来源：http://ve.huixinmuqiang.cn

[N09] 栈与队列
来源：http://hn.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ph.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lj.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nx.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ms.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://de.jctech888.com.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lk.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mv.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://it.nszjky.cn

[N10] 链表节点定义
来源：http://zp.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wg.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jt.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mh.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gy.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://fs.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wa.9csxet.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sf.bookmarksfly.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://id.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://ua.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gh.newstarts.cn

PHP:  // 手写递归函数
来源：http://hc.hnjuh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qt.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zg.nszjky.cn

Java: // 手写递归
来源：http://pe.hnjuh.cn

Go:   // 手写递归
来源：http://mk.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fv.muxihuayi.cn

C#:   // 手写递归
来源：http://uj.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sn.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mt.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ud.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ld.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fr.wgjwhj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hi.bookmarksfly.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nu.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://up.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ku.szsharing.cn


<!-- 参考信息 -->