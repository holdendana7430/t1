代发 wailian999

[K02] JSON 字符串转对象
来源：http://ko.lnxyls.cn

Py:   json.loads(s)
来源：http://dl.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ni.szsharing.cn

JS:   JSON.parse(s)
来源：http://xw.shxzskj.cn

TS:   JSON.parse(s)
来源：http://vt.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ip.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://rk.521024.cn

Ruby: JSON.parse(s)
来源：http://ay.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lo.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://jw.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nw.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lw.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zn.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gx.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ic.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bq.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://go.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qy.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://yo.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://no.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qo.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mz.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ve.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lp.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sg.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mn.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eg.huixiangedu.cn

[K05] 深拷贝对象
来源：http://ki.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://lg.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://rc.hnjuh.cn

JS:   structuredClone(obj)
来源：http://cn.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://ek.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bz.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yl.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gz.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mt.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://xi.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kx.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ys.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xx.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dx.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yl.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hh.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eo.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dr.jianghongdianzi.cn

[K07] 进制转换
来源：http://xu.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wh.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gv.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://af.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iw.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://if.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gn.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qk.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ko.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://ah.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://lx.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dc.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://sv.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://bt.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rd.jianghongdianzi.cn

Go:   encoding/gob
来源：http://xa.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://bh.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ox.haigaiapp.cn

================================================================================
来源：http://tp.yuntaijiaju.cn

L. 网络请求
来源：http://lw.jianghongdianzi.cn

================================================================================
来源：http://is.hahajie.cn

[L01] 发送 GET 请求
来源：http://au.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dq.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tb.panjiajie.cn

JS:   await fetch(url)
来源：http://fq.panjiajie.cn

TS:   await fetch(url)
来源：http://xg.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mm.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://ek.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tu.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ap.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://gg.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gf.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eo.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sb.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kg.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ci.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ho.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lf.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bt.nicolike.cn

[L03] 设置自定义请求头
来源：http://zc.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hh.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://me.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wi.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pl.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bl.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://um.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xt.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oe.jctech888.com.cn

[L04] 设置超时
来源：http://wd.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://ai.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bn.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pr.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vb.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dc.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xv.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ga.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ib.huanxung.cn

[L05] 上传文件（multipart）
来源：http://nn.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kb.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kl.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://we.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mc.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dn.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gh.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ye.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zx.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://ng.jctech888.com.cn

Py:   resp.json()
来源：http://dq.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://zx.bookmarksfly.cn

JS:   await resp.json()
来源：http://gh.chemitech.net.cn

TS:   await resp.json()
来源：http://kf.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ai.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nq.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://je.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eu.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://qy.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kx.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fv.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://cn.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://ui.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://dr.chemitech.net.cn

Go:   resp.StatusCode
来源：http://nt.gzmigu.cn

Ruby: resp.code.to_i
来源：http://mn.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://op.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://em.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xz.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://sr.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dx.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jk.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vg.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vq.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vq.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://my.wgjwhj.cn

================================================================================
来源：http://ed.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://ue.haigaiapp.cn

================================================================================
来源：http://pw.wgjwhj.cn

[M01] 读取命令行参数
来源：http://hj.huanxung.cn

Py:   sys.argv[1:]
来源：http://wc.hahajie.cn

PHP:  $argv;  $argc;
来源：http://it.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://oj.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://zn.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://mw.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://ir.jianghongdianzi.cn

Ruby: ARGV
来源：http://go.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://hx.bookmarksfly.cn

[M02] 读取环境变量
来源：http://pr.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://rs.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sl.chemitech.net.cn

JS:   process.env.HOME
来源：http://ab.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://nq.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://rl.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://un.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://pt.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fx.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://wy.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lk.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ei.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cm.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yt.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mq.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mi.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gd.yuntaijiaju.cn

C#:   Process.Start("ls", "-l");
来源：http://fv.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://rd.haigaiapp.cn

Py:   os.getcwd()
来源：http://sm.shtwfgs.cn

PHP:  getcwd();
来源：http://gc.huanxung.cn

