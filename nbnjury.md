代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zi.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jr.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gh.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://np.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ik.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ae.bookmarksfly.cn

[J09] 时区处理
来源：http://tp.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sl.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wz.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://be.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fp.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fe.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jc.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ng.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tb.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://cy.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://au.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lk.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lh.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ts.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hc.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tv.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nl.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://be.nicolike.cn

================================================================================
来源：http://pt.nicolike.cn

K. JSON 与序列化
来源：http://uy.asd995.cn

================================================================================
来源：http://tu.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://tn.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nt.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nb.asd995.cn

JS:   JSON.stringify(obj)
来源：http://gz.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://pa.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ey.521024.cn

Go:   json.Marshal(obj)
来源：http://zl.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xf.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://by.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://nr.hnjuh.cn

Py:   json.loads(s)
来源：http://gg.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aj.colortex.cn

JS:   JSON.parse(s)
来源：http://iy.nszjky.cn

TS:   JSON.parse(s)
来源：http://bf.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://in.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://el.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://zh.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wd.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://ha.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bo.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ch.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vw.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nl.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ta.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fj.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nk.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://in.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://iq.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pn.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ra.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://la.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hm.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eb.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ky.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://no.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://al.gzmigu.cn

[K05] 深拷贝对象
来源：http://ur.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://ze.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://fs.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://sl.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://xr.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://be.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oa.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gq.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kj.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://hs.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iq.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dw.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ij.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kx.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fn.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vv.huixiangedu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xt.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bk.hnjuh.cn

[K07] 进制转换
来源：http://xk.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cz.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://az.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jd.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xw.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zd.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zb.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ht.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tf.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://xy.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://ak.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://aa.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://gr.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://tn.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://so.yuexingan06.cn

Go:   encoding/gob
来源：http://pl.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://gu.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mg.9csxet.cn

================================================================================
来源：http://ao.gzmigu.cn

L. 网络请求
来源：http://uf.shtwfgs.cn

================================================================================
来源：http://hk.hahajie.cn

[L01] 发送 GET 请求
来源：http://kp.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gy.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fg.jctech888.com.cn

JS:   await fetch(url)
来源：http://mv.szsharing.cn

TS:   await fetch(url)
来源：http://ea.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vt.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://wb.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qb.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dk.colortex.cn

[L02] 发送 POST JSON
来源：http://qk.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cx.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iz.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xz.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hb.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wd.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ud.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rw.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kr.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://gk.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ut.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tb.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cf.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://am.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ad.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tm.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ay.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nd.huanxung.cn

[L04] 设置超时
来源：http://xj.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://nq.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gc.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://su.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fh.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ur.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tj.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cy.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://po.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://ao.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ff.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mf.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rp.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ss.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qx.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eq.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cr.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wx.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://kn.hahajie.cn

Py:   resp.json()
来源：http://vb.nszjky.cn

PHP:  json_decode($body, true);
来源：http://te.yuexingan06.cn

JS:   await resp.json()
来源：http://co.yuntaijiaju.cn

TS:   await resp.json()
来源：http://ut.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xx.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nh.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://jj.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ox.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://gf.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ip.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ih.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://nr.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://qg.panjiajie.cn

Java: resp.statusCode()
来源：http://ny.bjjhwx.cn

Go:   resp.StatusCode
来源：http://al.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://yi.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://if.9csxet.cn

[L08] 并发请求多个地址
来源：http://dp.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hb.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://ys.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qd.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ak.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uo.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ny.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aa.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wn.szxytkj.cn

================================================================================
来源：http://iu.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://mo.huanxung.cn

================================================================================
来源：http://qv.521024.cn

[M01] 读取命令行参数
来源：http://ls.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://th.asd995.cn

PHP:  $argv;  $argc;
来源：http://hu.nszjky.cn

JS:   process.argv.slice(2)
来源：http://xc.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://uu.asd995.cn

