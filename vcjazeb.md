代发 wailian999

================================================================================
来源：http://wx.9csxet.cn

K. JSON 与序列化
来源：http://mg.haigaiapp.cn

================================================================================
来源：http://yb.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://zw.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kz.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xk.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://hd.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://zy.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lk.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://so.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xv.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ki.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://gn.shtwfgs.cn

Py:   json.loads(s)
来源：http://ei.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cr.shxzukj.cn

JS:   JSON.parse(s)
来源：http://sq.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://ni.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://by.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://ev.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://bi.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fe.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://oq.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://og.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://et.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tb.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ip.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nb.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dz.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cd.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pc.hahajie.cn

[K04] 读取 JSON 文件
来源：http://al.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qe.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vv.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dv.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vc.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://to.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cl.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pd.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lu.shxzskj.cn

[K05] 深拷贝对象
来源：http://cm.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://cm.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://lr.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://rn.asd995.cn

TS:   structuredClone(obj)
来源：http://xe.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mu.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tu.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ie.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oy.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://nr.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tj.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sp.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ay.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vz.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kv.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nc.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wk.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jr.panjiajie.cn

[K07] 进制转换
来源：http://pf.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://at.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://it.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uk.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wv.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wv.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bi.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://aq.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cs.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://do.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://kq.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wf.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://yt.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://hb.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ml.asd995.cn

Go:   encoding/gob
来源：http://um.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://ex.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qv.shxzukj.cn

================================================================================
来源：http://pq.huanxung.cn

L. 网络请求
来源：http://nd.newstarts.cn

================================================================================
来源：http://cv.hnjuh.cn

[L01] 发送 GET 请求
来源：http://bn.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ty.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tt.gzmigu.cn

JS:   await fetch(url)
来源：http://pw.shtwfgs.cn

TS:   await fetch(url)
来源：http://wi.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nm.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://kq.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kg.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oc.hnjuh.cn

[L02] 发送 POST JSON
来源：http://xr.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mw.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vw.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uq.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://il.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jx.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lf.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://av.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uu.colortex.cn

[L03] 设置自定义请求头
来源：http://ww.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://le.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ll.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cj.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ra.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ay.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tu.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://us.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bi.hnjuh.cn

[L04] 设置超时
来源：http://vj.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://vr.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yv.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wx.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cl.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kg.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jc.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sv.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aq.asd995.cn

[L05] 上传文件（multipart）
来源：http://aw.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vu.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ye.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tl.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pd.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dk.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://se.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://br.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tt.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://xr.huixinmuqiang.cn

Py:   resp.json()
来源：http://do.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://lr.yuntaijiaju.cn

JS:   await resp.json()
来源：http://tw.yuntaijiaju.cn

TS:   await resp.json()
来源：http://nl.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ty.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yo.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://ud.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ev.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://ww.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cg.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bj.colortex.cn

JS:   resp.ok;  resp.status
来源：http://nb.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://hh.muxihuayi.cn

Java: resp.statusCode()
来源：http://dc.huanxung.cn

Go:   resp.StatusCode
来源：http://gq.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://tj.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://mz.huanxung.cn

[L08] 并发请求多个地址
来源：http://ts.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sx.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://ql.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hk.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bx.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://un.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ha.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mf.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://th.szsharing.cn

================================================================================
来源：http://lb.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://iz.nicolike.cn

================================================================================
来源：http://mn.newstarts.cn

[M01] 读取命令行参数
来源：http://gz.9csxet.cn

Py:   sys.argv[1:]
来源：http://ee.newstarts.cn

PHP:  $argv;  $argc;
来源：http://ar.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://ys.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://an.asd995.cn

Java: args 数组（main 方法参数）
来源：http://yh.huixiangedu.cn

Go:   os.Args[1:]
来源：http://hu.lnxyls.cn

Ruby: ARGV
来源：http://kz.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://lq.lnxyls.cn

[M02] 读取环境变量
来源：http://hd.asd995.cn

