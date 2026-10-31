代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://th.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pu.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yr.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zf.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fr.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jg.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lu.yuexingan06.cn

[K05] 深拷贝对象
来源：http://wh.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://na.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://gp.nicolike.cn

JS:   structuredClone(obj)
来源：http://kb.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://wx.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jm.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ns.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://in.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rk.newstarts.cn

[K06] 解析 URL 查询串
来源：http://lo.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://an.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://us.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jo.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://do.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cx.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gz.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uu.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oq.lnxyls.cn

[K07] 进制转换
来源：http://iw.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hi.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ft.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sh.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qj.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://av.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lc.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zm.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uz.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://dw.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://yb.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ss.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://gh.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://gh.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dh.yuexingan06.cn

Go:   encoding/gob
来源：http://lm.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://iv.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zn.haigaiapp.cn

================================================================================
来源：http://tp.hnjuh.cn

L. 网络请求
来源：http://zj.gzmigu.cn

================================================================================
来源：http://cj.newstarts.cn

[L01] 发送 GET 请求
来源：http://wg.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gk.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vs.521024.cn

JS:   await fetch(url)
来源：http://kk.newstarts.cn

TS:   await fetch(url)
来源：http://bc.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vg.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://jt.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mp.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://at.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://fs.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ly.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wa.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sw.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ox.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mu.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://me.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ur.shxzskj.cn

[L03] 设置自定义请求头
来源：http://sc.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xi.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gr.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bf.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vc.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://er.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vx.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://np.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kb.jianghongdianzi.cn

[L04] 设置超时
来源：http://pe.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://zh.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gp.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eq.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pb.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ck.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://th.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pz.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yf.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://yf.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lj.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ck.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ze.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tq.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://br.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fo.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bj.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://js.szsharing.cn

[L06] 解析响应为 JSON
来源：http://ob.asd995.cn

Py:   resp.json()
来源：http://hq.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://to.9csxet.cn

JS:   await resp.json()
来源：http://gz.yuexingan06.cn

TS:   await resp.json()
来源：http://mq.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ou.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yl.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://px.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pi.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://sp.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wx.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mi.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://br.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://un.nicolike.cn

Java: resp.statusCode()
来源：http://an.asd995.cn

Go:   resp.StatusCode
来源：http://qg.521024.cn

Ruby: resp.code.to_i
来源：http://oo.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://cu.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://ly.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yn.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://ea.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xt.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sj.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wh.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lh.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dm.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bq.newstarts.cn

================================================================================
来源：http://by.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://hx.chemitech.net.cn

================================================================================
来源：http://gs.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://uc.hnjuh.cn

Py:   sys.argv[1:]
来源：http://mr.9csxet.cn

PHP:  $argv;  $argc;
来源：http://ax.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://zu.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://ee.asd995.cn

Java: args 数组（main 方法参数）
来源：http://ob.bjjhwx.cn

Go:   os.Args[1:]
来源：http://zn.huixinmuqiang.cn

Ruby: ARGV
来源：http://mc.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://do.haigaiapp.cn

[M02] 读取环境变量
来源：http://oq.521024.cn

Py:   os.environ.get("HOME")
来源：http://kd.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mu.lnxyls.cn

JS:   process.env.HOME
来源：http://qx.szxytkj.cn

TS:   process.env.HOME
来源：http://lw.nicolike.cn

Java: System.getenv("HOME")
来源：http://ax.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ax.muxihuayi.cn

Ruby: ENV["HOME"]
来源：http://di.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://po.huanxung.cn

[M03] 执行外部命令
来源：http://dg.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oi.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gi.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wc.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tq.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uy.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qw.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://es.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://ol.9csxet.cn

[M04] 获取当前工作目录
来源：http://kp.panjiajie.cn

Py:   os.getcwd()
来源：http://iz.haigaiapp.cn

PHP:  getcwd();
来源：http://ws.asd995.cn

JS:   process.cwd()
来源：http://vs.bookmarksfly.cn

TS:   process.cwd()
来源：http://ly.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://sk.gzmigu.cn

Go:   os.Getwd()
来源：http://pm.szxytkj.cn

Ruby: Dir.pwd
来源：http://ll.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fs.muxihuayi.cn

[M05] 设置退出码
来源：http://du.chemitech.net.cn

