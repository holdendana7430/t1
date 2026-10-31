代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zu.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xc.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://ak.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://ic.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fv.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cv.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ao.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://mu.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iy.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://va.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ai.521024.cn

[J06] 计算两时间之差
来源：http://kr.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://xr.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://rm.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nc.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xq.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ks.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://fk.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://ar.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://af.lnxyls.cn

[J07] 比较两个日期
来源：http://ux.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://bi.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ko.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wu.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ej.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ws.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://he.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nf.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://rd.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://mv.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ru.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yy.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://re.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vn.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lw.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gd.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jr.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://im.huixinmuqiang.cn

[J09] 时区处理
来源：http://oh.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://va.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://og.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bl.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vf.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wn.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zy.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zy.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zv.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://xk.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sw.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jk.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://il.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hw.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ng.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bg.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ct.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gu.chemitech.net.cn

================================================================================
来源：http://li.wgjwhj.cn

K. JSON 与序列化
来源：http://xt.yuntaijiaju.cn

================================================================================
来源：http://iw.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://ta.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ia.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pv.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://qh.huanxung.cn

TS:   JSON.stringify(obj)
来源：http://hm.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rp.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://xp.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://aw.lnxyls.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fj.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://qc.panjiajie.cn

Py:   json.loads(s)
来源：http://iv.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nk.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://qr.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://qc.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rx.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://sf.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://ix.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oi.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://hk.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://my.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gs.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vz.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://iw.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://st.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ca.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aj.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ye.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://fi.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tx.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://re.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xb.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dc.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vh.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lw.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cr.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ga.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://dq.521024.cn

Py:   copy.deepcopy(obj)
来源：http://dd.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://mi.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://hm.nszjky.cn

TS:   structuredClone(obj)
来源：http://rr.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zn.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hp.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ho.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fy.hahajie.cn

[K06] 解析 URL 查询串
来源：http://tk.huixinmuqiang.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xs.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://db.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fm.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rk.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xf.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pc.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tr.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://da.hnjuh.cn

[K07] 进制转换
来源：http://uq.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://td.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://is.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wv.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yq.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xb.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fn.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ix.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sq.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://tr.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://tq.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://oz.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://mr.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://jf.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gd.nszjky.cn

Go:   encoding/gob
来源：http://ld.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://tm.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sw.huixinmuqiang.cn

================================================================================
来源：http://yp.hnjuh.cn

L. 网络请求
来源：http://uu.huixinmuqiang.cn

================================================================================
来源：http://te.nicolike.cn

[L01] 发送 GET 请求
来源：http://ou.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yd.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hw.shxzukj.cn

JS:   await fetch(url)
来源：http://ms.bookmarksfly.cn

TS:   await fetch(url)
来源：http://ri.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ew.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://wn.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dv.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tu.newstarts.cn

[L02] 发送 POST JSON
来源：http://sx.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nv.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tw.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yj.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gp.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tm.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hd.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pp.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sh.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://yp.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mm.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nh.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vh.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://af.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ig.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pa.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ur.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://to.521024.cn

[L04] 设置超时
来源：http://az.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://ur.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zo.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ry.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vj.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ao.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nq.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ti.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ac.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://ij.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jw.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vq.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://in.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bw.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ne.szxytkj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ow.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ao.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://je.521024.cn

[L06] 解析响应为 JSON
来源：http://xc.huanxung.cn

Py:   resp.json()
来源：http://wy.colortex.cn

PHP:  json_decode($body, true);
来源：http://kl.9csxet.cn

JS:   await resp.json()
来源：http://sl.jctech888.com.cn

TS:   await resp.json()
来源：http://sa.shxzskj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://em.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ga.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://wa.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ka.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://bb.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qy.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ld.asd995.cn

JS:   resp.ok;  resp.status
来源：http://mq.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://mt.521024.cn

Java: resp.statusCode()
来源：http://cl.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://wx.521024.cn

Ruby: resp.code.to_i
来源：http://gg.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://yx.huanxung.cn

[L08] 并发请求多个地址
来源：http://fw.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ye.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://cj.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xo.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rq.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bx.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vs.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gj.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://po.nszjky.cn

================================================================================
来源：http://qx.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://vj.szxytkj.cn

================================================================================
来源：http://mc.hahajie.cn

[M01] 读取命令行参数
来源：http://cs.newstarts.cn

Py:   sys.argv[1:]
来源：http://gq.hahajie.cn

PHP:  $argv;  $argc;
来源：http://mn.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://wk.newstarts.cn

TS:   process.argv.slice(2)
来源：http://pn.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://yk.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://mh.jctech888.com.cn

Ruby: ARGV
来源：http://lm.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://tb.nicolike.cn

[M02] 读取环境变量
来源：http://an.asd995.cn

Py:   os.environ.get("HOME")
来源：http://er.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ap.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://rv.nicolike.cn

TS:   process.env.HOME
来源：http://mb.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://qk.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zw.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://ws.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ya.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://vh.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xv.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jo.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tv.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mg.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kh.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tu.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vx.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://tj.szxytkj.cn

[M04] 获取当前工作目录
来源：http://xd.bjjhwx.cn

Py:   os.getcwd()
来源：http://ht.jianghongdianzi.cn

PHP:  getcwd();
来源：http://lf.hahajie.cn

JS:   process.cwd()
来源：http://ie.bjjhwx.cn

TS:   process.cwd()
来源：http://ia.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://wj.asd995.cn

Go:   os.Getwd()
来源：http://mb.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://el.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://it.szxytkj.cn

[M05] 设置退出码
来源：http://qb.shxzskj.cn

Py:   sys.exit(1)
来源：http://cu.huanxung.cn

PHP:  exit(1);
来源：http://yl.huixiangedu.cn

JS:   process.exit(1)
来源：http://yl.bjjhwx.cn

TS:   process.exit(1)
来源：http://fo.haigaiapp.cn

Java: System.exit(1)
来源：http://lq.shtwfgs.cn

Go:   os.Exit(1)
来源：http://xq.wgjwhj.cn

Ruby: exit 1
来源：http://gj.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tq.colortex.cn

[M06] 向标准错误输出
来源：http://ul.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://bs.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bb.gzmigu.cn

JS:   console.error("err")
来源：http://jy.521024.cn

TS:   console.error("err")
来源：http://js.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://jj.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ec.gzmigu.cn

Ruby: warn "err"
来源：http://cw.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://bf.colortex.cn

[M07] 判断是否为主入口
来源：http://de.521024.cn

Py:   if __name__ == "__main__":
来源：http://of.jianghongdianzi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yd.shtwfgs.cn

JS:   require.main === module
来源：http://kl.shxzskj.cn

TS:   require.main === module
来源：http://zu.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://us.asd995.cn

Go:   func main()
来源：http://cl.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jc.newstarts.cn

C#:   static void Main(string[] args)
来源：http://oi.521024.cn

[M08] 获取系统与运行时信息
来源：http://hv.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://tb.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://le.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://vc.szxytkj.cn

TS:   process.platform;  process.version
来源：http://wn.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://to.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://md.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ut.wgjwhj.cn

================================================================================
来源：http://ky.yuntaijiaju.cn

N. 数据结构与算法
来源：http://ao.hnjuh.cn

================================================================================
来源：http://mx.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://al.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://he.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sb.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://am.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zb.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pj.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://ox.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ri.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tv.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://by.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://cb.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kq.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://po.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ah.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zy.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://lo.shxzskj.cn


<!-- 参考信息 -->