JS:   process.cwd()
来源：http://nu.gzmigu.cn

TS:   process.cwd()
来源：http://cp.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://oh.panjiajie.cn

Go:   os.Getwd()
来源：http://hb.gzmigu.cn

Ruby: Dir.pwd
来源：http://ba.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ol.shtwfgs.cn

[M05] 设置退出码
来源：http://cx.shxzukj.cn

Py:   sys.exit(1)
来源：http://jh.bookmarksfly.cn

PHP:  exit(1);
来源：http://ak.muxihuayi.cn

JS:   process.exit(1)
来源：http://ao.9csxet.cn

TS:   process.exit(1)
来源：http://fc.jianghongdianzi.cn

Java: System.exit(1)
来源：http://fg.chemitech.net.cn

Go:   os.Exit(1)
来源：http://js.shtwfgs.cn

Ruby: exit 1
来源：http://qb.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tm.colortex.cn

[M06] 向标准错误输出
来源：http://gz.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://vn.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://km.muxihuayi.cn

JS:   console.error("err")
来源：http://mu.wgjwhj.cn

TS:   console.error("err")
来源：http://eo.shtwfgs.cn

Java: System.err.println("err")
来源：http://qv.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ic.521024.cn

Ruby: warn "err"
来源：http://vo.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://pm.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://nt.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://ri.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ft.shtwfgs.cn

JS:   require.main === module
来源：http://zi.newstarts.cn

TS:   require.main === module
来源：http://oj.gzmigu.cn

Java: public static void main(String[] args)
来源：http://cw.gzmigu.cn

Go:   func main()
来源：http://lo.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://no.9csxet.cn

C#:   static void Main(string[] args)
来源：http://uq.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://kr.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://mt.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://me.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://ho.shxzukj.cn

TS:   process.platform;  process.version
来源：http://aq.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ke.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vo.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cd.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sb.wgjwhj.cn

================================================================================
来源：http://bh.chemitech.net.cn

N. 数据结构与算法
来源：http://oe.nicolike.cn

================================================================================
来源：http://gh.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://ll.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://we.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mg.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qu.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wa.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://km.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://og.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wb.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://oj.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://jn.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://st.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zb.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xq.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rq.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zl.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://dc.asd995.cn

Ruby: arr.sort
来源：http://pw.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bs.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://wb.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ni.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://td.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mn.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://la.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ei.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tn.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tc.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://to.521024.cn

[N04] 斐波那契数列
来源：http://hp.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jd.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tg.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ip.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rz.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jn.colortex.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vp.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://an.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ch.lnxyls.cn

[N05] 最大公约数
来源：http://bs.yuntaijiaju.cn

Py:   math.gcd(a, b)
来源：http://dn.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uv.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://od.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yl.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xp.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uy.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://ys.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://se.chemitech.net.cn

[N06] 判断回文字符串
来源：http://tb.nicolike.cn

Py:   s == s[::-1]
来源：http://tb.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://tj.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://rx.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://pm.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rt.521024.cn

Go:   // 双指针从两端比较
来源：http://bl.bookmarksfly.cn

Ruby: s == s.reverse
来源：http://ru.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cz.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://zh.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dh.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wl.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sg.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://yr.panjiajie.cn

Java: // 手写 HashMap
来源：http://mj.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://tx.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://yx.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zv.colortex.cn

[N08] 生成全排列
来源：http://qf.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://gm.asd995.cn

PHP:  // 手写递归交换
来源：http://md.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://yp.hahajie.cn

TS:   // 手写回溯递归
来源：http://ie.szsharing.cn

Java: // 手写回溯递归
来源：http://vo.asd995.cn

Go:   // 手写回溯递归
来源：http://fm.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://ek.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://zk.9csxet.cn

[N09] 栈与队列
来源：http://aq.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pg.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iq.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ff.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ws.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jw.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yo.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cw.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dm.szxytkj.cn

[N10] 链表节点定义
来源：http://ts.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hf.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hl.jianghongdianzi.cn


<!-- 参考信息 -->