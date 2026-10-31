代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://oe.szsharing.cn

[J08] 提取年月日与星期
来源：http://qu.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fu.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dz.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ir.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dz.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nx.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lq.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ov.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://it.nszjky.cn

[J09] 时区处理
来源：http://va.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sz.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zj.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hb.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xg.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yo.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ft.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zq.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cg.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://jt.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nx.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ij.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xf.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://io.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mm.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gz.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vy.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ce.521024.cn

================================================================================
来源：http://op.nicolike.cn

K. JSON 与序列化
来源：http://uj.asd995.cn

================================================================================
来源：http://gt.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://bm.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kc.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rv.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://mn.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://yl.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lo.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://dr.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qf.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kr.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://rx.9csxet.cn

Py:   json.loads(s)
来源：http://rg.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tg.szxytkj.cn

JS:   JSON.parse(s)
来源：http://af.9csxet.cn

TS:   JSON.parse(s)
来源：http://du.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wi.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://in.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://sj.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nk.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://pc.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jd.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ci.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://eb.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gs.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qc.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xe.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ry.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jk.asd995.cn

[K04] 读取 JSON 文件
来源：http://kq.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nl.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fi.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://su.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yt.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zl.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rl.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://es.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ca.yuexingan06.cn

[K05] 深拷贝对象
来源：http://rr.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://hi.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://vh.szxytkj.cn

JS:   structuredClone(obj)
来源：http://jf.gzmigu.cn

TS:   structuredClone(obj)
来源：http://nz.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mj.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xi.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ng.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xz.9csxet.cn

[K06] 解析 URL 查询串
来源：http://vt.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sx.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://im.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ue.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xq.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hd.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ls.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xe.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dj.huanxung.cn

[K07] 进制转换
来源：http://dr.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fl.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yt.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ag.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yy.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oz.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ow.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tw.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://co.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://rs.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://ro.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pk.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://hd.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://xg.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://er.bjjhwx.cn

Go:   encoding/gob
来源：http://zf.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://rr.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cm.hahajie.cn

================================================================================
来源：http://ox.newstarts.cn

L. 网络请求
来源：http://fb.newstarts.cn

================================================================================
来源：http://np.newstarts.cn

[L01] 发送 GET 请求
来源：http://hg.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dk.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jt.newstarts.cn

JS:   await fetch(url)
来源：http://dn.panjiajie.cn

TS:   await fetch(url)
来源：http://xw.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uk.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://nj.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bp.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fy.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://dq.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://od.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bo.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vn.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ox.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zw.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hy.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pn.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ak.shxzskj.cn

[L03] 设置自定义请求头
来源：http://um.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qm.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bn.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iy.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ag.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://js.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lk.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vk.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://od.panjiajie.cn

[L04] 设置超时
来源：http://gc.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://mo.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://up.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cx.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xh.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oq.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ph.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ik.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uh.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://ap.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vy.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fd.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eb.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gm.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qo.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uc.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lt.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rz.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://xe.bookmarksfly.cn

Py:   resp.json()
来源：http://ny.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://jw.bookmarksfly.cn

JS:   await resp.json()
来源：http://zk.bookmarksfly.cn

TS:   await resp.json()
来源：http://nz.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://se.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ni.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://km.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yo.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://ig.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jv.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zo.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://mb.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://kt.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://da.9csxet.cn

Go:   resp.StatusCode
来源：http://im.panjiajie.cn

Ruby: resp.code.to_i
来源：http://ln.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://pb.9csxet.cn

[L08] 并发请求多个地址
来源：http://sl.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://em.521024.cn

PHP:  curl_multi_init() 系列
来源：http://ju.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zy.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vf.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tf.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ll.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wl.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nh.hnjuh.cn

================================================================================
来源：http://yf.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://rb.9csxet.cn

================================================================================
来源：http://hj.chemitech.net.cn

[M01] 读取命令行参数
来源：http://rh.szsharing.cn

Py:   sys.argv[1:]
来源：http://dp.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://ra.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://ax.nszjky.cn

TS:   process.argv.slice(2)
来源：http://zq.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://il.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://ch.haigaiapp.cn

Ruby: ARGV
来源：http://kl.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://ic.panjiajie.cn

[M02] 读取环境变量
来源：http://sq.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://mi.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dp.muxihuayi.cn

JS:   process.env.HOME
来源：http://gf.szsharing.cn

TS:   process.env.HOME
来源：http://yh.newstarts.cn

Java: System.getenv("HOME")
来源：http://lj.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ne.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://jy.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tv.muxihuayi.cn

[M03] 执行外部命令
来源：http://ez.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hk.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mw.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rj.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vw.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hp.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cz.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gk.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://rb.panjiajie.cn

[M04] 获取当前工作目录
来源：http://hw.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://dq.bookmarksfly.cn

PHP:  getcwd();
来源：http://ck.bjjhwx.cn

JS:   process.cwd()
来源：http://zn.nicolike.cn

TS:   process.cwd()
来源：http://sb.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://to.haigaiapp.cn

Go:   os.Getwd()
来源：http://xm.521024.cn

Ruby: Dir.pwd
来源：http://bw.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nd.shtwfgs.cn

[M05] 设置退出码
来源：http://ub.hnjuh.cn

Py:   sys.exit(1)
来源：http://ug.hnjuh.cn

PHP:  exit(1);
来源：http://nc.shxzskj.cn

JS:   process.exit(1)
来源：http://rl.colortex.cn

TS:   process.exit(1)
来源：http://eq.huixinmuqiang.cn

Java: System.exit(1)
来源：http://nm.muxihuayi.cn

Go:   os.Exit(1)
来源：http://eu.shxzukj.cn

Ruby: exit 1
来源：http://jn.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iv.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://sl.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://xf.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bv.nicolike.cn

JS:   console.error("err")
来源：http://gc.colortex.cn

TS:   console.error("err")
来源：http://ta.yuexingan06.cn

Java: System.err.println("err")
来源：http://jy.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ag.bjjhwx.cn

Ruby: warn "err"
来源：http://kd.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://dt.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://fy.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://au.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uu.szxytkj.cn

JS:   require.main === module
来源：http://tc.jianghongdianzi.cn

TS:   require.main === module
来源：http://ss.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://lv.lnxyls.cn

Go:   func main()
来源：http://tw.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mg.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://uw.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://qm.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://cs.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://xh.521024.cn

JS:   process.platform;  process.version
来源：http://gt.szsharing.cn

TS:   process.platform;  process.version
来源：http://to.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yk.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vo.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fi.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jb.gzmigu.cn

================================================================================
来源：http://vf.muxihuayi.cn

N. 数据结构与算法
来源：http://iz.shtwfgs.cn

================================================================================
来源：http://vb.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://kc.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://di.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bz.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dd.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cc.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jn.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://tt.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ps.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yq.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://ms.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://pi.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ai.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nu.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wl.521024.cn

Go:   slices.Sort(arr)
来源：http://ek.nszjky.cn

Ruby: arr.sort
来源：http://by.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wg.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://bm.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dq.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://ay.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vl.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://po.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vk.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sn.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cc.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qy.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://go.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mm.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cc.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nm.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yz.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ux.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ez.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://px.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://id.9csxet.cn

[N05] 最大公约数
来源：http://rh.nicolike.cn

Py:   math.gcd(a, b)
来源：http://fc.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://of.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jc.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gq.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hh.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zc.hnjuh.cn

Ruby: a.gcd(b)
来源：http://sm.muxihuayi.cn


<!-- 参考信息 -->