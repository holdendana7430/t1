代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ei.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lo.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xa.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://no.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zj.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gs.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://lv.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://ww.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://eb.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ys.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rn.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://gn.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lp.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://vi.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://di.panjiajie.cn

[J06] 计算两时间之差
来源：http://tq.asd995.cn

Py:   (end - start).total_seconds()
来源：http://ee.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://so.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ox.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ug.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cq.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://ie.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://ib.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://ae.yuexingan06.cn

[J07] 比较两个日期
来源：http://nn.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://id.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kf.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bz.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://aq.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gp.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dt.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hd.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://yk.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://cv.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sq.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ys.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rs.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hk.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pv.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oo.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sv.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bm.lnxyls.cn

[J09] 时区处理
来源：http://lt.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xr.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cp.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://la.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hx.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mr.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://np.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kn.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dc.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://vu.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wn.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mi.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jm.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gp.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lq.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qw.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qq.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lg.colortex.cn

================================================================================
来源：http://sb.haigaiapp.cn

K. JSON 与序列化
来源：http://ry.huixinmuqiang.cn

================================================================================
来源：http://us.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://xp.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hf.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://px.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://yc.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://wn.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ya.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://wa.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://no.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ym.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://zt.haigaiapp.cn

Py:   json.loads(s)
来源：http://il.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qp.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://zi.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://kj.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ue.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://xp.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://ms.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oj.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://rf.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vf.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://om.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ls.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xu.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ha.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fh.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fo.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ld.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://uj.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ov.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sx.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gv.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zg.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://el.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ex.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://me.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lr.nszjky.cn

[K05] 深拷贝对象
来源：http://vm.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://cf.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://jl.hahajie.cn

JS:   structuredClone(obj)
来源：http://mu.shxzukj.cn

TS:   structuredClone(obj)
来源：http://pr.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zi.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zl.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vc.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xv.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://dg.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://us.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hb.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hh.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ww.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wr.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jw.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pw.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wi.szxytkj.cn

[K07] 进制转换
来源：http://pr.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ud.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://do.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://or.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ua.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cu.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ie.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://if.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mt.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://rz.asd995.cn

Py:   pickle.dumps(obj)
来源：http://ya.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sj.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://bq.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://cz.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qz.bookmarksfly.cn

Go:   encoding/gob
来源：http://lz.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://qc.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yd.colortex.cn

================================================================================
来源：http://vo.9csxet.cn

L. 网络请求
来源：http://ja.szxytkj.cn

================================================================================
来源：http://at.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://sd.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://va.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pt.9csxet.cn

JS:   await fetch(url)
来源：http://bk.bjjhwx.cn

TS:   await fetch(url)
来源：http://mm.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bq.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://ha.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nh.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qg.hnjuh.cn

[L02] 发送 POST JSON
来源：http://qj.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wl.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ce.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ye.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pm.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dq.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://op.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wj.hahajie.cn

[L03] 设置自定义请求头
来源：http://tz.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nw.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vl.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nw.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pb.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nq.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nm.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wz.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ge.yuntaijiaju.cn

[L04] 设置超时
来源：http://ec.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://mm.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lm.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vv.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qz.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nt.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mv.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fy.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://fs.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vx.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://td.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cq.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ld.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://de.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://od.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dk.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kh.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://bh.hnjuh.cn

Py:   resp.json()
来源：http://dr.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://ak.gzmigu.cn

JS:   await resp.json()
来源：http://tj.jianghongdianzi.cn

TS:   await resp.json()
来源：http://my.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ah.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mg.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://og.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wg.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://zo.newstarts.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gd.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ow.colortex.cn

JS:   resp.ok;  resp.status
来源：http://bd.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://jr.lnxyls.cn

Java: resp.statusCode()
来源：http://of.521024.cn

Go:   resp.StatusCode
来源：http://ga.gzmigu.cn

Ruby: resp.code.to_i
来源：http://xy.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://eb.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://sq.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jp.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://mf.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tq.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lr.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xd.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zo.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://it.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ci.jctech888.com.cn

================================================================================
来源：http://uv.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://hw.lnxyls.cn

================================================================================
来源：http://tz.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://lz.asd995.cn

Py:   sys.argv[1:]
来源：http://lv.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://vu.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://nm.newstarts.cn

TS:   process.argv.slice(2)
来源：http://ua.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://jr.huixiangedu.cn

Go:   os.Args[1:]
来源：http://ys.chemitech.net.cn

Ruby: ARGV
来源：http://dk.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://wh.521024.cn

[M02] 读取环境变量
来源：http://nx.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://sm.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rm.huixiangedu.cn

JS:   process.env.HOME
来源：http://hb.colortex.cn

TS:   process.env.HOME
来源：http://ia.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://iq.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ng.nicolike.cn

Ruby: ENV["HOME"]
来源：http://rd.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sb.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://ma.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zv.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qv.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://md.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bo.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fs.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hj.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vv.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://io.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://db.panjiajie.cn

Py:   os.getcwd()
来源：http://eo.asd995.cn

PHP:  getcwd();
来源：http://ml.hnjuh.cn

JS:   process.cwd()
来源：http://de.colortex.cn

TS:   process.cwd()
来源：http://ck.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://gp.lnxyls.cn

Go:   os.Getwd()
来源：http://ow.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://dp.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qj.colortex.cn

[M05] 设置退出码
来源：http://yp.nszjky.cn

Py:   sys.exit(1)
来源：http://pb.nicolike.cn

PHP:  exit(1);
来源：http://me.shxzukj.cn

JS:   process.exit(1)
来源：http://nf.lnxyls.cn

TS:   process.exit(1)
来源：http://im.szsharing.cn

Java: System.exit(1)
来源：http://ks.nicolike.cn

Go:   os.Exit(1)
来源：http://kh.lnxyls.cn

Ruby: exit 1
来源：http://wg.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qy.bjjhwx.cn

[M06] 向标准错误输出
来源：http://uk.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://gd.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://om.bjjhwx.cn

JS:   console.error("err")
来源：http://ur.jctech888.com.cn

TS:   console.error("err")
来源：http://el.shtwfgs.cn

Java: System.err.println("err")
来源：http://vc.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jx.shtwfgs.cn

Ruby: warn "err"
来源：http://ix.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://er.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://ix.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://sv.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cx.shxzskj.cn

JS:   require.main === module
来源：http://wk.muxihuayi.cn

TS:   require.main === module
来源：http://kw.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://pd.bjjhwx.cn

Go:   func main()
来源：http://qx.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rp.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://ik.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://bk.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://kw.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://kx.lnxyls.cn

JS:   process.platform;  process.version
来源：http://za.shxzskj.cn

TS:   process.platform;  process.version
来源：http://md.jctech888.com.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xk.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ry.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://co.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://va.panjiajie.cn

================================================================================
来源：http://wm.shxzukj.cn

N. 数据结构与算法
来源：http://me.chemitech.net.cn

================================================================================
来源：http://dk.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://nl.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ce.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vt.huanxung.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ng.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ei.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://li.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://pj.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yt.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pn.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://tn.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://ke.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ov.521024.cn


<!-- 参考信息 -->