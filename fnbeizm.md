代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aj.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://og.jianghongdianzi.cn

[J09] 时区处理
来源：http://qc.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sr.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gp.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uc.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qc.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mv.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jn.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nz.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ra.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://go.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hw.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://md.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://am.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zm.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zs.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gq.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hv.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kb.newstarts.cn

================================================================================
来源：http://hz.chemitech.net.cn

K. JSON 与序列化
来源：http://ye.jianghongdianzi.cn

================================================================================
来源：http://wn.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://mp.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nd.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://th.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://bq.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://cx.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cf.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://qa.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tg.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rp.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://wf.shtwfgs.cn

Py:   json.loads(s)
来源：http://ti.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fi.szxytkj.cn

JS:   JSON.parse(s)
来源：http://fh.newstarts.cn

TS:   JSON.parse(s)
来源：http://sw.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xe.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ed.nszjky.cn

Ruby: JSON.parse(s)
来源：http://eo.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dn.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://jk.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://af.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nd.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://un.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ob.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vm.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://om.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ro.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kz.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://gh.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nq.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jp.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ob.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ey.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ln.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cu.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gz.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ub.panjiajie.cn

[K05] 深拷贝对象
来源：http://lk.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://ee.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://td.hnjuh.cn

JS:   structuredClone(obj)
来源：http://ch.panjiajie.cn

TS:   structuredClone(obj)
来源：http://qk.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://iz.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://se.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rt.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tr.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://eo.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://al.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zj.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pe.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iy.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rd.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ne.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bi.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rg.colortex.cn

[K07] 进制转换
来源：http://rb.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vh.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://an.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ic.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://is.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uu.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ts.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mg.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zm.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://dk.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://bx.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fa.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://va.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://pc.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jg.huixiangedu.cn

Go:   encoding/gob
来源：http://at.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://sw.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ft.lnxyls.cn

================================================================================
来源：http://ir.haigaiapp.cn

L. 网络请求
来源：http://qm.jianghongdianzi.cn

================================================================================
来源：http://rw.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://xg.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sy.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jv.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://wj.haigaiapp.cn

TS:   await fetch(url)
来源：http://pr.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eu.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://vj.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pk.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xf.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://xr.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yi.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://so.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zi.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ev.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zd.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fi.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nv.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wl.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://xr.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hd.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vs.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hu.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ci.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sd.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rr.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cq.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nf.wgjwhj.cn

[L04] 设置超时
来源：http://pl.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://ay.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jr.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lb.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vg.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://he.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jr.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vj.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zk.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://dt.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rp.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vg.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sl.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://li.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rs.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wa.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zq.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hx.hahajie.cn

[L06] 解析响应为 JSON
来源：http://pq.shxzukj.cn

Py:   resp.json()
来源：http://qw.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://gn.yuexingan06.cn

JS:   await resp.json()
来源：http://om.huixinmuqiang.cn

TS:   await resp.json()
来源：http://bu.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oo.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hu.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://uq.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vu.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://wh.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ni.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ag.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://qf.521024.cn

TS:   resp.ok;  resp.status
来源：http://fu.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://vf.nszjky.cn

Go:   resp.StatusCode
来源：http://rq.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://ub.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://yq.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://dg.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kq.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://kf.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mj.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bn.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pp.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vh.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kc.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jv.szsharing.cn

================================================================================
来源：http://od.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://cl.huixinmuqiang.cn

================================================================================
来源：http://mo.lnxyls.cn

[M01] 读取命令行参数
来源：http://tn.9csxet.cn

Py:   sys.argv[1:]
来源：http://gm.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://mu.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://xv.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://xw.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://ut.huanxung.cn

Go:   os.Args[1:]
来源：http://vz.panjiajie.cn

Ruby: ARGV
来源：http://pk.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://dz.muxihuayi.cn

[M02] 读取环境变量
来源：http://uf.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://mv.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cs.huanxung.cn

JS:   process.env.HOME
来源：http://bf.szsharing.cn

TS:   process.env.HOME
来源：http://sd.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://sj.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rs.9csxet.cn

Ruby: ENV["HOME"]
来源：http://gd.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gy.haigaiapp.cn

[M03] 执行外部命令
来源：http://ej.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wn.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://am.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fe.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://by.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ff.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jo.panjiajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ae.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://iu.shxzskj.cn

[M04] 获取当前工作目录
来源：http://ip.bookmarksfly.cn

Py:   os.getcwd()
来源：http://zg.newstarts.cn

PHP:  getcwd();
来源：http://fb.newstarts.cn

JS:   process.cwd()
来源：http://ef.nicolike.cn

TS:   process.cwd()
来源：http://bs.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://vt.9csxet.cn

Go:   os.Getwd()
来源：http://et.bjjhwx.cn

Ruby: Dir.pwd
来源：http://ya.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hs.shxzukj.cn

[M05] 设置退出码
来源：http://qq.chemitech.net.cn

Py:   sys.exit(1)
来源：http://ww.szsharing.cn

PHP:  exit(1);
来源：http://xl.lnxyls.cn

JS:   process.exit(1)
来源：http://or.chemitech.net.cn

TS:   process.exit(1)
来源：http://vj.chemitech.net.cn

Java: System.exit(1)
来源：http://uv.jctech888.com.cn

Go:   os.Exit(1)
来源：http://rq.shxzskj.cn

Ruby: exit 1
来源：http://qo.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vl.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://iq.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://gx.gzmigu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kg.9csxet.cn

JS:   console.error("err")
来源：http://el.haigaiapp.cn

TS:   console.error("err")
来源：http://uz.newstarts.cn

Java: System.err.println("err")
来源：http://zq.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wv.hnjuh.cn

Ruby: warn "err"
来源：http://ro.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://wj.newstarts.cn

[M07] 判断是否为主入口
来源：http://jr.colortex.cn

Py:   if __name__ == "__main__":
来源：http://ks.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lj.shxzukj.cn

JS:   require.main === module
来源：http://sk.jianghongdianzi.cn

TS:   require.main === module
来源：http://ak.nicolike.cn

Java: public static void main(String[] args)
来源：http://km.gzmigu.cn

Go:   func main()
来源：http://ah.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wi.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://cr.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://yr.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://ij.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://mp.hnjuh.cn

JS:   process.platform;  process.version
来源：http://tn.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://zx.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yx.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://iu.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uh.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://no.nicolike.cn

================================================================================
来源：http://yc.nicolike.cn

N. 数据结构与算法
来源：http://xy.bjjhwx.cn

================================================================================
来源：http://zh.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://uf.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yy.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fb.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cl.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rc.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ny.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://sv.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://du.521024.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gi.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://jk.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://pt.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ux.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://iu.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cx.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tb.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://oo.colortex.cn

Ruby: arr.sort
来源：http://sc.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cc.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://gw.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bi.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://ni.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fx.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vi.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://le.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ly.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://et.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fm.9csxet.cn

[N04] 斐波那契数列
来源：http://gp.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mv.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jq.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ad.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qr.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nu.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qf.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ap.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qm.chemitech.net.cn

[N05] 最大公约数
来源：http://ro.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://cm.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hu.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://be.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://si.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nh.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pg.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://cb.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ds.shxzskj.cn

[N06] 判断回文字符串
来源：http://mh.shxzskj.cn

Py:   s == s[::-1]
来源：http://ku.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://sw.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://oy.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://hp.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uz.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://ea.nicolike.cn


<!-- 参考信息 -->