Java: args 数组（main 方法参数）
来源：http://qg.muxihuayi.cn

Go:   os.Args[1:]
来源：http://rq.nszjky.cn

Ruby: ARGV
来源：http://zy.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://fd.521024.cn

[M02] 读取环境变量
来源：http://pj.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://pu.bookmarksfly.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ew.huixiangedu.cn

JS:   process.env.HOME
来源：http://bq.jctech888.com.cn

TS:   process.env.HOME
来源：http://cw.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://gi.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jt.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://nt.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ii.asd995.cn

[M03] 执行外部命令
来源：http://eq.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vi.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bo.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ho.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ge.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pn.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cu.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xm.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://kt.newstarts.cn

[M04] 获取当前工作目录
来源：http://em.lnxyls.cn

Py:   os.getcwd()
来源：http://ra.muxihuayi.cn

PHP:  getcwd();
来源：http://ze.jianghongdianzi.cn

JS:   process.cwd()
来源：http://zd.lnxyls.cn

TS:   process.cwd()
来源：http://jt.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://wf.muxihuayi.cn

Go:   os.Getwd()
来源：http://nf.muxihuayi.cn

Ruby: Dir.pwd
来源：http://mr.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jo.panjiajie.cn

[M05] 设置退出码
来源：http://jn.chemitech.net.cn

Py:   sys.exit(1)
来源：http://ac.asd995.cn

PHP:  exit(1);
来源：http://ki.wgjwhj.cn

JS:   process.exit(1)
来源：http://eg.yuexingan06.cn

TS:   process.exit(1)
来源：http://tc.shtwfgs.cn

Java: System.exit(1)
来源：http://rc.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://vc.hahajie.cn

Ruby: exit 1
来源：http://bf.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vp.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://is.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://ao.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ef.muxihuayi.cn

JS:   console.error("err")
来源：http://iv.jianghongdianzi.cn

TS:   console.error("err")
来源：http://um.shxzukj.cn

Java: System.err.println("err")
来源：http://tb.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://le.newstarts.cn

Ruby: warn "err"
来源：http://st.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://bm.szxytkj.cn

[M07] 判断是否为主入口
来源：http://ju.colortex.cn

Py:   if __name__ == "__main__":
来源：http://in.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ih.szxytkj.cn

JS:   require.main === module
来源：http://xf.shxzukj.cn

TS:   require.main === module
来源：http://zs.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://iv.shxzukj.cn

Go:   func main()
来源：http://zb.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vy.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://dq.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://id.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://uu.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://up.wgjwhj.cn

JS:   process.platform;  process.version
来源：http://hg.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://gr.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gr.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gk.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tb.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bq.yuntaijiaju.cn

================================================================================
来源：http://ey.huixiangedu.cn

N. 数据结构与算法
来源：http://pw.yuntaijiaju.cn

================================================================================
来源：http://or.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://rv.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ee.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mo.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lk.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bg.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://js.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://gs.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jj.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zq.huixinmuqiang.cn

[N02] 排序（工程实践用内置实现）
来源：http://of.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://ym.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xh.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sz.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fi.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ng.huanxung.cn

Go:   slices.Sort(arr)
来源：http://ne.wgjwhj.cn

Ruby: arr.sort
来源：http://he.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zx.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://va.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ii.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://ls.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oo.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tj.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ii.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://so.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ix.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ci.shxzskj.cn

[N04] 斐波那契数列
来源：http://gg.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ss.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bw.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fn.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iw.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://co.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rn.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jg.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rv.yuntaijiaju.cn

[N05] 最大公约数
来源：http://vu.nszjky.cn

Py:   math.gcd(a, b)
来源：http://bn.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aq.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ya.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wi.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mv.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://ci.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ja.hahajie.cn

[N06] 判断回文字符串
来源：http://os.newstarts.cn

Py:   s == s[::-1]
来源：http://mm.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://bd.bjjhwx.cn


<!-- 参考信息 -->