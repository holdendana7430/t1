代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ew.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cu.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ud.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rz.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qm.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uu.nicolike.cn

[J09] 时区处理
来源：http://jm.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ph.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ld.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xa.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sh.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lz.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://go.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://me.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cb.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://zr.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hw.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ec.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yx.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://as.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ay.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hk.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iv.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://os.shxzskj.cn

================================================================================
来源：http://fv.hahajie.cn

K. JSON 与序列化
来源：http://xa.panjiajie.cn

================================================================================
来源：http://ad.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://dp.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rm.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qh.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://jn.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://tj.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ic.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://rn.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yw.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pc.szsharing.cn

[K02] JSON 字符串转对象
来源：http://ab.shxzskj.cn

Py:   json.loads(s)
来源：http://it.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://er.newstarts.cn

JS:   JSON.parse(s)
来源：http://sf.9csxet.cn

TS:   JSON.parse(s)
来源：http://ec.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://da.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://mg.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://cw.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mw.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://xu.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qv.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qj.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xr.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gj.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ps.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qo.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jc.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yd.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://sa.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://if.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gr.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uu.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yw.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wq.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rx.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://py.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ci.9csxet.cn

[K05] 深拷贝对象
来源：http://mk.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://hk.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://an.nicolike.cn

JS:   structuredClone(obj)
来源：http://ht.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://jp.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ba.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ys.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cz.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ai.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://km.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zk.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wb.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ty.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lq.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kb.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fe.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://no.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://du.colortex.cn

[K07] 进制转换
来源：http://pj.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ka.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ap.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ma.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jd.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gl.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ub.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bo.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cc.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://nx.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://wq.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rr.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://lw.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://ya.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jz.521024.cn

Go:   encoding/gob
来源：http://jb.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://cn.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jx.hahajie.cn

================================================================================
来源：http://yg.jctech888.com.cn

L. 网络请求
来源：http://dh.gzmigu.cn

================================================================================
来源：http://gy.huanxung.cn

[L01] 发送 GET 请求
来源：http://be.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ec.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nc.9csxet.cn

JS:   await fetch(url)
来源：http://kt.muxihuayi.cn

TS:   await fetch(url)
来源：http://nv.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pg.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://fo.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bg.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ap.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://sb.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dh.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eo.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ii.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sp.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ph.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rt.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hw.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vy.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://cl.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rr.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xv.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lz.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wj.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lc.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tf.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ad.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ks.huanxung.cn

[L04] 设置超时
来源：http://ph.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://wj.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qc.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vd.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sj.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yj.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ys.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ne.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zf.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://ao.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yo.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ll.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hf.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hj.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://do.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vq.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gc.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xb.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://oi.panjiajie.cn

Py:   resp.json()
来源：http://wn.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://eg.lnxyls.cn

JS:   await resp.json()
来源：http://jo.hnjuh.cn

TS:   await resp.json()
来源：http://my.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oz.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ef.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://qr.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sw.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://bg.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sw.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xp.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://bi.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://jw.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://cw.huixiangedu.cn

Go:   resp.StatusCode
来源：http://br.huanxung.cn

Ruby: resp.code.to_i
来源：http://hh.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://lv.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://ia.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uy.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://cp.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ch.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rd.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://or.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pj.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dd.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bb.colortex.cn

================================================================================
来源：http://gw.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://zx.hnjuh.cn

================================================================================
来源：http://bd.asd995.cn

[M01] 读取命令行参数
来源：http://fr.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://bo.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://mu.newstarts.cn

JS:   process.argv.slice(2)
来源：http://vx.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://qt.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://nd.gzmigu.cn

Go:   os.Args[1:]
来源：http://lj.jianghongdianzi.cn

Ruby: ARGV
来源：http://gh.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://ln.bjjhwx.cn

[M02] 读取环境变量
来源：http://ej.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://ml.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ol.szsharing.cn

JS:   process.env.HOME
来源：http://xb.gzmigu.cn

TS:   process.env.HOME
来源：http://oz.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://qo.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yg.colortex.cn

Ruby: ENV["HOME"]
来源：http://yu.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iy.haigaiapp.cn

[M03] 执行外部命令
来源：http://yn.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://db.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ne.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wa.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xq.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://op.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vq.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sq.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://ke.shxzskj.cn

[M04] 获取当前工作目录
来源：http://sw.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://sr.hahajie.cn

PHP:  getcwd();
来源：http://fr.hahajie.cn

JS:   process.cwd()
来源：http://co.colortex.cn

TS:   process.cwd()
来源：http://tg.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://mp.muxihuayi.cn

Go:   os.Getwd()
来源：http://ww.9csxet.cn

Ruby: Dir.pwd
来源：http://mc.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wg.jctech888.com.cn

[M05] 设置退出码
来源：http://cx.lnxyls.cn

Py:   sys.exit(1)
来源：http://jk.hnjuh.cn

PHP:  exit(1);
来源：http://tc.muxihuayi.cn

JS:   process.exit(1)
来源：http://js.shtwfgs.cn

TS:   process.exit(1)
来源：http://ts.bookmarksfly.cn

Java: System.exit(1)
来源：http://sd.szsharing.cn

Go:   os.Exit(1)
来源：http://uw.shxzukj.cn

Ruby: exit 1
来源：http://sg.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rt.jctech888.com.cn

[M06] 向标准错误输出
来源：http://co.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://mi.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tz.colortex.cn

JS:   console.error("err")
来源：http://hw.asd995.cn

TS:   console.error("err")
来源：http://cv.hahajie.cn

Java: System.err.println("err")
来源：http://vi.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yw.gzmigu.cn

Ruby: warn "err"
来源：http://mg.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://rg.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://ob.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://oh.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gu.huixinmuqiang.cn

JS:   require.main === module
来源：http://uj.muxihuayi.cn

TS:   require.main === module
来源：http://hz.huanxung.cn

Java: public static void main(String[] args)
来源：http://iq.gzmigu.cn

Go:   func main()
来源：http://sk.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iw.nicolike.cn

C#:   static void Main(string[] args)
来源：http://ce.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://rg.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://bu.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://gl.lnxyls.cn

JS:   process.platform;  process.version
来源：http://jd.asd995.cn

TS:   process.platform;  process.version
来源：http://do.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lm.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ya.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ee.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://th.panjiajie.cn

================================================================================
来源：http://pr.szsharing.cn

N. 数据结构与算法
来源：http://ud.muxihuayi.cn

================================================================================
来源：http://xt.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://oi.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wl.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hs.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ix.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qg.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://km.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://va.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tz.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rs.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://qf.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://vs.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ov.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nn.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://in.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cc.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://ip.hnjuh.cn

Ruby: arr.sort
来源：http://wm.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gj.521024.cn

[N03] 快速排序（分治示例）
来源：http://qa.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lg.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://ny.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xs.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ov.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zl.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qs.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cx.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pz.9csxet.cn

[N04] 斐波那契数列
来源：http://dp.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gl.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rw.yuexingan06.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ux.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gb.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ti.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xn.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xx.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eg.szsharing.cn

[N05] 最大公约数
来源：http://qi.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://ti.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://if.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mz.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kz.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gx.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cf.panjiajie.cn

Ruby: a.gcd(b)
来源：http://ij.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lz.huanxung.cn

[N06] 判断回文字符串
来源：http://gy.colortex.cn

Py:   s == s[::-1]
来源：http://fh.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://sb.hnjuh.cn


<!-- 参考信息 -->