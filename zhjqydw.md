代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://po.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rc.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://no.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ok.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fg.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iv.lnxyls.cn

[J09] 时区处理
来源：http://hk.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jg.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gb.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://au.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gb.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://de.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ie.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pl.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cl.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://fw.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://iz.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vw.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rf.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qq.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lu.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sw.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pw.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oo.nszjky.cn

================================================================================
来源：http://db.shtwfgs.cn

K. JSON 与序列化
来源：http://jw.yuexingan06.cn

================================================================================
来源：http://ux.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://pu.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gj.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dy.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://hl.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://lm.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ol.huanxung.cn

Go:   json.Marshal(obj)
来源：http://ik.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vh.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mb.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://mu.shxzukj.cn

Py:   json.loads(s)
来源：http://ie.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nk.gzmigu.cn

JS:   JSON.parse(s)
来源：http://kz.asd995.cn

TS:   JSON.parse(s)
来源：http://qw.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gi.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://pb.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://cp.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pb.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://zk.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ds.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qf.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sp.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xv.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vk.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yy.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nc.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ak.521024.cn

[K04] 读取 JSON 文件
来源：http://tr.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ha.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wb.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://og.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://do.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ox.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yu.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mf.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xc.shxzukj.cn

[K05] 深拷贝对象
来源：http://pd.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://kh.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://ew.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://hn.asd995.cn

TS:   structuredClone(obj)
来源：http://do.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oj.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kk.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uu.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://be.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://dc.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xs.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ds.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sm.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cf.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vf.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lj.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fd.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jr.szxytkj.cn

[K07] 进制转换
来源：http://cd.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mp.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sh.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://je.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yo.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lv.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jv.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://np.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qk.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://wh.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://rm.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mw.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://ee.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://hx.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ie.jianghongdianzi.cn

Go:   encoding/gob
来源：http://nc.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://ja.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rk.panjiajie.cn

================================================================================
来源：http://iu.yuntaijiaju.cn

L. 网络请求
来源：http://et.huixiangedu.cn

================================================================================
来源：http://np.huanxung.cn

[L01] 发送 GET 请求
来源：http://ml.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pg.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bp.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://xd.bookmarksfly.cn

TS:   await fetch(url)
来源：http://te.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gb.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://rl.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xr.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ut.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://uq.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jq.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lm.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dw.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dl.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ua.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ps.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dn.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wo.gzmigu.cn

[L03] 设置自定义请求头
来源：http://ux.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://th.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kt.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ce.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://po.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ie.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ia.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bn.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ep.asd995.cn

[L04] 设置超时
来源：http://up.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://pi.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cc.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gz.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hh.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://os.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uo.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qh.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ex.asd995.cn

[L05] 上传文件（multipart）
来源：http://iu.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wk.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zc.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rh.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://un.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lh.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jz.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bc.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ut.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://xo.wgjwhj.cn

Py:   resp.json()
来源：http://fb.nszjky.cn

PHP:  json_decode($body, true);
来源：http://ed.szsharing.cn

JS:   await resp.json()
来源：http://zc.yuexingan06.cn

TS:   await resp.json()
来源：http://zk.shxzskj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rv.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mh.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://zi.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://we.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://wg.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uf.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cd.521024.cn

JS:   resp.ok;  resp.status
来源：http://ii.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://vw.nicolike.cn

Java: resp.statusCode()
来源：http://ym.colortex.cn

Go:   resp.StatusCode
来源：http://nn.nicolike.cn

Ruby: resp.code.to_i
来源：http://my.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://iu.lnxyls.cn

[L08] 并发请求多个地址
来源：http://gi.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tj.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://bd.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yj.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://he.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lt.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dm.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ey.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kv.lnxyls.cn

================================================================================
来源：http://bn.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://hl.huanxung.cn

================================================================================
来源：http://bo.hahajie.cn

[M01] 读取命令行参数
来源：http://cs.hnjuh.cn

