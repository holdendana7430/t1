代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://it.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vz.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ag.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zk.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://ek.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://wi.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bb.bookmarksfly.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lw.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ms.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pg.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uu.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ah.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cf.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lg.nicolike.cn

[J09] 时区处理
来源：http://rn.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eb.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://we.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wx.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fo.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pd.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ou.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rp.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mn.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://gc.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jx.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tu.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mt.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ob.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gl.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cy.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rf.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zm.jctech888.com.cn

================================================================================
来源：http://eb.hahajie.cn

K. JSON 与序列化
来源：http://ci.bookmarksfly.cn

================================================================================
来源：http://yg.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://qo.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yk.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qw.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://rf.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://wc.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zy.huanxung.cn

Go:   json.Marshal(obj)
来源：http://kl.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mz.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ls.newstarts.cn

[K02] JSON 字符串转对象
来源：http://hy.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://vd.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hg.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://ye.521024.cn

TS:   JSON.parse(s)
来源：http://ls.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gn.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://xf.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://jw.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fl.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://tw.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lg.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uj.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dd.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sp.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yr.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sz.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://em.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vc.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://vr.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hj.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fh.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vk.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://py.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lz.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lp.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gz.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://te.hnjuh.cn

[K05] 深拷贝对象
来源：http://ox.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://jw.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://xz.shxzskj.cn

JS:   structuredClone(obj)
来源：http://as.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://oz.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dg.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wj.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://me.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tu.hahajie.cn

[K06] 解析 URL 查询串
来源：http://da.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jr.huixinmuqiang.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qw.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ev.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ou.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jx.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fb.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tf.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ir.hnjuh.cn

[K07] 进制转换
来源：http://cm.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mp.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ux.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ju.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kj.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zj.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kc.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wl.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rs.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://kd.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://xy.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sy.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://cc.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://oh.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xn.asd995.cn

Go:   encoding/gob
来源：http://zj.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://co.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bk.yuntaijiaju.cn

================================================================================
来源：http://ha.shtwfgs.cn

L. 网络请求
来源：http://pw.bookmarksfly.cn

================================================================================
来源：http://im.hnjuh.cn

[L01] 发送 GET 请求
来源：http://tn.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rw.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bd.bjjhwx.cn

JS:   await fetch(url)
来源：http://kl.nszjky.cn

TS:   await fetch(url)
来源：http://ri.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ur.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://xz.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://er.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bo.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://bw.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://id.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fq.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bf.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kw.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ca.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pe.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ab.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://no.hahajie.cn

[L03] 设置自定义请求头
来源：http://fq.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://un.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://js.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eh.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bi.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eq.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jk.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fj.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sw.gzmigu.cn

[L04] 设置超时
来源：http://rw.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://py.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qv.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jz.jianghongdianzi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ep.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eo.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yg.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jw.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tw.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://tb.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://to.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fn.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://av.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ds.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hf.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gj.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ko.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wi.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://bv.panjiajie.cn

Py:   resp.json()
来源：http://mv.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://ye.chemitech.net.cn

JS:   await resp.json()
来源：http://mn.yuexingan06.cn

TS:   await resp.json()
来源：http://vw.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ho.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tm.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://ai.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fu.521024.cn

[L07] 处理 HTTP 状态码
来源：http://lb.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jp.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hb.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://sa.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://qz.shtwfgs.cn

Java: resp.statusCode()
来源：http://yd.panjiajie.cn

Go:   resp.StatusCode
来源：http://jg.panjiajie.cn

Ruby: resp.code.to_i
来源：http://ya.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://hz.szxytkj.cn

[L08] 并发请求多个地址
来源：http://rh.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kn.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://ob.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lv.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ra.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ep.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xf.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hc.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gd.shtwfgs.cn

================================================================================
来源：http://jc.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://zt.newstarts.cn

================================================================================
来源：http://pf.wgjwhj.cn

[M01] 读取命令行参数
来源：http://gj.521024.cn

Py:   sys.argv[1:]
来源：http://tj.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://zf.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://pu.nszjky.cn

TS:   process.argv.slice(2)
来源：http://yr.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://xu.huanxung.cn

Go:   os.Args[1:]
来源：http://rl.shxzukj.cn

Ruby: ARGV
来源：http://jf.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://pv.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://by.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://wl.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wx.lnxyls.cn

JS:   process.env.HOME
来源：http://yz.lnxyls.cn

TS:   process.env.HOME
来源：http://aj.nszjky.cn

Java: System.getenv("HOME")
来源：http://wv.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://so.newstarts.cn

Ruby: ENV["HOME"]
来源：http://lr.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://au.hnjuh.cn

[M03] 执行外部命令
来源：http://hk.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ff.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ky.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tj.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bz.521024.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://da.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pv.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oa.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://ti.hahajie.cn

[M04] 获取当前工作目录
来源：http://zd.9csxet.cn

Py:   os.getcwd()
来源：http://ei.wgjwhj.cn

PHP:  getcwd();
来源：http://lp.yuexingan06.cn

JS:   process.cwd()
来源：http://lx.huanxung.cn

TS:   process.cwd()
来源：http://oh.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://qg.shtwfgs.cn

Go:   os.Getwd()
来源：http://qx.lnxyls.cn

Ruby: Dir.pwd
来源：http://fv.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vm.newstarts.cn

[M05] 设置退出码
来源：http://yv.panjiajie.cn

Py:   sys.exit(1)
来源：http://gy.wgjwhj.cn

PHP:  exit(1);
来源：http://nq.521024.cn

JS:   process.exit(1)
来源：http://vy.9csxet.cn

TS:   process.exit(1)
来源：http://yi.muxihuayi.cn

Java: System.exit(1)
来源：http://hh.nszjky.cn

Go:   os.Exit(1)
来源：http://wj.jianghongdianzi.cn

Ruby: exit 1
来源：http://sw.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bo.huixiangedu.cn

[M06] 向标准错误输出
来源：http://xv.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://bg.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qc.bjjhwx.cn

JS:   console.error("err")
来源：http://ue.jianghongdianzi.cn

TS:   console.error("err")
来源：http://gl.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://la.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ba.9csxet.cn

Ruby: warn "err"
来源：http://hg.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://jf.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://od.huixinmuqiang.cn

Py:   if __name__ == "__main__":
来源：http://iu.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rd.hahajie.cn

JS:   require.main === module
来源：http://yt.colortex.cn

TS:   require.main === module
来源：http://be.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://bs.gzmigu.cn

Go:   func main()
来源：http://si.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dm.szsharing.cn

C#:   static void Main(string[] args)
来源：http://bq.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://my.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://lp.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://bo.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://je.hahajie.cn

TS:   process.platform;  process.version
来源：http://uz.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lk.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wc.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sq.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jo.shxzukj.cn

================================================================================
来源：http://co.huanxung.cn

N. 数据结构与算法
来源：http://rl.shxzukj.cn

================================================================================
来源：http://di.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://ot.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gq.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hr.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ps.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jb.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bc.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://ba.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jo.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ww.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://gx.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://qp.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dn.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bc.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sr.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nz.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://nv.shxzskj.cn

Ruby: arr.sort
来源：http://jh.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hv.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://lx.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dg.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://ro.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tf.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lf.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zx.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fb.bjjhwx.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rc.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fj.wgjwhj.cn

[N04] 斐波那契数列
来源：http://ns.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ka.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hi.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oc.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sk.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pi.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oe.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kt.muxihuayi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fw.yuexingan06.cn

[N05] 最大公约数
来源：http://kp.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://tr.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kr.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ud.nszjky.cn


<!-- 参考信息 -->