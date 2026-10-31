代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vf.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uo.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hi.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://er.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pt.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xt.szsharing.cn

[J09] 时区处理
来源：http://yi.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ku.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kj.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tj.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rz.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wf.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vq.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sn.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://la.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://qt.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ms.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jm.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vf.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ah.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ef.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wy.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jq.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jt.huixiangedu.cn

================================================================================
来源：http://oh.shxzukj.cn

K. JSON 与序列化
来源：http://ro.bjjhwx.cn

================================================================================
来源：http://hb.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://wo.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vy.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sa.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://nx.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://aj.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ot.newstarts.cn

Go:   json.Marshal(obj)
来源：http://qm.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ag.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pp.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://ad.chemitech.net.cn

Py:   json.loads(s)
来源：http://uq.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yv.panjiajie.cn

JS:   JSON.parse(s)
来源：http://iv.lnxyls.cn

TS:   JSON.parse(s)
来源：http://zb.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://am.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://wm.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://qn.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wm.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://vn.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jl.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hx.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ea.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ot.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xz.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ag.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rn.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aa.szsharing.cn

[K04] 读取 JSON 文件
来源：http://vq.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wo.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dh.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ie.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lf.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qw.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sz.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zk.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bw.jctech888.com.cn

[K05] 深拷贝对象
来源：http://nh.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://rt.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://wz.nszjky.cn

JS:   structuredClone(obj)
来源：http://wn.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://ap.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lv.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mi.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nu.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xt.szsharing.cn

[K06] 解析 URL 查询串
来源：http://hu.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pe.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wm.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xd.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yb.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mp.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yz.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gx.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tk.colortex.cn

[K07] 进制转换
来源：http://tb.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mn.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ss.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fa.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://em.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vz.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gt.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pd.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hc.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ih.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://zb.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://je.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://ij.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://pl.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wz.huixinmuqiang.cn

Go:   encoding/gob
来源：http://zu.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://aw.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dx.yuexingan06.cn

================================================================================
来源：http://xo.asd995.cn

L. 网络请求
来源：http://ba.lnxyls.cn

================================================================================
来源：http://js.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://tc.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://af.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ug.chemitech.net.cn

JS:   await fetch(url)
来源：http://bu.wgjwhj.cn

TS:   await fetch(url)
来源：http://ex.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aq.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://rm.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gu.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vk.newstarts.cn

[L02] 发送 POST JSON
来源：http://ju.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yj.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ln.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rc.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ng.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://te.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kn.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gq.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tz.colortex.cn

[L03] 设置自定义请求头
来源：http://uo.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yg.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://so.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gv.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nk.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tg.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oy.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sx.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fy.huixinmuqiang.cn

[L04] 设置超时
来源：http://ya.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://dn.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://up.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://db.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qg.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mk.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xh.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bo.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://to.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://gh.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kd.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://px.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lh.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bv.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ak.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ex.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vr.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sp.asd995.cn

[L06] 解析响应为 JSON
来源：http://so.hahajie.cn

Py:   resp.json()
来源：http://wt.colortex.cn

PHP:  json_decode($body, true);
来源：http://td.jctech888.com.cn

JS:   await resp.json()
来源：http://mj.chemitech.net.cn

TS:   await resp.json()
来源：http://cg.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uc.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hb.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://mf.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gc.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://jn.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fa.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rx.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://cs.521024.cn

TS:   resp.ok;  resp.status
来源：http://lw.yuexingan06.cn

Java: resp.statusCode()
来源：http://nf.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://co.521024.cn

Ruby: resp.code.to_i
来源：http://cq.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://fl.lnxyls.cn

[L08] 并发请求多个地址
来源：http://vv.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ky.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://fa.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rj.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bi.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://so.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ju.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xy.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xd.shtwfgs.cn

================================================================================
来源：http://vv.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://xq.nszjky.cn

================================================================================
来源：http://ar.newstarts.cn

[M01] 读取命令行参数
来源：http://tu.521024.cn

Py:   sys.argv[1:]
来源：http://nr.hnjuh.cn

