代发 wailian999

TS:   new Date("2024-01-02")
来源：http://my.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bk.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fq.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://lk.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dc.colortex.cn

[J04] 时间戳与日期互转
来源：http://uu.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://te.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yx.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ge.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qo.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xf.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ka.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hf.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zy.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://ic.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://wb.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://va.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ud.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eh.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://td.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wa.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://sz.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kt.nicolike.cn

[J06] 计算两时间之差
来源：http://pd.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://ou.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://vd.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bm.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ir.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mf.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://rx.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://tu.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://wh.nszjky.cn

[J07] 比较两个日期
来源：http://em.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://qr.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://la.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ze.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jy.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hn.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bf.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dc.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://to.521024.cn

[J08] 提取年月日与星期
来源：http://gm.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dm.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://as.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hr.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uz.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://km.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rg.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vd.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zr.huanxung.cn

[J09] 时区处理
来源：http://pd.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vg.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lf.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://js.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pl.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ss.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ub.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://be.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zl.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://va.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://we.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zm.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fg.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hs.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lv.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xv.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vg.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iu.newstarts.cn

================================================================================
来源：http://vf.huixinmuqiang.cn

K. JSON 与序列化
来源：http://tq.chemitech.net.cn

================================================================================
来源：http://sv.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://dy.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ay.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xv.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://og.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://oj.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://do.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://db.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rd.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fk.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://sh.bjjhwx.cn

Py:   json.loads(s)
来源：http://hw.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tc.lnxyls.cn

JS:   JSON.parse(s)
来源：http://ke.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://am.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qr.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://jc.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://zx.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wd.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://cz.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yq.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fp.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ci.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uu.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lw.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yj.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lx.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hf.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://fq.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://if.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oo.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cn.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fu.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://br.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nl.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gv.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eb.newstarts.cn

[K05] 深拷贝对象
来源：http://fd.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://sp.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://il.huanxung.cn

JS:   structuredClone(obj)
来源：http://mt.szsharing.cn

TS:   structuredClone(obj)
来源：http://wx.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://za.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wk.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sb.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cd.colortex.cn

[K06] 解析 URL 查询串
来源：http://hi.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lm.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cw.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nj.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xh.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cg.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gt.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jt.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bo.hnjuh.cn

[K07] 进制转换
来源：http://lh.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dp.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ey.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wr.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://er.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uk.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sp.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lc.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pw.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://tl.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://vs.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ax.szsharing.cn

JS:   v8.serialize(obj)        // Node
来源：http://bo.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://ey.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ls.hahajie.cn

Go:   encoding/gob
来源：http://mk.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://zq.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sm.bookmarksfly.cn

================================================================================
来源：http://nv.chemitech.net.cn

L. 网络请求
来源：http://zs.nicolike.cn

================================================================================
来源：http://yw.9csxet.cn

[L01] 发送 GET 请求
来源：http://nh.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sa.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yr.bookmarksfly.cn

JS:   await fetch(url)
来源：http://nb.jctech888.com.cn

TS:   await fetch(url)
来源：http://ue.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jt.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://we.asd995.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gi.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ws.9csxet.cn

[L02] 发送 POST JSON
来源：http://ia.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fu.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ru.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fa.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zf.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ip.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://me.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kr.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bw.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://gc.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://om.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sv.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://me.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mf.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pe.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cq.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qf.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vf.lnxyls.cn

[L04] 设置超时
来源：http://vv.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://hq.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://od.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://on.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ui.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qs.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ok.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dc.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jy.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://dr.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fj.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gq.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vw.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qj.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bk.szxytkj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ru.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ed.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vs.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://qm.nszjky.cn

Py:   resp.json()
来源：http://hg.asd995.cn

PHP:  json_decode($body, true);
来源：http://gh.shtwfgs.cn

JS:   await resp.json()
来源：http://rt.yuntaijiaju.cn

