代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://hl.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ev.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://km.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ln.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ep.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cn.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dx.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yd.shxzukj.cn

================================================================================
来源：http://jn.hahajie.cn

K. JSON 与序列化
来源：http://cv.521024.cn

================================================================================
来源：http://jw.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://lk.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://py.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gf.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://mc.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://ev.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ku.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://yy.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bu.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tv.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://qk.bjjhwx.cn

Py:   json.loads(s)
来源：http://kx.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://in.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://xx.gzmigu.cn

TS:   JSON.parse(s)
来源：http://jt.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://is.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://dd.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://lx.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tz.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://fn.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cp.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kn.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xv.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rr.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dk.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sq.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aa.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ah.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://ca.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fc.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sl.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://si.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zd.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yt.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fy.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yx.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://po.szsharing.cn

[K05] 深拷贝对象
来源：http://nk.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://hz.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://yk.asd995.cn

JS:   structuredClone(obj)
来源：http://vt.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://zr.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://om.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://na.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zp.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://df.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://ku.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qu.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zb.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xx.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hx.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zp.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wv.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fd.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gb.jianghongdianzi.cn

[K07] 进制转换
来源：http://tw.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qx.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qc.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wb.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zi.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gp.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sc.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qr.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sw.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://jo.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://gj.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ia.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://qi.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://mk.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vg.gzmigu.cn

Go:   encoding/gob
来源：http://bt.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://vw.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gc.lnxyls.cn

================================================================================
来源：http://uv.newstarts.cn

L. 网络请求
来源：http://pc.szxytkj.cn

================================================================================
来源：http://vj.asd995.cn

[L01] 发送 GET 请求
来源：http://pd.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kb.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://it.shxzskj.cn

JS:   await fetch(url)
来源：http://xg.hnjuh.cn

TS:   await fetch(url)
来源：http://nn.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tw.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://ts.huixiangedu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jn.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tp.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://tq.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ms.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ot.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cq.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mp.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ki.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eb.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fd.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mt.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://yr.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yf.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://if.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uv.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ft.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mw.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qq.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sz.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jw.9csxet.cn

[L04] 设置超时
来源：http://zc.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://ju.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cx.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cx.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sn.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yp.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zj.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mg.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ai.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://ra.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jz.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bm.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dx.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://er.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zk.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jw.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ka.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ni.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://mh.newstarts.cn

Py:   resp.json()
来源：http://ie.newstarts.cn

PHP:  json_decode($body, true);
来源：http://xc.jctech888.com.cn

JS:   await resp.json()
来源：http://vz.chemitech.net.cn

TS:   await resp.json()
来源：http://qd.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nb.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yv.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://jk.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ue.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://fh.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xw.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ej.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://mw.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://ud.yuexingan06.cn

Java: resp.statusCode()
来源：http://dg.hahajie.cn

Go:   resp.StatusCode
来源：http://at.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://tt.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://oa.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://wl.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yn.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://bu.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nh.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aw.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pa.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rc.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qn.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ii.gzmigu.cn

================================================================================
来源：http://gu.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://fb.bjjhwx.cn

================================================================================
来源：http://gl.huixiangedu.cn

[M01] 读取命令行参数
来源：http://oe.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://oo.521024.cn

PHP:  $argv;  $argc;
来源：http://hw.521024.cn

JS:   process.argv.slice(2)
来源：http://eh.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://qs.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://mk.muxihuayi.cn

Go:   os.Args[1:]
来源：http://kt.nicolike.cn

Ruby: ARGV
来源：http://pu.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://xw.huanxung.cn

[M02] 读取环境变量
来源：http://wm.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://fo.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eh.shxzskj.cn

JS:   process.env.HOME
来源：http://uk.wgjwhj.cn

TS:   process.env.HOME
来源：http://no.szxytkj.cn

Java: System.getenv("HOME")
来源：http://py.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://up.asd995.cn

