代发 wailian999

TS:   new Date("2024-01-02")
来源：http://mr.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xa.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dh.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://hn.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bw.newstarts.cn

[J04] 时间戳与日期互转
来源：http://uh.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dn.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xi.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ud.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://eg.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qo.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ep.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hf.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qb.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://jy.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://cu.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tz.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lv.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qx.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://bw.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://od.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://ee.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://oc.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://mj.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://ps.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://nr.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yp.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bz.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dm.521024.cn

Go:   end.Sub(start).Hours()
来源：http://yh.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://cm.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://jg.szsharing.cn

[J07] 比较两个日期
来源：http://kc.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://fx.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oc.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://at.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hg.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://od.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dh.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qj.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://ic.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://ij.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pr.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://db.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://li.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://od.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pq.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ti.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://og.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lg.521024.cn

[J09] 时区处理
来源：http://ma.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zn.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lw.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hg.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zy.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bd.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xa.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://of.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vt.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://kg.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vk.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cw.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xp.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xk.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xi.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iq.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jn.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yx.gzmigu.cn

================================================================================
来源：http://dh.shxzskj.cn

K. JSON 与序列化
来源：http://lz.hahajie.cn

================================================================================
来源：http://yi.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://ny.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hs.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nd.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://vl.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://xx.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://af.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://nx.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ma.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ko.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://kq.szsharing.cn

Py:   json.loads(s)
来源：http://eb.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qx.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://ip.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://bh.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dt.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://nc.521024.cn

Ruby: JSON.parse(s)
来源：http://kh.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lv.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://tc.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gs.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rw.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nz.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rv.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kg.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lc.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://os.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hs.9csxet.cn

[K04] 读取 JSON 文件
来源：http://me.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yw.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ih.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jc.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sp.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://si.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yv.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ad.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kl.yuexingan06.cn

[K05] 深拷贝对象
来源：http://rn.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://gs.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://vd.asd995.cn

JS:   structuredClone(obj)
来源：http://pk.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://as.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://aw.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xp.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uw.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uv.huanxung.cn

[K06] 解析 URL 查询串
来源：http://hf.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pm.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ja.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yu.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://me.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rw.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://im.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fu.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bc.szxytkj.cn

[K07] 进制转换
来源：http://bc.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lg.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yb.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://od.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xc.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hn.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vq.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tg.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bh.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://rv.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://ox.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://if.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://pc.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://zu.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ks.jianghongdianzi.cn

Go:   encoding/gob
来源：http://pe.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://nh.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mt.nszjky.cn

================================================================================
来源：http://xj.asd995.cn

L. 网络请求
来源：http://nu.szsharing.cn

================================================================================
来源：http://yp.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://px.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hm.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ec.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://vl.huanxung.cn

TS:   await fetch(url)
来源：http://uo.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gz.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://ux.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fq.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hd.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://cu.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ad.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ud.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vb.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://td.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kz.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ky.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dg.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xl.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://rq.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qz.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sk.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mo.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cu.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ai.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rq.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qr.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://np.huixiangedu.cn

[L04] 设置超时
来源：http://mf.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://sr.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ut.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oq.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nr.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fz.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mg.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yb.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jg.colortex.cn

[L05] 上传文件（multipart）
来源：http://ul.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zl.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qf.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qs.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rf.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jf.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jv.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lz.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://op.521024.cn

[L06] 解析响应为 JSON
来源：http://ym.shxzskj.cn

Py:   resp.json()
来源：http://ej.asd995.cn

PHP:  json_decode($body, true);
来源：http://tv.szsharing.cn

JS:   await resp.json()
来源：http://zt.huixiangedu.cn

TS:   await resp.json()
来源：http://ez.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ql.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ku.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://lw.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://us.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://dj.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aa.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jc.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://si.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://lo.huanxung.cn

Java: resp.statusCode()
来源：http://wr.521024.cn

Go:   resp.StatusCode
来源：http://kt.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://sh.shxzukj.cn

C#:   (int)resp.StatusCode
来源：http://hi.newstarts.cn

[L08] 并发请求多个地址
来源：http://lr.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dr.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://si.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sc.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wc.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ld.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gt.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ox.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hv.yuntaijiaju.cn

================================================================================
来源：http://rr.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://ie.shxzukj.cn

================================================================================
来源：http://sg.chemitech.net.cn

[M01] 读取命令行参数
来源：http://kh.nicolike.cn

Py:   sys.argv[1:]
来源：http://lh.newstarts.cn

PHP:  $argv;  $argc;
来源：http://xv.nszjky.cn

JS:   process.argv.slice(2)
来源：http://vc.hahajie.cn

TS:   process.argv.slice(2)
来源：http://ms.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://ml.asd995.cn

Go:   os.Args[1:]
来源：http://ak.hnjuh.cn

Ruby: ARGV
来源：http://vk.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://yn.hnjuh.cn

[M02] 读取环境变量
来源：http://mi.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://ay.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vm.asd995.cn

JS:   process.env.HOME
来源：http://er.panjiajie.cn

TS:   process.env.HOME
来源：http://mo.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://bc.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nn.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://iq.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jc.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://wh.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nj.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iy.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ur.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qi.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wj.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kt.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vz.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://nf.hnjuh.cn

[M04] 获取当前工作目录
来源：http://fo.shxzukj.cn

Py:   os.getcwd()
来源：http://dl.nicolike.cn

PHP:  getcwd();
来源：http://yb.bjjhwx.cn

JS:   process.cwd()
来源：http://tu.huanxung.cn

TS:   process.cwd()
来源：http://eo.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://jl.9csxet.cn

Go:   os.Getwd()
来源：http://hc.haigaiapp.cn

Ruby: Dir.pwd
来源：http://zu.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://om.jctech888.com.cn

[M05] 设置退出码
来源：http://hu.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://wq.gzmigu.cn

PHP:  exit(1);
来源：http://oi.lnxyls.cn

JS:   process.exit(1)
来源：http://jc.9csxet.cn

TS:   process.exit(1)
来源：http://ma.szxytkj.cn

Java: System.exit(1)
来源：http://pf.colortex.cn

Go:   os.Exit(1)
来源：http://ci.szsharing.cn

Ruby: exit 1
来源：http://qf.shtwfgs.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ld.haigaiapp.cn

[M06] 向标准错误输出
来源：http://xi.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://jm.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nb.muxihuayi.cn

JS:   console.error("err")
来源：http://dv.haigaiapp.cn

TS:   console.error("err")
来源：http://vg.shtwfgs.cn

Java: System.err.println("err")
来源：http://er.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vw.shtwfgs.cn

Ruby: warn "err"
来源：http://nl.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://td.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://is.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://jm.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ub.bjjhwx.cn

JS:   require.main === module
来源：http://rk.9csxet.cn

TS:   require.main === module
来源：http://ft.szsharing.cn

Java: public static void main(String[] args)
来源：http://gr.hnjuh.cn

Go:   func main()
来源：http://fc.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qz.9csxet.cn

C#:   static void Main(string[] args)
来源：http://aj.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://ow.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://zl.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://rl.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://ja.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://gr.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://om.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://eg.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jo.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ys.shxzukj.cn

================================================================================
来源：http://jl.bjjhwx.cn

N. 数据结构与算法
来源：http://nd.yuexingan06.cn

================================================================================
来源：http://zl.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://kh.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ps.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://im.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ju.bookmarksfly.cn


<!-- 参考信息 -->