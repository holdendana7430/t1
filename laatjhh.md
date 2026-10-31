代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ly.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jh.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tr.nicolike.cn

================================================================================
来源：http://bo.jctech888.com.cn

J. 日期与时间
来源：http://sk.shxzskj.cn

================================================================================
来源：http://lf.hnjuh.cn

[J01] 获取当前时间
来源：http://uh.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ku.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ko.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://kv.nicolike.cn

TS:   new Date();  Date.now()
来源：http://zs.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ol.huixiangedu.cn

Go:   time.Now()
来源：http://gu.newstarts.cn

Ruby: Time.now
来源：http://ds.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ac.gzmigu.cn

[J02] 格式化输出
来源：http://xh.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vg.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://je.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uj.panjiajie.cn

TS:   d.toISOString()
来源：http://ga.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fh.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vi.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://au.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zw.nszjky.cn

[J03] 字符串解析为日期
来源：http://lm.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://da.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vu.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://jh.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://io.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sk.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://il.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://jy.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uv.huanxung.cn

[J04] 时间戳与日期互转
来源：http://wh.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gj.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xl.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rp.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rz.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mo.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tg.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gb.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ne.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://ba.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://lb.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yn.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sd.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oj.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://lt.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jx.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://wv.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wq.bjjhwx.cn

[J06] 计算两时间之差
来源：http://aq.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://ny.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://op.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://il.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://os.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nm.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://od.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://rs.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://vk.muxihuayi.cn

[J07] 比较两个日期
来源：http://rz.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://to.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rh.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://br.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cn.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fo.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ux.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pl.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://jy.shxzskj.cn

[J08] 提取年月日与星期
来源：http://xj.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ww.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://th.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://io.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tf.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qj.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lv.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mn.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ym.shxzskj.cn

[J09] 时区处理
来源：http://yz.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nd.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yp.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pv.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wd.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bt.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rx.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://iv.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lv.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://yx.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rx.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jr.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xm.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uy.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fx.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tm.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kk.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dx.huixinmuqiang.cn

================================================================================
来源：http://ol.hahajie.cn

K. JSON 与序列化
来源：http://wg.wgjwhj.cn

================================================================================
来源：http://we.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://ki.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://of.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rq.521024.cn

JS:   JSON.stringify(obj)
来源：http://cy.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://vm.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wq.asd995.cn

Go:   json.Marshal(obj)
来源：http://ng.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sh.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zt.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://gu.huixiangedu.cn

Py:   json.loads(s)
来源：http://vl.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://so.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://ys.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://uw.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yf.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://jl.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://ts.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ey.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://ux.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xu.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qx.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ec.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ow.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wp.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jr.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sp.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://do.newstarts.cn

[K04] 读取 JSON 文件
来源：http://bz.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qg.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sp.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jb.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zl.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gg.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ra.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ys.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xd.gzmigu.cn

[K05] 深拷贝对象
来源：http://ld.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://ud.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://wg.nszjky.cn

JS:   structuredClone(obj)
来源：http://ei.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://kr.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bb.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dl.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ga.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oa.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://on.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kg.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sh.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ww.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qz.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vc.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hp.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fw.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lc.newstarts.cn

[K07] 进制转换
来源：http://pd.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://np.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://od.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ue.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://th.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tt.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bu.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nr.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ph.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://yw.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://ek.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zw.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://it.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://sg.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vc.huixinmuqiang.cn

Go:   encoding/gob
来源：http://iu.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://jk.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fc.shxzskj.cn

================================================================================
来源：http://gc.haigaiapp.cn

L. 网络请求
来源：http://ow.haigaiapp.cn

================================================================================
来源：http://ql.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://yr.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://on.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bw.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://ry.shtwfgs.cn

TS:   await fetch(url)
来源：http://yy.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gt.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://pq.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sq.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xv.newstarts.cn

[L02] 发送 POST JSON
来源：http://pe.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://re.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vm.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sd.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ya.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lb.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://je.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ev.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://py.gzmigu.cn

[L03] 设置自定义请求头
来源：http://dq.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ln.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qi.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://et.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ag.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bz.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wk.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ed.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vv.nszjky.cn

[L04] 设置超时
来源：http://ih.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://fm.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://af.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rd.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tr.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ho.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ii.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iw.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pb.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://zs.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gf.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oi.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sp.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bm.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ne.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cf.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fg.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rc.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://vu.hnjuh.cn

Py:   resp.json()
来源：http://ek.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://om.wgjwhj.cn

JS:   await resp.json()
来源：http://hq.nszjky.cn

TS:   await resp.json()
来源：http://rh.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bq.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fj.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://pb.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bi.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://gx.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bp.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ux.521024.cn

JS:   resp.ok;  resp.status
来源：http://we.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://ex.colortex.cn

Java: resp.statusCode()
来源：http://il.shxzskj.cn

Go:   resp.StatusCode
来源：http://ug.hnjuh.cn

Ruby: resp.code.to_i
来源：http://qw.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://hk.huanxung.cn

[L08] 并发请求多个地址
来源：http://ub.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lc.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://jl.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fx.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rw.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zj.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uu.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jy.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qq.shxzukj.cn

================================================================================
来源：http://hx.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://tw.nszjky.cn

================================================================================
来源：http://nk.shxzukj.cn

[M01] 读取命令行参数
来源：http://hl.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://dy.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://tp.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://ti.asd995.cn

TS:   process.argv.slice(2)
来源：http://ra.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://yq.521024.cn

Go:   os.Args[1:]
来源：http://wh.chemitech.net.cn

Ruby: ARGV
来源：http://ei.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://sf.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://mj.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://ot.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vi.panjiajie.cn

JS:   process.env.HOME
来源：http://yz.newstarts.cn

TS:   process.env.HOME
来源：http://fp.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://dt.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ip.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://ef.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ke.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://uw.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rj.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xl.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wt.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vf.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hp.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ki.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gm.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://pt.newstarts.cn

[M04] 获取当前工作目录
来源：http://zl.szsharing.cn

Py:   os.getcwd()
来源：http://ya.jianghongdianzi.cn

PHP:  getcwd();
来源：http://ze.huixinmuqiang.cn

JS:   process.cwd()
来源：http://hz.yuexingan06.cn

TS:   process.cwd()
来源：http://by.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://xp.yuexingan06.cn

Go:   os.Getwd()
来源：http://fg.9csxet.cn

Ruby: Dir.pwd
来源：http://vl.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xk.bjjhwx.cn

[M05] 设置退出码
来源：http://oz.panjiajie.cn

Py:   sys.exit(1)
来源：http://ih.jianghongdianzi.cn

PHP:  exit(1);
来源：http://hl.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://ap.huixiangedu.cn

TS:   process.exit(1)
来源：http://fv.lnxyls.cn

Java: System.exit(1)
来源：http://ig.9csxet.cn

Go:   os.Exit(1)
来源：http://jv.hnjuh.cn

Ruby: exit 1
来源：http://hn.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://aw.nicolike.cn

[M06] 向标准错误输出
来源：http://qe.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://km.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ys.bjjhwx.cn

JS:   console.error("err")
来源：http://kq.jctech888.com.cn

TS:   console.error("err")
来源：http://xl.szxytkj.cn

Java: System.err.println("err")
来源：http://nu.nicolike.cn


<!-- 参考信息 -->