代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pc.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qe.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rk.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yr.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yq.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ki.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://uc.521024.cn

Py:   now + timedelta(days=7)
来源：http://ng.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gu.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uv.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lg.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://nw.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ym.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://am.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pq.huixiangedu.cn

[J06] 计算两时间之差
来源：http://yb.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://gz.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://ua.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cg.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tg.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ho.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://pp.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://wa.521024.cn

C#:   (end - start).TotalSeconds
来源：http://il.wgjwhj.cn

[J07] 比较两个日期
来源：http://vi.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://rk.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fc.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gv.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sx.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gh.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rd.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lx.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://cl.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://mr.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eb.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xh.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bo.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cp.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eo.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cg.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vo.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pr.shxzukj.cn

[J09] 时区处理
来源：http://pf.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wv.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pf.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zq.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lo.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nd.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fn.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ft.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eg.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://uy.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qm.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gi.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gp.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oe.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fj.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ld.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rp.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fa.panjiajie.cn

================================================================================
来源：http://ym.jctech888.com.cn

K. JSON 与序列化
来源：http://vi.szxytkj.cn

================================================================================
来源：http://qj.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://de.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xu.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ef.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://he.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://hb.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bl.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://rv.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qf.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ru.nicolike.cn

[K02] JSON 字符串转对象
来源：http://xy.szsharing.cn

Py:   json.loads(s)
来源：http://vc.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qd.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://kz.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://ye.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jc.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://xa.521024.cn

Ruby: JSON.parse(s)
来源：http://di.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pp.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://ti.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hi.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ep.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fr.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://km.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jy.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pd.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gs.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tu.nszjky.cn

[K04] 读取 JSON 文件
来源：http://fe.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zp.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gv.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vy.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://du.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pb.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pe.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://je.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qy.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://uw.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://vp.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://ck.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://sd.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://xu.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cl.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uz.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ji.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tr.yuexingan06.cn

[K06] 解析 URL 查询串
来源：http://of.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rr.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yp.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rj.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tr.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ro.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xu.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ja.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xq.bjjhwx.cn

[K07] 进制转换
来源：http://bw.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yt.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://re.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mw.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dx.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dj.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jm.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rz.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://im.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://ua.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://fm.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dy.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://ws.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://fj.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vy.yuntaijiaju.cn

Go:   encoding/gob
来源：http://py.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://bw.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://im.panjiajie.cn

================================================================================
来源：http://ya.shtwfgs.cn

L. 网络请求
来源：http://my.jctech888.com.cn

================================================================================
来源：http://wb.panjiajie.cn

[L01] 发送 GET 请求
来源：http://di.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://as.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yp.nszjky.cn

JS:   await fetch(url)
来源：http://xd.colortex.cn

TS:   await fetch(url)
来源：http://fr.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pd.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://ln.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gw.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gq.panjiajie.cn

[L02] 发送 POST JSON
来源：http://wl.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zt.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mj.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jz.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dq.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ts.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://di.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ga.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://at.521024.cn

[L03] 设置自定义请求头
来源：http://jm.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dm.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ag.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zn.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ji.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cy.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rk.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rc.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dq.panjiajie.cn

[L04] 设置超时
来源：http://st.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://un.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wn.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tl.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eb.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kc.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wc.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ev.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kd.nicolike.cn

[L05] 上传文件（multipart）
来源：http://qg.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pc.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qo.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jo.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ps.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sx.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qy.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eb.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zl.newstarts.cn

[L06] 解析响应为 JSON
来源：http://br.wgjwhj.cn

Py:   resp.json()
来源：http://za.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://az.lnxyls.cn

JS:   await resp.json()
来源：http://px.521024.cn

TS:   await resp.json()
来源：http://fe.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xz.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zg.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://ze.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zx.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://hf.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ha.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ei.asd995.cn

JS:   resp.ok;  resp.status
来源：http://pi.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://yg.jctech888.com.cn

Java: resp.statusCode()
来源：http://qn.521024.cn

Go:   resp.StatusCode
来源：http://oz.nszjky.cn

Ruby: resp.code.to_i
来源：http://lq.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://kf.newstarts.cn

[L08] 并发请求多个地址
来源：http://bz.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://my.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://me.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vx.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rb.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vs.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pd.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lm.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wx.9csxet.cn

================================================================================
来源：http://vl.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://dn.huixinmuqiang.cn

================================================================================
来源：http://um.wgjwhj.cn

[M01] 读取命令行参数
来源：http://tm.szsharing.cn

Py:   sys.argv[1:]
来源：http://sw.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://hx.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://qz.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://pq.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://yu.newstarts.cn

Go:   os.Args[1:]
来源：http://cl.bookmarksfly.cn

Ruby: ARGV
来源：http://jf.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://ja.szxytkj.cn

[M02] 读取环境变量
来源：http://vz.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://ic.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mr.shxzukj.cn

JS:   process.env.HOME
来源：http://lp.wgjwhj.cn

TS:   process.env.HOME
来源：http://cb.shxzskj.cn

Java: System.getenv("HOME")
来源：http://fp.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xc.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://rk.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xv.colortex.cn

[M03] 执行外部命令
来源：http://su.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wo.muxihuayi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nr.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nt.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ip.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gz.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gs.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yn.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://wk.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://hs.asd995.cn

Py:   os.getcwd()
来源：http://pt.shxzskj.cn

PHP:  getcwd();
来源：http://kr.nicolike.cn

JS:   process.cwd()
来源：http://zb.hnjuh.cn

TS:   process.cwd()
来源：http://hv.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://yh.szxytkj.cn

Go:   os.Getwd()
来源：http://ao.haigaiapp.cn

Ruby: Dir.pwd
来源：http://ld.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://af.shxzukj.cn

[M05] 设置退出码
来源：http://wc.yuexingan06.cn

Py:   sys.exit(1)
来源：http://vt.jianghongdianzi.cn

PHP:  exit(1);
来源：http://vy.colortex.cn

JS:   process.exit(1)
来源：http://lc.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://wk.shtwfgs.cn

Java: System.exit(1)
来源：http://ke.shtwfgs.cn

Go:   os.Exit(1)
来源：http://jk.wgjwhj.cn

Ruby: exit 1
来源：http://dh.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fx.shxzukj.cn

[M06] 向标准错误输出
来源：http://kb.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://yy.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ga.bjjhwx.cn

JS:   console.error("err")
来源：http://lm.bjjhwx.cn

TS:   console.error("err")
来源：http://uf.nszjky.cn

Java: System.err.println("err")
来源：http://pb.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oi.colortex.cn

Ruby: warn "err"
来源：http://cd.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://ye.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://fh.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://dk.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rm.wgjwhj.cn

JS:   require.main === module
来源：http://mo.shxzskj.cn

TS:   require.main === module
来源：http://oi.nszjky.cn

Java: public static void main(String[] args)
来源：http://ws.shxzskj.cn

Go:   func main()
来源：http://ty.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pi.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://jj.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://lm.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://hg.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://ts.huanxung.cn

JS:   process.platform;  process.version
来源：http://og.9csxet.cn

TS:   process.platform;  process.version
来源：http://jt.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vy.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yr.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tv.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ct.wgjwhj.cn

================================================================================
来源：http://sv.yuntaijiaju.cn

N. 数据结构与算法
来源：http://cn.colortex.cn

================================================================================
来源：http://qe.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://db.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oi.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hr.huanxung.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bc.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ss.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gl.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://fy.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vm.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lj.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://kf.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://bu.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eu.newstarts.cn


<!-- 参考信息 -->