TS:   await resp.json()
来源：http://qk.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qh.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cg.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://og.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xh.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://oh.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wi.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zr.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://be.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://bn.newstarts.cn

Java: resp.statusCode()
来源：http://qv.nszjky.cn

Go:   resp.StatusCode
来源：http://lk.nicolike.cn

Ruby: resp.code.to_i
来源：http://cu.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://ox.newstarts.cn

[L08] 并发请求多个地址
来源：http://iy.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vp.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://fm.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gr.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fg.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ae.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ky.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pz.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jr.haigaiapp.cn

================================================================================
来源：http://dg.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://yf.panjiajie.cn

================================================================================
来源：http://or.nszjky.cn

[M01] 读取命令行参数
来源：http://ni.gzmigu.cn

Py:   sys.argv[1:]
来源：http://sq.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://vy.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://tf.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://it.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://kt.haigaiapp.cn

Go:   os.Args[1:]
来源：http://gs.9csxet.cn

Ruby: ARGV
来源：http://rh.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://jd.521024.cn

[M02] 读取环境变量
来源：http://tg.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://ic.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kg.szxytkj.cn

JS:   process.env.HOME
来源：http://wu.wgjwhj.cn

TS:   process.env.HOME
来源：http://jf.szxytkj.cn

Java: System.getenv("HOME")
来源：http://ep.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ow.colortex.cn

Ruby: ENV["HOME"]
来源：http://za.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gq.nszjky.cn

[M03] 执行外部命令
来源：http://wz.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jx.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lw.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wc.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qh.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pl.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ng.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jg.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://ei.newstarts.cn

[M04] 获取当前工作目录
来源：http://qw.chemitech.net.cn

Py:   os.getcwd()
来源：http://pv.gzmigu.cn

PHP:  getcwd();
来源：http://ea.hahajie.cn

JS:   process.cwd()
来源：http://eg.hnjuh.cn

TS:   process.cwd()
来源：http://al.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://ha.colortex.cn

Go:   os.Getwd()
来源：http://yj.nicolike.cn

Ruby: Dir.pwd
来源：http://ik.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ie.jctech888.com.cn

[M05] 设置退出码
来源：http://fa.colortex.cn

Py:   sys.exit(1)
来源：http://hp.shtwfgs.cn

PHP:  exit(1);
来源：http://ez.nszjky.cn

JS:   process.exit(1)
来源：http://dy.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://wy.huixinmuqiang.cn

Java: System.exit(1)
来源：http://au.shxzukj.cn

Go:   os.Exit(1)
来源：http://ng.chemitech.net.cn

Ruby: exit 1
来源：http://yz.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ae.shxzskj.cn

[M06] 向标准错误输出
来源：http://th.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://iz.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://at.chemitech.net.cn

JS:   console.error("err")
来源：http://qa.colortex.cn

TS:   console.error("err")
来源：http://ar.nicolike.cn

Java: System.err.println("err")
来源：http://by.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rp.bjjhwx.cn

Ruby: warn "err"
来源：http://br.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://ca.9csxet.cn

[M07] 判断是否为主入口
来源：http://ix.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://ox.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dl.bookmarksfly.cn

JS:   require.main === module
来源：http://ol.lnxyls.cn

TS:   require.main === module
来源：http://eo.hnjuh.cn

Java: public static void main(String[] args)
来源：http://hj.hnjuh.cn

Go:   func main()
来源：http://bl.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cg.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://tz.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://ne.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://um.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://xf.szxytkj.cn

JS:   process.platform;  process.version
来源：http://se.hnjuh.cn

TS:   process.platform;  process.version
来源：http://bm.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dx.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ge.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zo.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ky.huixiangedu.cn

================================================================================
来源：http://qe.panjiajie.cn

N. 数据结构与算法
来源：http://kb.shxzskj.cn

================================================================================
来源：http://ro.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://nf.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hy.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gj.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qr.colortex.cn


<!-- 参考信息 -->