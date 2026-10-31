代发 wailian999

TS:   JSON.parse(s)
来源：http://kp.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://te.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://yt.colortex.cn

Ruby: JSON.parse(s)
来源：http://tt.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ed.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://kz.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rk.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xj.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bv.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fh.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nq.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oi.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bv.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mt.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://bd.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yl.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qa.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qb.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lp.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gm.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://op.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ym.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ha.huixiangedu.cn

[K05] 深拷贝对象
来源：http://te.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://xx.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://xw.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://bp.9csxet.cn

TS:   structuredClone(obj)
来源：http://zw.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ss.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gc.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://la.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uv.hahajie.cn

[K06] 解析 URL 查询串
来源：http://sx.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cc.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://am.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wv.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wd.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bq.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://go.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vx.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bq.bookmarksfly.cn

[K07] 进制转换
来源：http://fl.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xr.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iw.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gq.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ik.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pm.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rz.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://te.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bs.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://wh.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://pt.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rz.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://sv.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://dc.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lf.bjjhwx.cn

Go:   encoding/gob
来源：http://xq.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://qq.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ew.9csxet.cn

================================================================================
来源：http://dj.nicolike.cn

L. 网络请求
来源：http://xq.yuntaijiaju.cn

================================================================================
来源：http://ay.nszjky.cn

[L01] 发送 GET 请求
来源：http://fp.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bp.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tn.yuexingan06.cn

JS:   await fetch(url)
来源：http://jg.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://yr.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://he.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://po.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lf.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xp.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://vp.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pf.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ol.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://il.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://av.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nw.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hs.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rc.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dh.newstarts.cn

[L03] 设置自定义请求头
来源：http://mx.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gh.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zu.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dm.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ar.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xz.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ih.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tq.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mk.asd995.cn

[L04] 设置超时
来源：http://xe.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://cs.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gc.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bs.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xu.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gg.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pb.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rx.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xz.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://hy.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wa.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ii.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ij.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gt.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uz.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ra.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ng.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hr.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://dj.haigaiapp.cn

Py:   resp.json()
来源：http://dn.nszjky.cn

PHP:  json_decode($body, true);
来源：http://zl.chemitech.net.cn

JS:   await resp.json()
来源：http://mv.yuntaijiaju.cn

TS:   await resp.json()
来源：http://ip.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pe.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qa.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://nx.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xj.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://an.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bc.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gh.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://zn.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://pz.shxzskj.cn

Java: resp.statusCode()
来源：http://rx.jctech888.com.cn

Go:   resp.StatusCode
来源：http://hp.shxzskj.cn

Ruby: resp.code.to_i
来源：http://eg.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://nq.hnjuh.cn

[L08] 并发请求多个地址
来源：http://in.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hy.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://vw.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hx.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tq.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://au.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mp.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rp.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ie.chemitech.net.cn

================================================================================
来源：http://ud.521024.cn

M. 命令行 / 进程 / 环境
来源：http://rt.asd995.cn

================================================================================
来源：http://nb.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://wx.shxzskj.cn

Py:   sys.argv[1:]
来源：http://iq.nszjky.cn

PHP:  $argv;  $argc;
来源：http://jv.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://ya.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://by.colortex.cn

Java: args 数组（main 方法参数）
来源：http://zb.haigaiapp.cn

Go:   os.Args[1:]
来源：http://mr.yuntaijiaju.cn

Ruby: ARGV
来源：http://mm.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://sa.wgjwhj.cn

[M02] 读取环境变量
来源：http://re.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://yk.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xf.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://tt.huanxung.cn

TS:   process.env.HOME
来源：http://di.newstarts.cn

Java: System.getenv("HOME")
来源：http://pe.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jo.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://pj.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nz.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://ss.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ax.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://id.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rw.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cq.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ho.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ki.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yw.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://is.szsharing.cn

[M04] 获取当前工作目录
来源：http://ar.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://zh.haigaiapp.cn

PHP:  getcwd();
来源：http://dx.huanxung.cn

JS:   process.cwd()
来源：http://ik.shxzukj.cn