PHP:  $argv;  $argc;
来源：http://cn.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://eq.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://mi.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://og.huanxung.cn

Go:   os.Args[1:]
来源：http://gf.chemitech.net.cn

Ruby: ARGV
来源：http://qd.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://ev.lnxyls.cn

[M02] 读取环境变量
来源：http://ee.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://ny.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lt.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://pp.shxzukj.cn

TS:   process.env.HOME
来源：http://gy.szsharing.cn

Java: System.getenv("HOME")
来源：http://du.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://an.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://hu.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nh.wgjwhj.cn

[M03] 执行外部命令
来源：http://fr.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ca.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tr.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qk.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pu.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bk.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lh.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qr.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://pz.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://vk.muxihuayi.cn

Py:   os.getcwd()
来源：http://dx.hnjuh.cn

PHP:  getcwd();
来源：http://zb.muxihuayi.cn

JS:   process.cwd()
来源：http://il.jctech888.com.cn

TS:   process.cwd()
来源：http://qy.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://ge.newstarts.cn

Go:   os.Getwd()
来源：http://xi.nicolike.cn

Ruby: Dir.pwd
来源：http://di.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sl.chemitech.net.cn

[M05] 设置退出码
来源：http://af.muxihuayi.cn

Py:   sys.exit(1)
来源：http://nm.asd995.cn

PHP:  exit(1);
来源：http://dk.huanxung.cn

JS:   process.exit(1)
来源：http://eb.colortex.cn

TS:   process.exit(1)
来源：http://jh.jctech888.com.cn

Java: System.exit(1)
来源：http://fd.nszjky.cn

Go:   os.Exit(1)
来源：http://ck.panjiajie.cn

Ruby: exit 1
来源：http://ru.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rz.nszjky.cn

[M06] 向标准错误输出
来源：http://ny.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://qt.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vp.wgjwhj.cn

JS:   console.error("err")
来源：http://ik.nszjky.cn

TS:   console.error("err")
来源：http://df.szsharing.cn

Java: System.err.println("err")
来源：http://fo.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rh.shxzskj.cn

Ruby: warn "err"
来源：http://zi.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://lw.hnjuh.cn

[M07] 判断是否为主入口
来源：http://si.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://nl.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://di.newstarts.cn

JS:   require.main === module
来源：http://ah.szxytkj.cn

TS:   require.main === module
来源：http://xi.panjiajie.cn

Java: public static void main(String[] args)
来源：http://ez.shtwfgs.cn

Go:   func main()
来源：http://ir.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yo.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://em.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://jy.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://tg.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://pl.panjiajie.cn

JS:   process.platform;  process.version
来源：http://wo.szsharing.cn

TS:   process.platform;  process.version
来源：http://dt.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vz.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vv.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bz.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tk.huixinmuqiang.cn

================================================================================
来源：http://kp.hahajie.cn

N. 数据结构与算法
来源：http://bd.szsharing.cn

================================================================================
来源：http://ri.asd995.cn

[N01] 二分查找（有序数组）
来源：http://uv.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://do.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ad.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gn.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wq.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tu.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://kw.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xs.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sr.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://vt.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://vg.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tq.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fz.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://up.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://np.nicolike.cn

Go:   slices.Sort(arr)
来源：http://wx.chemitech.net.cn

Ruby: arr.sort
来源：http://vj.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jk.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://vc.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bo.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://xc.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ue.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://in.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bu.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gd.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jx.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://li.521024.cn

[N04] 斐波那契数列
来源：http://um.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ye.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sn.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hf.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ru.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ks.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fu.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iv.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ou.lnxyls.cn

[N05] 最大公约数
来源：http://ik.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://lm.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fr.colortex.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cp.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uu.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mk.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ep.nszjky.cn

Ruby: a.gcd(b)
来源：http://hh.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pa.chemitech.net.cn

[N06] 判断回文字符串
来源：http://cq.shtwfgs.cn

Py:   s == s[::-1]
来源：http://zg.huanxung.cn

PHP:  $s === strrev($s);
来源：http://zx.9csxet.cn


<!-- 参考信息 -->