Py:   sys.exit(1)
来源：http://vt.szsharing.cn

PHP:  exit(1);
来源：http://dx.yuexingan06.cn

JS:   process.exit(1)
来源：http://an.wgjwhj.cn

TS:   process.exit(1)
来源：http://wx.bookmarksfly.cn

Java: System.exit(1)
来源：http://is.hahajie.cn

Go:   os.Exit(1)
来源：http://jt.panjiajie.cn

Ruby: exit 1
来源：http://qj.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uw.gzmigu.cn

[M06] 向标准错误输出
来源：http://js.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://ga.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kp.huixinmuqiang.cn

JS:   console.error("err")
来源：http://nd.huixinmuqiang.cn

TS:   console.error("err")
来源：http://im.hahajie.cn

Java: System.err.println("err")
来源：http://wz.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dn.bjjhwx.cn

Ruby: warn "err"
来源：http://eq.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://qi.szxytkj.cn

[M07] 判断是否为主入口
来源：http://xa.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://ky.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mz.huanxung.cn

JS:   require.main === module
来源：http://tk.newstarts.cn

TS:   require.main === module
来源：http://co.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://mc.yuntaijiaju.cn

Go:   func main()
来源：http://bx.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xn.hahajie.cn

C#:   static void Main(string[] args)
来源：http://ry.521024.cn

[M08] 获取系统与运行时信息
来源：http://es.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://sm.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://qr.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://ag.gzmigu.cn

TS:   process.platform;  process.version
来源：http://qv.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mb.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yj.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ar.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ub.huixiangedu.cn

================================================================================
来源：http://mh.huanxung.cn

N. 数据结构与算法
来源：http://aq.wgjwhj.cn

================================================================================
来源：http://ud.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://rf.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ru.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dr.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zv.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qi.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qq.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://ga.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wd.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tc.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://fr.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://yh.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lw.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mn.huixinmuqiang.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ee.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ux.huanxung.cn

Go:   slices.Sort(arr)
来源：http://js.jctech888.com.cn

Ruby: arr.sort
来源：http://rb.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://do.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://zm.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://um.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://oh.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kd.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://li.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tx.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mr.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rx.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xn.shtwfgs.cn

[N04] 斐波那契数列
来源：http://gc.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vh.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vd.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://al.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ax.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gm.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dc.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uf.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jc.yuexingan06.cn

[N05] 最大公约数
来源：http://id.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://fw.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vc.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hc.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rm.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lj.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://il.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://oo.521024.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://et.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://co.chemitech.net.cn

Py:   s == s[::-1]
来源：http://zb.9csxet.cn

PHP:  $s === strrev($s);
来源：http://cn.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://hz.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://rq.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jg.521024.cn

Go:   // 双指针从两端比较
来源：http://bd.muxihuayi.cn

Ruby: s == s.reverse
来源：http://lh.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://av.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://jv.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rm.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sc.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cs.huixinmuqiang.cn

TS:   // 手写 Map<string, number>
来源：http://wi.hahajie.cn

Java: // 手写 HashMap
来源：http://jg.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://qn.nszjky.cn

Ruby: // 手写 Hash
来源：http://pe.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vw.bjjhwx.cn

[N08] 生成全排列
来源：http://oa.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://yl.colortex.cn

PHP:  // 手写递归交换
来源：http://sz.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://sb.hnjuh.cn

TS:   // 手写回溯递归
来源：http://kj.nicolike.cn

Java: // 手写回溯递归
来源：http://oz.panjiajie.cn

Go:   // 手写回溯递归
来源：http://jm.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://ur.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://jd.chemitech.net.cn

[N09] 栈与队列
来源：http://nw.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zx.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sg.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ab.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hm.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wu.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iu.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jm.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ef.colortex.cn

[N10] 链表节点定义
来源：http://pj.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ll.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kb.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nd.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://er.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://ad.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gh.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sf.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sa.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://cd.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xi.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://ox.hnjuh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://re.muxihuayi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mn.521024.cn

Java: // 手写递归
来源：http://to.colortex.cn

Go:   // 手写递归
来源：http://ty.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gy.haigaiapp.cn

C#:   // 手写递归
来源：http://xq.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wg.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://da.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lb.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ou.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uu.bjjhwx.cn


<!-- 参考信息 -->