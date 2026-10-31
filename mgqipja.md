代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ei.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jg.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://pg.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://to.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qu.nszjky.cn

Go:   json.Marshal(obj)
来源：http://ig.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ok.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oi.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://lx.hnjuh.cn

Py:   json.loads(s)
来源：http://dk.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gx.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://ns.hnjuh.cn

TS:   JSON.parse(s)
来源：http://kv.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yt.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://sg.asd995.cn

Ruby: JSON.parse(s)
来源：http://zc.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jr.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://mg.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zj.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fk.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tm.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tt.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tr.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ed.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rz.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sc.szsharing.cn

[K04] 读取 JSON 文件
来源：http://uq.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ne.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tt.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qf.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dk.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://us.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uy.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vc.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://id.huixiangedu.cn

[K05] 深拷贝对象
来源：http://yn.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://cb.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://pt.huanxung.cn

JS:   structuredClone(obj)
来源：http://uv.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://zr.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ew.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lv.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dy.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ec.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://ro.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dt.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mw.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pl.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xv.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ae.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pv.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uq.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://re.newstarts.cn

[K07] 进制转换
来源：http://is.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://im.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ab.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qw.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://al.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hr.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oe.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hd.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uk.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://mt.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://ze.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pr.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://uw.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://de.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://um.hahajie.cn

Go:   encoding/gob
来源：http://nh.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://lc.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uh.hahajie.cn

================================================================================
来源：http://mf.szxytkj.cn

L. 网络请求
来源：http://nk.huanxung.cn

================================================================================
来源：http://gh.panjiajie.cn

[L01] 发送 GET 请求
来源：http://ar.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://it.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zr.muxihuayi.cn

JS:   await fetch(url)
来源：http://kh.jctech888.com.cn

TS:   await fetch(url)
来源：http://mv.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fu.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://jy.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vl.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oz.nszjky.cn

[L02] 发送 POST JSON
来源：http://jz.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xr.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bw.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nx.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://du.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jb.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ji.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qs.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pp.newstarts.cn

[L03] 设置自定义请求头
来源：http://yp.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lg.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qx.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jm.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ch.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ht.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zi.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wl.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ym.nicolike.cn

[L04] 设置超时
来源：http://tw.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://bj.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ro.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ej.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yc.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://th.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nm.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tg.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gs.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://gk.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ui.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tx.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rj.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kf.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aq.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mn.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iy.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xh.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://nc.shtwfgs.cn

Py:   resp.json()
来源：http://lg.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://go.huixinmuqiang.cn

JS:   await resp.json()
来源：http://ia.9csxet.cn

TS:   await resp.json()
来源：http://mo.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wx.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://se.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://hz.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ic.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://ya.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jn.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iy.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://ky.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://ng.jctech888.com.cn

Java: resp.statusCode()
来源：http://yn.yuexingan06.cn

Go:   resp.StatusCode
来源：http://zo.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://al.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://lp.szsharing.cn

[L08] 并发请求多个地址
来源：http://fw.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cr.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://oe.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ek.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oe.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lv.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dp.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kx.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tv.9csxet.cn

================================================================================
来源：http://kp.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://tb.gzmigu.cn

================================================================================
来源：http://fi.yuexingan06.cn

[M01] 读取命令行参数
来源：http://pw.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://ss.nszjky.cn

PHP:  $argv;  $argc;
来源：http://id.nicolike.cn

JS:   process.argv.slice(2)
来源：http://tz.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://ow.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://sf.nszjky.cn

Go:   os.Args[1:]
来源：http://jp.jctech888.com.cn

Ruby: ARGV
来源：http://dn.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://zw.yuexingan06.cn

[M02] 读取环境变量
来源：http://jn.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://ot.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qh.muxihuayi.cn

JS:   process.env.HOME
来源：http://bn.asd995.cn

TS:   process.env.HOME
来源：http://xy.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://fx.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dj.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://lg.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://es.shtwfgs.cn

[M03] 执行外部命令
来源：http://qr.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bt.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ty.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cq.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://eb.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bd.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ic.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pt.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://ds.lnxyls.cn