Py:   os.environ.get("HOME")
来源：http://vz.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ui.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://pa.asd995.cn

TS:   process.env.HOME
来源：http://tm.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://bv.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ly.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://pw.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://db.nicolike.cn

[M03] 执行外部命令
来源：http://lv.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tv.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wi.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jt.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sz.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wa.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mu.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zy.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://mk.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://ds.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://wx.jianghongdianzi.cn

PHP:  getcwd();
来源：http://oh.nszjky.cn

JS:   process.cwd()
来源：http://wj.panjiajie.cn

TS:   process.cwd()
来源：http://gh.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://he.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://mz.bjjhwx.cn

Ruby: Dir.pwd
来源：http://jx.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yf.huanxung.cn

[M05] 设置退出码
来源：http://pd.shtwfgs.cn

Py:   sys.exit(1)
来源：http://xc.wgjwhj.cn

PHP:  exit(1);
来源：http://or.huixiangedu.cn

JS:   process.exit(1)
来源：http://vk.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://hm.shxzskj.cn

Java: System.exit(1)
来源：http://pi.haigaiapp.cn

Go:   os.Exit(1)
来源：http://pl.newstarts.cn

Ruby: exit 1
来源：http://ny.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hm.521024.cn

[M06] 向标准错误输出
来源：http://mg.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://nm.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sw.shtwfgs.cn

JS:   console.error("err")
来源：http://xz.haigaiapp.cn

TS:   console.error("err")
来源：http://eq.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://io.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ar.gzmigu.cn

Ruby: warn "err"
来源：http://vu.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://yj.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://hj.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://ar.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aa.newstarts.cn

JS:   require.main === module
来源：http://jh.panjiajie.cn

TS:   require.main === module
来源：http://qy.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://ym.haigaiapp.cn

Go:   func main()
来源：http://mx.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ay.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://dt.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://jd.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://sf.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://cv.521024.cn

JS:   process.platform;  process.version
来源：http://yl.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://jw.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cn.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xz.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aq.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xh.colortex.cn

================================================================================
来源：http://fs.huixinmuqiang.cn

N. 数据结构与算法
来源：http://so.huanxung.cn

================================================================================
来源：http://qf.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://zx.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sq.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rl.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wl.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ne.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wf.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://rq.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hm.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cv.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://wz.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://mc.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jo.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vj.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wt.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://da.521024.cn

Go:   slices.Sort(arr)
来源：http://ak.newstarts.cn

Ruby: arr.sort
来源：http://uq.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ae.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://ui.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ok.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://uk.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ng.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jk.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qc.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aw.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uw.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hv.9csxet.cn

[N04] 斐波那契数列
来源：http://yj.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://em.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xl.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mi.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mn.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dn.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wc.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xe.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xh.szxytkj.cn

[N05] 最大公约数
来源：http://rh.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://zm.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ak.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ba.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yh.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tz.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://el.nszjky.cn

Ruby: a.gcd(b)
来源：http://ve.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gf.haigaiapp.cn

[N06] 判断回文字符串
来源：http://qj.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://ut.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://ey.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://sw.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://rt.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wb.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://ip.shtwfgs.cn

Ruby: s == s.reverse
来源：http://ma.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hj.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://ig.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ri.bjjhwx.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qq.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zf.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://kb.521024.cn

Java: // 手写 HashMap
来源：http://xi.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://ba.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://pk.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nv.shxzskj.cn

[N08] 生成全排列
来源：http://gx.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://en.asd995.cn

PHP:  // 手写递归交换
来源：http://qb.9csxet.cn

JS:   // 手写回溯递归
来源：http://dr.colortex.cn

TS:   // 手写回溯递归
来源：http://lq.huanxung.cn

Java: // 手写回溯递归
来源：http://da.shxzskj.cn

Go:   // 手写回溯递归
来源：http://wi.colortex.cn

Ruby: arr.permutation.to_a
来源：http://od.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://uo.szxytkj.cn


<!-- 参考信息 -->