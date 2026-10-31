代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fv.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ks.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://il.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iq.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tz.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oa.huanxung.cn

[J09] 时区处理
来源：http://ca.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qj.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tb.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bq.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jo.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ob.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ha.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mq.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uq.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://nj.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ar.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xe.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hu.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zg.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ka.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oc.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ad.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://va.jctech888.com.cn

================================================================================
来源：http://jx.szsharing.cn

K. JSON 与序列化
来源：http://qu.yuexingan06.cn

================================================================================
来源：http://wq.521024.cn

[K01] 对象转 JSON 字符串
来源：http://cm.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kq.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kn.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://qf.asd995.cn

TS:   JSON.stringify(obj)
来源：http://fn.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gb.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://ai.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jb.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ht.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://cx.shtwfgs.cn

Py:   json.loads(s)
来源：http://sa.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nq.asd995.cn

JS:   JSON.parse(s)
来源：http://xe.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://pg.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uq.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://pf.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://pt.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sh.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://rr.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dn.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ns.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jc.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ds.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://st.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ug.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bb.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gr.9csxet.cn

[K04] 读取 JSON 文件
来源：http://mi.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fo.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ab.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mj.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tc.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vg.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mo.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xk.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kt.gzmigu.cn

[K05] 深拷贝对象
来源：http://fb.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://mg.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://mu.9csxet.cn

JS:   structuredClone(obj)
来源：http://ze.shxzukj.cn

TS:   structuredClone(obj)
来源：http://hc.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://an.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hm.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eh.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hn.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://jk.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ra.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zj.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eb.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://of.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mh.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zl.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hv.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xw.9csxet.cn

[K07] 进制转换
来源：http://uu.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wl.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wd.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ci.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wt.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wm.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eo.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hj.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qy.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://zv.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://jr.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pg.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://tr.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://fs.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ur.jctech888.com.cn

Go:   encoding/gob
来源：http://xw.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://xz.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://em.bjjhwx.cn

================================================================================
来源：http://fi.newstarts.cn

L. 网络请求
来源：http://mw.shxzukj.cn

================================================================================
来源：http://eb.521024.cn

[L01] 发送 GET 请求
来源：http://dp.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vk.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tn.9csxet.cn

JS:   await fetch(url)
来源：http://mj.nszjky.cn

TS:   await fetch(url)
来源：http://wb.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qd.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://hb.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pu.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lu.nicolike.cn

[L02] 发送 POST JSON
来源：http://ii.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zy.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ne.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ua.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sq.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sx.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ee.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xa.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tt.nicolike.cn

[L03] 设置自定义请求头
来源：http://ci.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mn.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pj.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://to.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ns.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dx.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ed.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rs.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nl.9csxet.cn

[L04] 设置超时
来源：http://rc.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://aa.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wq.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dz.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xa.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yk.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zb.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oq.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dl.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://zv.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yf.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zw.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mq.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hl.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ih.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eq.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gl.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rg.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://fy.wgjwhj.cn

Py:   resp.json()
来源：http://ed.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://qn.gzmigu.cn

JS:   await resp.json()
来源：http://qk.bjjhwx.cn

TS:   await resp.json()
来源：http://gs.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ww.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mk.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://ng.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ex.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://pi.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mx.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hc.521024.cn

JS:   resp.ok;  resp.status
来源：http://ce.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://yv.521024.cn

Java: resp.statusCode()
来源：http://ef.huixiangedu.cn

Go:   resp.StatusCode
来源：http://iv.huanxung.cn

Ruby: resp.code.to_i
来源：http://kd.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://bw.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://nm.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tz.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://qd.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rp.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kc.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ri.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xz.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xt.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xn.nszjky.cn

================================================================================
来源：http://lm.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://ym.gzmigu.cn

================================================================================
来源：http://zv.jctech888.com.cn

[M01] 读取命令行参数
来源：http://dt.shxzskj.cn

Py:   sys.argv[1:]
来源：http://ff.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://gr.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://xm.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://cb.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://xy.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://po.colortex.cn

