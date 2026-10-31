代发 wailian999

[J07] 比较两个日期
来源：http://fn.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://jb.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://co.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://er.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uc.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://je.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bs.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ot.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://lv.colortex.cn

[J08] 提取年月日与星期
来源：http://wd.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eg.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gw.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qh.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dy.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://np.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gq.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bu.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cd.yuntaijiaju.cn

[J09] 时区处理
来源：http://ty.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tn.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bf.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tw.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://me.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ye.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://py.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vq.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xu.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://jt.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gu.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bb.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wb.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yv.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qj.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://is.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cb.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jh.bookmarksfly.cn

================================================================================
来源：http://vb.yuntaijiaju.cn

K. JSON 与序列化
来源：http://gz.huanxung.cn

================================================================================
来源：http://wl.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://ba.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ag.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lw.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://fw.asd995.cn

TS:   JSON.stringify(obj)
来源：http://os.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wi.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://cw.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://br.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ul.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://yq.bookmarksfly.cn

Py:   json.loads(s)
来源：http://ug.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://on.9csxet.cn

JS:   JSON.parse(s)
来源：http://tg.huanxung.cn

TS:   JSON.parse(s)
来源：http://vy.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cx.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://ek.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://aw.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eo.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://nj.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ai.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jv.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uo.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pw.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xs.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://py.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uy.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ht.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://nq.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://py.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vy.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dn.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rm.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wd.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eo.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://if.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xa.shtwfgs.cn

[K05] 深拷贝对象
来源：http://is.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://sd.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://gg.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://fw.9csxet.cn

TS:   structuredClone(obj)
来源：http://dc.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://it.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jt.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tm.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gm.asd995.cn

[K06] 解析 URL 查询串
来源：http://ub.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dt.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kr.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ph.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hm.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dm.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://iy.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ri.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dp.shxzskj.cn

[K07] 进制转换
来源：http://ty.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ef.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sh.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ag.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ou.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hj.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ki.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nr.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rw.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://zr.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://xs.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://en.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://vl.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://kg.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vx.9csxet.cn

Go:   encoding/gob
来源：http://tt.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://uh.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sn.gzmigu.cn

================================================================================
来源：http://iw.gzmigu.cn

L. 网络请求
来源：http://xu.muxihuayi.cn

================================================================================
来源：http://ee.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://lp.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sk.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sr.huanxung.cn

JS:   await fetch(url)
来源：http://ce.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://kk.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xy.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://kz.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oh.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bu.asd995.cn

[L02] 发送 POST JSON
来源：http://wy.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nh.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://le.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ot.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hr.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://is.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rr.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://di.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xo.asd995.cn

[L03] 设置自定义请求头
来源：http://os.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nt.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ql.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sr.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gf.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ku.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sf.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cf.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zy.9csxet.cn

[L04] 设置超时
来源：http://wu.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://tq.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ba.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xt.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qf.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ta.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qj.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lk.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zf.nicolike.cn

[L05] 上传文件（multipart）
来源：http://oz.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bi.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://az.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ia.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://in.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lr.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ma.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qc.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://be.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://ie.9csxet.cn

Py:   resp.json()
来源：http://wq.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://jd.newstarts.cn

JS:   await resp.json()
来源：http://wn.jianghongdianzi.cn

TS:   await resp.json()
来源：http://tm.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nm.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://av.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://wn.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ba.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://re.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fv.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sx.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://gz.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://pm.hnjuh.cn

Java: resp.statusCode()
来源：http://js.chemitech.net.cn

Go:   resp.StatusCode
来源：http://cu.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://rr.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://iz.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://xe.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zr.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://nb.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hv.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rw.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mz.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xi.nicolike.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vu.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jb.asd995.cn

================================================================================
来源：http://io.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://nf.bookmarksfly.cn

================================================================================
来源：http://og.shxzukj.cn

[M01] 读取命令行参数
来源：http://jt.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://ht.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://fj.huanxung.cn

JS:   process.argv.slice(2)
来源：http://bf.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://sn.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://wt.shtwfgs.cn

Go:   os.Args[1:]
来源：http://rh.lnxyls.cn

Ruby: ARGV
来源：http://ex.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://zi.shxzukj.cn

[M02] 读取环境变量
来源：http://sy.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://wx.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bl.huanxung.cn

JS:   process.env.HOME
来源：http://mn.chemitech.net.cn

TS:   process.env.HOME
来源：http://kk.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://ym.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://px.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://qu.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://le.hnjuh.cn

[M03] 执行外部命令
来源：http://jx.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tw.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fu.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cn.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zu.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sa.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dg.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ew.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://ni.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://vu.shtwfgs.cn

Py:   os.getcwd()
来源：http://pl.chemitech.net.cn

PHP:  getcwd();
来源：http://il.nicolike.cn

JS:   process.cwd()
来源：http://qw.asd995.cn

TS:   process.cwd()
来源：http://hn.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://qm.panjiajie.cn

Go:   os.Getwd()
来源：http://hv.nszjky.cn

Ruby: Dir.pwd
来源：http://pi.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://eu.jctech888.com.cn

[M05] 设置退出码
来源：http://xg.chemitech.net.cn

Py:   sys.exit(1)
来源：http://vf.colortex.cn

PHP:  exit(1);
来源：http://oy.9csxet.cn

JS:   process.exit(1)
来源：http://hn.huixiangedu.cn

TS:   process.exit(1)
来源：http://we.jctech888.com.cn

Java: System.exit(1)
来源：http://no.chemitech.net.cn

Go:   os.Exit(1)
来源：http://td.huixiangedu.cn

Ruby: exit 1
来源：http://yn.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nd.521024.cn

[M06] 向标准错误输出
来源：http://we.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://xb.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ac.colortex.cn

JS:   console.error("err")
来源：http://jb.gzmigu.cn

TS:   console.error("err")
来源：http://pr.panjiajie.cn

Java: System.err.println("err")
来源：http://ln.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ap.szxytkj.cn

Ruby: warn "err"
来源：http://gg.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://ma.asd995.cn

[M07] 判断是否为主入口
来源：http://wm.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://hb.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xn.nicolike.cn

JS:   require.main === module
来源：http://jm.gzmigu.cn

TS:   require.main === module
来源：http://pb.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://hx.huixiangedu.cn

Go:   func main()
来源：http://jd.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dd.szsharing.cn

C#:   static void Main(string[] args)
来源：http://hb.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://tu.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://mt.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://xx.gzmigu.cn

JS:   process.platform;  process.version
来源：http://dy.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://ht.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://am.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ez.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fk.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nj.nicolike.cn

================================================================================
来源：http://ba.panjiajie.cn

N. 数据结构与算法
来源：http://ws.muxihuayi.cn

================================================================================
来源：http://qu.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://db.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ri.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kc.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://st.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ch.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wo.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://ha.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xw.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ek.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://vm.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://pe.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bz.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xq.nicolike.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sa.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vh.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://yg.jctech888.com.cn

Ruby: arr.sort
来源：http://uv.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fn.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://jq.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ce.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://cy.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ua.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xt.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ve.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qq.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fm.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xc.colortex.cn

[N04] 斐波那契数列
来源：http://ix.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iy.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lk.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ru.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ut.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zl.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hu.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ju.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gr.colortex.cn


<!-- 参考信息 -->