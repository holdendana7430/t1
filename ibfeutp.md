代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://et.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fu.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tw.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wk.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mb.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xd.panjiajie.cn

[J09] 时区处理
来源：http://my.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ul.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wz.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oz.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mv.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ov.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dp.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://eo.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rs.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://vo.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tg.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://un.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dd.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pi.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dg.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kt.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cz.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hq.jctech888.com.cn

================================================================================
来源：http://tm.panjiajie.cn

K. JSON 与序列化
来源：http://dx.shxzskj.cn

================================================================================
来源：http://gz.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://az.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wb.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lz.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://ec.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://fa.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sf.szsharing.cn

Go:   json.Marshal(obj)
来源：http://py.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://er.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lx.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://xf.521024.cn

Py:   json.loads(s)
来源：http://bk.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ay.panjiajie.cn

JS:   JSON.parse(s)
来源：http://po.521024.cn

TS:   JSON.parse(s)
来源：http://em.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ec.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://fq.9csxet.cn

Ruby: JSON.parse(s)
来源：http://by.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wa.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://gn.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ca.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jx.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qm.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tn.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yi.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dj.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bj.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hc.huanxung.cn

[K04] 读取 JSON 文件
来源：http://jp.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qn.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zl.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ae.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xm.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gt.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://es.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sx.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://it.shxzukj.cn

[K05] 深拷贝对象
来源：http://wf.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://lr.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://ik.szsharing.cn

JS:   structuredClone(obj)
来源：http://mt.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://om.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hr.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iz.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vk.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pu.colortex.cn

[K06] 解析 URL 查询串
来源：http://vo.gzmigu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lg.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gu.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wt.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tk.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iu.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vy.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ks.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dn.521024.cn

[K07] 进制转换
来源：http://ox.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ho.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://en.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yh.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pl.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iz.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tp.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lg.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://si.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://vq.521024.cn

Py:   pickle.dumps(obj)
来源：http://xy.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vk.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://tg.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://it.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ly.asd995.cn

Go:   encoding/gob
来源：http://tn.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://co.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ga.wgjwhj.cn

================================================================================
来源：http://rs.9csxet.cn

L. 网络请求
来源：http://jj.asd995.cn

================================================================================
来源：http://mh.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://kg.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://db.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cm.nszjky.cn

JS:   await fetch(url)
来源：http://km.chemitech.net.cn

TS:   await fetch(url)
来源：http://mf.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kd.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://xo.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cs.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ml.szxytkj.cn

[L02] 发送 POST JSON
来源：http://sm.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tb.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://st.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://op.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hv.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://no.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ny.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vh.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ct.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://bi.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hv.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zm.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rg.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ey.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ey.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fz.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://om.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fa.colortex.cn

[L04] 设置超时
来源：http://tw.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://uc.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tl.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rj.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dd.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bs.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ms.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ux.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qh.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://tk.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zi.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nr.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sr.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kp.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zd.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://po.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vb.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kp.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://ks.huanxung.cn

Py:   resp.json()
来源：http://zz.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://uw.521024.cn

JS:   await resp.json()
来源：http://qd.gzmigu.cn

TS:   await resp.json()
来源：http://zw.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wo.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ud.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://dd.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fw.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://de.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yr.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tr.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://ux.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://xl.szsharing.cn

Java: resp.statusCode()
来源：http://dh.panjiajie.cn

Go:   resp.StatusCode
来源：http://vj.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://sd.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://lf.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://da.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mw.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://ip.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wv.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fh.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mh.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fd.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cs.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oe.huixinmuqiang.cn

================================================================================
来源：http://cl.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://pn.wgjwhj.cn

================================================================================
来源：http://fl.panjiajie.cn

[M01] 读取命令行参数
来源：http://uo.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://to.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://zk.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://ro.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://uo.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://ie.haigaiapp.cn

Go:   os.Args[1:]
来源：http://og.shxzukj.cn

Ruby: ARGV
来源：http://ft.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://st.shxzskj.cn

[M02] 读取环境变量
来源：http://ax.asd995.cn

Py:   os.environ.get("HOME")
来源：http://yp.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xm.hnjuh.cn

JS:   process.env.HOME
来源：http://zr.asd995.cn

TS:   process.env.HOME
来源：http://jk.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://ij.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://as.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://ff.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rb.hahajie.cn

[M03] 执行外部命令
来源：http://yg.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xj.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://op.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wi.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dy.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ty.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ht.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sf.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://tx.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://fy.muxihuayi.cn

Py:   os.getcwd()
来源：http://oa.nicolike.cn

PHP:  getcwd();
来源：http://sx.jianghongdianzi.cn

JS:   process.cwd()
来源：http://yz.bjjhwx.cn

TS:   process.cwd()
来源：http://tu.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://hu.bjjhwx.cn

Go:   os.Getwd()
来源：http://nd.huanxung.cn

Ruby: Dir.pwd
来源：http://aj.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wp.bjjhwx.cn

[M05] 设置退出码
来源：http://lc.haigaiapp.cn

Py:   sys.exit(1)
来源：http://nt.shxzukj.cn

PHP:  exit(1);
来源：http://xf.yuexingan06.cn

JS:   process.exit(1)
来源：http://ch.bjjhwx.cn

TS:   process.exit(1)
来源：http://nc.jctech888.com.cn

Java: System.exit(1)
来源：http://cn.huixiangedu.cn

Go:   os.Exit(1)
来源：http://ee.hahajie.cn

Ruby: exit 1
来源：http://xy.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gc.chemitech.net.cn

[M06] 向标准错误输出
来源：http://ex.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://ot.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sz.yuntaijiaju.cn

JS:   console.error("err")
来源：http://ws.szsharing.cn

TS:   console.error("err")
来源：http://fz.lnxyls.cn

Java: System.err.println("err")
来源：http://au.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://my.asd995.cn

Ruby: warn "err"
来源：http://jc.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://gd.szxytkj.cn

[M07] 判断是否为主入口
来源：http://gi.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://im.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nm.chemitech.net.cn

JS:   require.main === module
来源：http://tr.asd995.cn

TS:   require.main === module
来源：http://ay.huanxung.cn

Java: public static void main(String[] args)
来源：http://ab.nicolike.cn

Go:   func main()
来源：http://ys.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cc.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://az.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://dz.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://za.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://xg.gzmigu.cn

JS:   process.platform;  process.version
来源：http://ky.9csxet.cn

TS:   process.platform;  process.version
来源：http://pm.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cg.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nk.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sa.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uo.haigaiapp.cn

================================================================================
来源：http://ze.521024.cn

N. 数据结构与算法
来源：http://jp.yuexingan06.cn

================================================================================
来源：http://ei.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://yx.huixinmuqiang.cn

Py:   bisect.bisect_left(arr, x)
来源：http://di.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zy.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yb.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kr.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gi.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://ta.bjjhwx.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kd.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://iq.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://el.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://jl.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fi.wgjwhj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sy.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fp.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ev.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://cf.szxytkj.cn

Ruby: arr.sort
来源：http://gb.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sz.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://tv.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://su.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://ct.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ts.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://si.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lz.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tm.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tb.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mk.hnjuh.cn

[N04] 斐波那契数列
来源：http://fb.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mx.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oc.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mj.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yq.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gb.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oh.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ah.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eh.asd995.cn

[N05] 最大公约数
来源：http://at.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://ne.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dm.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sn.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dt.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ib.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yw.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://sz.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qx.szsharing.cn

[N06] 判断回文字符串
来源：http://ig.shxzskj.cn

Py:   s == s[::-1]
来源：http://lw.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://yn.shxzskj.cn


<!-- 参考信息 -->