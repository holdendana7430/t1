代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xw.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xh.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sf.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mz.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bx.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mj.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://pw.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://ds.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mh.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kq.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jg.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://vb.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yy.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://bh.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kx.shxzukj.cn

[J06] 计算两时间之差
来源：http://yq.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://bf.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://uw.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://op.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kr.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pw.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://ce.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://uc.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://ob.hahajie.cn

[J07] 比较两个日期
来源：http://zn.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://mx.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://az.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ys.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ou.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://by.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://po.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xx.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://pf.521024.cn

[J08] 提取年月日与星期
来源：http://tt.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bd.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dc.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cy.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rv.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wl.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://et.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xx.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zr.hahajie.cn

[J09] 时区处理
来源：http://es.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qk.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ag.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lj.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dp.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nl.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jb.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sr.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://df.521024.cn

[J10] 取今天 / 本月第一天
来源：http://tl.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://di.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ym.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rr.shxzukj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ld.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qg.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cy.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://co.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uq.newstarts.cn

================================================================================
来源：http://ro.shtwfgs.cn

K. JSON 与序列化
来源：http://cp.szxytkj.cn

================================================================================
来源：http://ty.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://zr.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yq.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ax.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://lp.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://rn.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wn.nicolike.cn

Go:   json.Marshal(obj)
来源：http://fv.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oq.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bf.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://fb.hnjuh.cn

Py:   json.loads(s)
来源：http://kw.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ai.asd995.cn

JS:   JSON.parse(s)
来源：http://sm.szsharing.cn

TS:   JSON.parse(s)
来源：http://sj.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lv.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://ju.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://me.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xg.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ph.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://py.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sr.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ty.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sl.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ub.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tg.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://by.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ns.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://qo.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kv.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qy.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yv.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xz.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wq.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ng.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://de.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pj.hahajie.cn

[K05] 深拷贝对象
来源：http://mk.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://ey.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://lv.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://hq.gzmigu.cn

TS:   structuredClone(obj)
来源：http://cs.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hn.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ow.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wl.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pw.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://rv.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://an.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yc.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tk.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://za.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sn.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zz.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://od.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vn.chemitech.net.cn

[K07] 进制转换
来源：http://fy.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oq.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eb.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gj.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yt.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jo.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nn.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lu.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zf.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://or.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://vd.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yf.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://ns.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://up.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zr.wgjwhj.cn

Go:   encoding/gob
来源：http://ge.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://he.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tr.shxzukj.cn

================================================================================
来源：http://we.jianghongdianzi.cn

L. 网络请求
来源：http://eo.shxzskj.cn

================================================================================
来源：http://bz.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://fe.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://to.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://li.bookmarksfly.cn

JS:   await fetch(url)
来源：http://zz.shxzskj.cn

TS:   await fetch(url)
来源：http://yv.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tg.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://pq.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rr.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uq.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://vg.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yz.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sn.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lx.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wt.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yc.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xs.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vj.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fx.szsharing.cn

[L03] 设置自定义请求头
来源：http://dr.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wh.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hd.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qr.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sx.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gp.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vp.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://os.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ka.hahajie.cn

[L04] 设置超时
来源：http://fm.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://ar.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ri.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ls.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nz.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jk.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jh.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xv.9csxet.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jk.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://bn.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mo.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ay.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://te.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vs.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rs.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mi.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ot.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kb.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://hb.shxzukj.cn

Py:   resp.json()
来源：http://ik.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://ro.shxzukj.cn

JS:   await resp.json()
来源：http://hc.muxihuayi.cn

TS:   await resp.json()
来源：http://kq.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zb.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oe.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://ty.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ti.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://cd.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ie.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ha.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://yp.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://fu.hnjuh.cn

Java: resp.statusCode()
来源：http://xq.szxytkj.cn

Go:   resp.StatusCode
来源：http://dw.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://iu.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://of.newstarts.cn

[L08] 并发请求多个地址
来源：http://ka.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nr.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://qs.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bn.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nm.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bq.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tp.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aq.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xl.chemitech.net.cn

================================================================================
来源：http://gl.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://gs.nicolike.cn

================================================================================
来源：http://nq.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://mi.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://fw.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://ab.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://ed.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://ow.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://mo.szsharing.cn

Go:   os.Args[1:]
来源：http://zz.haigaiapp.cn

Ruby: ARGV
来源：http://jh.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://pv.asd995.cn

[M02] 读取环境变量
来源：http://qq.colortex.cn

Py:   os.environ.get("HOME")
来源：http://dz.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jf.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://lf.panjiajie.cn

TS:   process.env.HOME
来源：http://ae.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://hd.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://na.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://aq.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ys.wgjwhj.cn

[M03] 执行外部命令
来源：http://df.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ng.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lc.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://we.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xd.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ct.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wx.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mz.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://wo.hnjuh.cn

[M04] 获取当前工作目录
来源：http://ff.nszjky.cn

Py:   os.getcwd()
来源：http://hv.nicolike.cn

PHP:  getcwd();
来源：http://wj.colortex.cn

JS:   process.cwd()
来源：http://ex.jctech888.com.cn

TS:   process.cwd()
来源：http://cv.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://yy.bookmarksfly.cn

Go:   os.Getwd()
来源：http://yb.shxzskj.cn

Ruby: Dir.pwd
来源：http://kc.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gb.yuexingan06.cn

[M05] 设置退出码
来源：http://ko.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://cf.bjjhwx.cn

PHP:  exit(1);
来源：http://zo.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://dl.yuexingan06.cn

TS:   process.exit(1)
来源：http://qw.hnjuh.cn

Java: System.exit(1)
来源：http://gg.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://ar.shtwfgs.cn

Ruby: exit 1
来源：http://bu.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pg.wgjwhj.cn

[M06] 向标准错误输出
来源：http://zk.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://vr.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qa.shtwfgs.cn

JS:   console.error("err")
来源：http://vq.wgjwhj.cn

TS:   console.error("err")
来源：http://vk.shxzskj.cn

Java: System.err.println("err")
来源：http://sa.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iu.colortex.cn

Ruby: warn "err"
来源：http://bp.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://mp.nicolike.cn

[M07] 判断是否为主入口
来源：http://dz.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://zi.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wc.bjjhwx.cn

JS:   require.main === module
来源：http://lj.gzmigu.cn

TS:   require.main === module
来源：http://rm.szsharing.cn

Java: public static void main(String[] args)
来源：http://zq.chemitech.net.cn

Go:   func main()
来源：http://gf.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iv.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://tq.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://tx.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://og.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://ig.szxytkj.cn

JS:   process.platform;  process.version
来源：http://ft.nicolike.cn

TS:   process.platform;  process.version
来源：http://wd.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ua.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ps.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cc.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bh.hahajie.cn

================================================================================
来源：http://zm.jianghongdianzi.cn

N. 数据结构与算法
来源：http://og.9csxet.cn

================================================================================
来源：http://qt.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://df.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ib.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rs.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://td.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nd.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gw.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://rk.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gz.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ao.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://rh.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://kv.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://si.yuntaijiaju.cn


<!-- 参考信息 -->