Py:   sys.argv[1:]
来源：http://cf.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://rp.nszjky.cn

JS:   process.argv.slice(2)
来源：http://iz.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://el.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://ij.huanxung.cn

Go:   os.Args[1:]
来源：http://hh.521024.cn

Ruby: ARGV
来源：http://xh.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://wx.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://tk.521024.cn

Py:   os.environ.get("HOME")
来源：http://uu.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://re.haigaiapp.cn

JS:   process.env.HOME
来源：http://qn.haigaiapp.cn

TS:   process.env.HOME
来源：http://cd.asd995.cn

Java: System.getenv("HOME")
来源：http://pc.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wr.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://lk.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://os.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://qo.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vw.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mt.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ud.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ul.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cz.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jx.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kk.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://us.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://ya.haigaiapp.cn

Py:   os.getcwd()
来源：http://vq.shtwfgs.cn

PHP:  getcwd();
来源：http://dr.huixiangedu.cn

JS:   process.cwd()
来源：http://sq.wgjwhj.cn

TS:   process.cwd()
来源：http://kd.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://dv.asd995.cn

Go:   os.Getwd()
来源：http://na.shtwfgs.cn

Ruby: Dir.pwd
来源：http://qa.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zs.nicolike.cn

[M05] 设置退出码
来源：http://nx.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://ul.yuexingan06.cn

PHP:  exit(1);
来源：http://bb.panjiajie.cn

JS:   process.exit(1)
来源：http://ha.lnxyls.cn

TS:   process.exit(1)
来源：http://bz.yuexingan06.cn

Java: System.exit(1)
来源：http://hz.asd995.cn

Go:   os.Exit(1)
来源：http://zg.newstarts.cn

Ruby: exit 1
来源：http://jc.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zu.panjiajie.cn

[M06] 向标准错误输出
来源：http://tk.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://ya.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sm.panjiajie.cn

JS:   console.error("err")
来源：http://ja.huanxung.cn

TS:   console.error("err")
来源：http://hh.shxzskj.cn

Java: System.err.println("err")
来源：http://cr.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lh.nicolike.cn

Ruby: warn "err"
来源：http://io.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://lg.521024.cn

[M07] 判断是否为主入口
来源：http://lr.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://jr.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eo.colortex.cn

JS:   require.main === module
来源：http://ii.yuexingan06.cn

TS:   require.main === module
来源：http://uw.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://fx.shtwfgs.cn

Go:   func main()
来源：http://dp.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wk.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://qi.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://by.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://rz.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://rv.szxytkj.cn

JS:   process.platform;  process.version
来源：http://zi.9csxet.cn

TS:   process.platform;  process.version
来源：http://rx.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dj.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://to.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nd.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://is.bookmarksfly.cn

================================================================================
来源：http://uh.lnxyls.cn

N. 数据结构与算法
来源：http://ht.panjiajie.cn

================================================================================
来源：http://tf.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://dk.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hh.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hu.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pr.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hv.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oe.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://hl.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mw.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ph.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://bg.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://yh.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ga.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oc.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://be.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uz.9csxet.cn

Go:   slices.Sort(arr)
来源：http://nb.gzmigu.cn

Ruby: arr.sort
来源：http://wo.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gg.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://kd.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mg.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://fi.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://se.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xa.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tu.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mr.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://il.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ha.shxzukj.cn

[N04] 斐波那契数列
来源：http://ye.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ui.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://za.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tw.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iu.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zh.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://al.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rn.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cy.yuntaijiaju.cn

[N05] 最大公约数
来源：http://bq.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://zm.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ym.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ks.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vp.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ze.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nh.szsharing.cn

Ruby: a.gcd(b)
来源：http://st.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://av.shtwfgs.cn

[N06] 判断回文字符串
来源：http://fa.hahajie.cn

Py:   s == s[::-1]
来源：http://lq.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://tc.szxytkj.cn


<!-- 参考信息 -->