Ruby: ENV["HOME"]
来源：http://hg.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vr.hnjuh.cn

[M03] 执行外部命令
来源：http://uc.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yi.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fg.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vy.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ve.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rt.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nk.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rs.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://yp.shxzukj.cn

[M04] 获取当前工作目录
来源：http://zw.chemitech.net.cn

Py:   os.getcwd()
来源：http://sj.521024.cn

PHP:  getcwd();
来源：http://xo.muxihuayi.cn

JS:   process.cwd()
来源：http://jm.huixiangedu.cn

TS:   process.cwd()
来源：http://mb.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://yz.muxihuayi.cn

Go:   os.Getwd()
来源：http://cn.shtwfgs.cn

Ruby: Dir.pwd
来源：http://py.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uq.asd995.cn

[M05] 设置退出码
来源：http://qe.jctech888.com.cn

Py:   sys.exit(1)
来源：http://qb.panjiajie.cn

PHP:  exit(1);
来源：http://nu.asd995.cn

JS:   process.exit(1)
来源：http://zo.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://bw.colortex.cn

Java: System.exit(1)
来源：http://be.bjjhwx.cn

Go:   os.Exit(1)
来源：http://ek.yuexingan06.cn

Ruby: exit 1
来源：http://pz.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bq.bjjhwx.cn

[M06] 向标准错误输出
来源：http://pk.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://wh.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://oe.huixinmuqiang.cn

JS:   console.error("err")
来源：http://qg.szsharing.cn

TS:   console.error("err")
来源：http://qj.yuexingan06.cn

Java: System.err.println("err")
来源：http://ym.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mk.chemitech.net.cn

Ruby: warn "err"
来源：http://al.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://nr.colortex.cn

[M07] 判断是否为主入口
来源：http://sf.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://yz.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kp.bookmarksfly.cn

JS:   require.main === module
来源：http://aq.szxytkj.cn

TS:   require.main === module
来源：http://jj.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://ok.yuntaijiaju.cn

Go:   func main()
来源：http://oh.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dy.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://tw.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://gz.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://eq.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://mx.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://ao.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://wl.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ia.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ng.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yc.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yg.bookmarksfly.cn

================================================================================
来源：http://iy.colortex.cn

N. 数据结构与算法
来源：http://ig.nszjky.cn

================================================================================
来源：http://iu.jianghongdianzi.cn

[N01] 二分查找（有序数组）
来源：http://kf.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xw.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zn.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tz.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://es.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ou.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://vl.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ob.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://go.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://gv.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://xc.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yz.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kn.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lv.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ta.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://ni.asd995.cn

Ruby: arr.sort
来源：http://ak.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ry.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://fz.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xk.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://ye.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vw.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fz.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nx.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sq.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ew.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ow.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://fz.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ds.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ve.huixiangedu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qy.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rc.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://io.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fq.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yl.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sf.jianghongdianzi.cn

[N05] 最大公约数
来源：http://yi.nszjky.cn

Py:   math.gcd(a, b)
来源：http://jz.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pj.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hi.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://be.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://li.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uw.szsharing.cn

Ruby: a.gcd(b)
来源：http://zn.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mr.szxytkj.cn

[N06] 判断回文字符串
来源：http://qe.bjjhwx.cn

Py:   s == s[::-1]
来源：http://vh.9csxet.cn

PHP:  $s === strrev($s);
来源：http://qp.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://om.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://gw.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nm.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://hv.szsharing.cn

Ruby: s == s.reverse
来源：http://lb.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ik.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://yl.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cx.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dl.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vh.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://lk.nicolike.cn

Java: // 手写 HashMap
来源：http://hp.szsharing.cn

Go:   // 手写 map[int]int
来源：http://rq.shxzukj.cn

Ruby: // 手写 Hash
来源：http://ca.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ym.huanxung.cn

[N08] 生成全排列
来源：http://ve.wgjwhj.cn


<!-- 参考信息 -->