[M04] 获取当前工作目录
来源：http://mm.muxihuayi.cn

Py:   os.getcwd()
来源：http://ox.huixinmuqiang.cn

PHP:  getcwd();
来源：http://sx.shxzukj.cn

JS:   process.cwd()
来源：http://mb.9csxet.cn

TS:   process.cwd()
来源：http://rp.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://cp.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://ko.asd995.cn

Ruby: Dir.pwd
来源：http://fk.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jy.lnxyls.cn

[M05] 设置退出码
来源：http://tz.shtwfgs.cn

Py:   sys.exit(1)
来源：http://kv.chemitech.net.cn

PHP:  exit(1);
来源：http://bd.nicolike.cn

JS:   process.exit(1)
来源：http://kw.shxzskj.cn

TS:   process.exit(1)
来源：http://kq.lnxyls.cn

Java: System.exit(1)
来源：http://dp.asd995.cn

Go:   os.Exit(1)
来源：http://yr.szsharing.cn

Ruby: exit 1
来源：http://tj.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pi.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://yn.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://iy.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vc.yuexingan06.cn

JS:   console.error("err")
来源：http://xc.bookmarksfly.cn

TS:   console.error("err")
来源：http://hf.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://gy.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vt.yuntaijiaju.cn

Ruby: warn "err"
来源：http://ju.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://em.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://bu.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://ot.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rs.szsharing.cn

JS:   require.main === module
来源：http://ws.yuexingan06.cn

TS:   require.main === module
来源：http://om.hahajie.cn

Java: public static void main(String[] args)
来源：http://ge.wgjwhj.cn

Go:   func main()
来源：http://ol.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jw.9csxet.cn

C#:   static void Main(string[] args)
来源：http://xb.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://cm.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://np.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://fw.gzmigu.cn

JS:   process.platform;  process.version
来源：http://nk.9csxet.cn

TS:   process.platform;  process.version
来源：http://ph.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oj.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ix.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zh.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bk.nszjky.cn

================================================================================
来源：http://xv.shtwfgs.cn

N. 数据结构与算法
来源：http://nr.shxzukj.cn

================================================================================
来源：http://bp.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://cp.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://id.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uy.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rn.colortex.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sw.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gj.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ig.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bf.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ap.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://of.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://yu.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yv.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dp.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://af.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fb.hahajie.cn

Go:   slices.Sort(arr)
来源：http://ql.huixiangedu.cn

Ruby: arr.sort
来源：http://fj.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uv.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://ls.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nn.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://fv.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nk.hnjuh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ed.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ub.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ro.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hn.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ns.panjiajie.cn

[N04] 斐波那契数列
来源：http://uk.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zz.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ly.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wc.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qi.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ov.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://es.huanxung.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nm.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fi.nszjky.cn

[N05] 最大公约数
来源：http://ae.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://aj.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fp.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cu.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jt.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xw.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://as.lnxyls.cn

Ruby: a.gcd(b)
来源：http://zc.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://af.haigaiapp.cn

[N06] 判断回文字符串
来源：http://bx.szsharing.cn

Py:   s == s[::-1]
来源：http://lv.asd995.cn

PHP:  $s === strrev($s);
来源：http://hy.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://fa.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://gj.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vc.asd995.cn

Go:   // 双指针从两端比较
来源：http://el.9csxet.cn

Ruby: s == s.reverse
来源：http://pk.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://np.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://am.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pq.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://os.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://eq.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://jv.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://qv.colortex.cn

Go:   // 手写 map[int]int
来源：http://tr.szxytkj.cn

Ruby: // 手写 Hash
来源：http://tw.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tc.521024.cn

[N08] 生成全排列
来源：http://di.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://dt.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://as.9csxet.cn

JS:   // 手写回溯递归
来源：http://wd.hahajie.cn

TS:   // 手写回溯递归
来源：http://wo.shxzukj.cn

Java: // 手写回溯递归
来源：http://ox.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://pe.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://ec.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://ex.nszjky.cn

[N09] 栈与队列
来源：http://rp.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ow.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sj.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bm.shxzskj.cn


<!-- 参考信息 -->