Ruby: ARGV
来源：http://gu.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://sm.asd995.cn

[M02] 读取环境变量
来源：http://mx.521024.cn

Py:   os.environ.get("HOME")
来源：http://oh.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zm.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://ur.muxihuayi.cn

TS:   process.env.HOME
来源：http://tp.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://le.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tw.muxihuayi.cn

Ruby: ENV["HOME"]
来源：http://vf.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uc.colortex.cn

[M03] 执行外部命令
来源：http://ed.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mp.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yp.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zi.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ew.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gj.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ok.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nk.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://gv.szsharing.cn

[M04] 获取当前工作目录
来源：http://km.bjjhwx.cn

Py:   os.getcwd()
来源：http://nz.shxzskj.cn

PHP:  getcwd();
来源：http://ks.hnjuh.cn

JS:   process.cwd()
来源：http://xd.szxytkj.cn

TS:   process.cwd()
来源：http://pk.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://qm.shxzukj.cn

Go:   os.Getwd()
来源：http://qr.huixiangedu.cn

Ruby: Dir.pwd
来源：http://xo.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vi.yuexingan06.cn

[M05] 设置退出码
来源：http://qp.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://qh.jctech888.com.cn

PHP:  exit(1);
来源：http://ci.asd995.cn

JS:   process.exit(1)
来源：http://mf.nicolike.cn

TS:   process.exit(1)
来源：http://cn.huixiangedu.cn

Java: System.exit(1)
来源：http://mp.yuexingan06.cn

Go:   os.Exit(1)
来源：http://sn.newstarts.cn

Ruby: exit 1
来源：http://ju.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sg.shxzukj.cn

[M06] 向标准错误输出
来源：http://vk.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://kf.gzmigu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://al.asd995.cn

JS:   console.error("err")
来源：http://bd.nszjky.cn

TS:   console.error("err")
来源：http://ad.haigaiapp.cn

Java: System.err.println("err")
来源：http://kq.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bl.panjiajie.cn

Ruby: warn "err"
来源：http://ui.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://qv.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://dr.panjiajie.cn

Py:   if __name__ == "__main__":
来源：http://xo.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ui.huixinmuqiang.cn

JS:   require.main === module
来源：http://eo.jctech888.com.cn

TS:   require.main === module
来源：http://xo.nicolike.cn

Java: public static void main(String[] args)
来源：http://up.shxzskj.cn

Go:   func main()
来源：http://xa.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yq.nicolike.cn

C#:   static void Main(string[] args)
来源：http://hh.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://iq.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://ql.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://gx.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://nw.newstarts.cn

TS:   process.platform;  process.version
来源：http://ld.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ys.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gj.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ds.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qz.bjjhwx.cn

================================================================================
来源：http://rw.yuntaijiaju.cn

N. 数据结构与算法
来源：http://wb.colortex.cn

================================================================================
来源：http://el.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://nc.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cp.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jq.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bs.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ms.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tl.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://zn.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://eu.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xk.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://ta.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://qr.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://op.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://un.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vy.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gz.nicolike.cn

Go:   slices.Sort(arr)
来源：http://mh.jianghongdianzi.cn

Ruby: arr.sort
来源：http://on.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oa.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://jt.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uz.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://gj.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ih.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vo.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lr.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ln.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://an.nicolike.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tg.szsharing.cn

[N04] 斐波那契数列
来源：http://xe.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fx.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qk.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ln.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wr.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gd.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yy.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xn.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jd.yuntaijiaju.cn

[N05] 最大公约数
来源：http://kh.521024.cn

Py:   math.gcd(a, b)
来源：http://uf.panjiajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vv.wgjwhj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pn.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pm.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jx.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://st.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://ul.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bq.nszjky.cn

[N06] 判断回文字符串
来源：http://ag.yuexingan06.cn

Py:   s == s[::-1]
来源：http://fr.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://oh.huixinmuqiang.cn


<!-- 参考信息 -->