TS:   process.cwd()
来源：http://ic.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://rg.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://if.hahajie.cn

Ruby: Dir.pwd
来源：http://va.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ln.szsharing.cn

[M05] 设置退出码
来源：http://or.jctech888.com.cn

Py:   sys.exit(1)
来源：http://wl.asd995.cn

PHP:  exit(1);
来源：http://rl.chemitech.net.cn

JS:   process.exit(1)
来源：http://op.wgjwhj.cn

TS:   process.exit(1)
来源：http://wa.shxzskj.cn

Java: System.exit(1)
来源：http://vj.521024.cn

Go:   os.Exit(1)
来源：http://ht.chemitech.net.cn

Ruby: exit 1
来源：http://nk.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://to.muxihuayi.cn

[M06] 向标准错误输出
来源：http://yb.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://er.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ua.huixiangedu.cn

JS:   console.error("err")
来源：http://fj.newstarts.cn

TS:   console.error("err")
来源：http://eb.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://oh.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ta.hnjuh.cn

Ruby: warn "err"
来源：http://in.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://ul.newstarts.cn

[M07] 判断是否为主入口
来源：http://is.521024.cn

Py:   if __name__ == "__main__":
来源：http://pv.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dh.huanxung.cn

JS:   require.main === module
来源：http://vd.jianghongdianzi.cn

TS:   require.main === module
来源：http://ui.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://zk.jctech888.com.cn

Go:   func main()
来源：http://jd.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yt.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://wv.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://ba.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://dh.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://ll.newstarts.cn

JS:   process.platform;  process.version
来源：http://he.shxzskj.cn

TS:   process.platform;  process.version
来源：http://xh.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qr.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nr.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lk.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dv.lnxyls.cn

================================================================================
来源：http://ah.szxytkj.cn

N. 数据结构与算法
来源：http://ya.9csxet.cn

================================================================================
来源：http://ew.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://xr.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yo.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ur.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zy.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nd.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pf.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://hk.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sc.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xw.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://sl.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://yw.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ux.wgjwhj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ub.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xx.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ag.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://dq.nszjky.cn

Ruby: arr.sort
来源：http://jr.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lz.asd995.cn

[N03] 快速排序（分治示例）
来源：http://ku.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cr.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://cc.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ao.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tf.newstarts.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zz.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iw.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ph.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ob.asd995.cn

[N04] 斐波那契数列
来源：http://nk.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aq.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ur.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wd.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xk.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yg.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ji.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vv.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://al.jctech888.com.cn

[N05] 最大公约数
来源：http://bh.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://zo.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xb.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sr.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qw.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vq.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uj.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://gh.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fe.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://lp.hnjuh.cn

Py:   s == s[::-1]
来源：http://en.yuntaijiaju.cn

PHP:  $s === strrev($s);
来源：http://tg.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://ep.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://ex.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pz.nicolike.cn

Go:   // 双指针从两端比较
来源：http://wz.yuexingan06.cn

Ruby: s == s.reverse
来源：http://mb.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://va.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://yd.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kp.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ei.bjjhwx.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xf.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://gl.bjjhwx.cn

Java: // 手写 HashMap
来源：http://la.szsharing.cn

Go:   // 手写 map[int]int
来源：http://yv.shtwfgs.cn

Ruby: // 手写 Hash
来源：http://rg.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wl.huixinmuqiang.cn

[N08] 生成全排列
来源：http://mr.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://ng.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://rg.szxytkj.cn

JS:   // 手写回溯递归
来源：http://ri.panjiajie.cn

TS:   // 手写回溯递归
来源：http://da.szsharing.cn

Java: // 手写回溯递归
来源：http://ir.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://qz.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://hy.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://qg.jianghongdianzi.cn

[N09] 栈与队列
来源：http://em.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mn.asd995.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ju.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://km.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bb.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oe.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fq.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hm.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wd.yuexingan06.cn

[N10] 链表节点定义
来源：http://rh.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ng.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fj.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qu.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tg.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://ac.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vn.nicolike.cn


<!-- 参考信息 -->