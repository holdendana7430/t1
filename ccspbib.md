代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wh.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ya.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nt.nicolike.cn

================================================================================
来源：http://ms.yuntaijiaju.cn

J. 日期与时间
来源：http://ig.shxzukj.cn

================================================================================
来源：http://mr.nicolike.cn

[J01] 获取当前时间
来源：http://fm.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qd.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://er.szsharing.cn

JS:   new Date();  Date.now()
来源：http://gw.asd995.cn

TS:   new Date();  Date.now()
来源：http://cv.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tq.jianghongdianzi.cn

Go:   time.Now()
来源：http://iz.yuexingan06.cn

Ruby: Time.now
来源：http://yy.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qe.nszjky.cn

[J02] 格式化输出
来源：http://cm.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bm.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cq.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zs.panjiajie.cn

TS:   d.toISOString()
来源：http://sb.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qx.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jf.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vb.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://he.huanxung.cn

[J03] 字符串解析为日期
来源：http://ac.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dd.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ja.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://gd.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://lc.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nl.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sx.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://be.521024.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hw.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://un.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ka.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lp.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ig.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fk.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qq.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://of.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ms.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uq.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://jn.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://sn.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://eu.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ll.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ls.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://ny.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://av.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://ze.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xy.nszjky.cn

[J06] 计算两时间之差
来源：http://wq.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://mb.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://ys.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hg.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dk.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yv.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://va.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://uc.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://do.muxihuayi.cn

[J07] 比较两个日期
来源：http://qe.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://kz.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ck.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ly.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ac.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wo.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://br.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ga.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://yt.huanxung.cn

[J08] 提取年月日与星期
来源：http://pq.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rs.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hq.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qu.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ug.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hl.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vw.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ot.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iv.lnxyls.cn

[J09] 时区处理
来源：http://mw.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pm.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yx.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qo.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cg.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ry.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gv.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hp.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://it.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://rn.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jg.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dg.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qs.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pc.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cm.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xk.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://il.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lx.521024.cn

================================================================================
来源：http://dz.muxihuayi.cn

K. JSON 与序列化
来源：http://nv.521024.cn

================================================================================
来源：http://qs.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://wi.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hx.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vx.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://fk.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://us.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jc.9csxet.cn

Go:   json.Marshal(obj)
来源：http://wd.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ym.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rf.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://ew.bjjhwx.cn

Py:   json.loads(s)
来源：http://xg.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rj.lnxyls.cn

JS:   JSON.parse(s)
来源：http://wf.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://tr.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xk.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://mo.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://rj.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gq.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://qq.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sa.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wp.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jv.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ni.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://du.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://im.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dl.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ci.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://fh.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ae.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dz.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lf.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yy.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ae.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cl.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oj.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ow.hnjuh.cn

[K05] 深拷贝对象
来源：http://lo.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://wq.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://jf.hnjuh.cn

JS:   structuredClone(obj)
来源：http://ao.asd995.cn

TS:   structuredClone(obj)
来源：http://kr.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ef.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eb.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wt.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zj.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://xm.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mu.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wn.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://em.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ch.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mk.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://np.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zl.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qd.gzmigu.cn

[K07] 进制转换
来源：http://hi.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iq.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fr.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ux.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zq.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xm.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ui.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qc.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fi.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://zz.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://jg.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gp.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://pr.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://wz.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ge.bjjhwx.cn

Go:   encoding/gob
来源：http://gq.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://yz.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ur.yuntaijiaju.cn

================================================================================
来源：http://fy.chemitech.net.cn

L. 网络请求
来源：http://ki.yuntaijiaju.cn

================================================================================
来源：http://qe.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://tw.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bu.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fc.jctech888.com.cn

JS:   await fetch(url)
来源：http://ie.shxzskj.cn

TS:   await fetch(url)
来源：http://nk.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://md.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://am.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xa.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wh.hahajie.cn

[L02] 发送 POST JSON
来源：http://vc.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jz.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pi.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jw.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ey.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vn.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://am.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nl.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://af.szxytkj.cn

[L03] 设置自定义请求头
来源：http://hp.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gu.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gw.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mz.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bq.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dv.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dn.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ae.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yo.shxzukj.cn

[L04] 设置超时
来源：http://vv.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://mk.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ru.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ja.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tn.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gm.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gs.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cs.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eh.asd995.cn

[L05] 上传文件（multipart）
来源：http://cl.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yf.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mq.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ub.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bv.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aa.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cy.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kf.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://my.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://zs.lnxyls.cn

Py:   resp.json()
来源：http://yl.colortex.cn

PHP:  json_decode($body, true);
来源：http://es.szxytkj.cn

JS:   await resp.json()
来源：http://kl.jctech888.com.cn

TS:   await resp.json()
来源：http://rk.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lu.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wd.yuexingan06.cn

Ruby: JSON.parse(resp.body)
来源：http://xd.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gg.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://vu.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ew.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uh.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://yp.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://ek.szsharing.cn

Java: resp.statusCode()
来源：http://jq.szsharing.cn

Go:   resp.StatusCode
来源：http://mc.gzmigu.cn

Ruby: resp.code.to_i
来源：http://km.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://nb.9csxet.cn

[L08] 并发请求多个地址
来源：http://in.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cs.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://fm.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://es.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eq.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ga.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://el.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lb.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jw.hahajie.cn

================================================================================
来源：http://md.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://iy.asd995.cn

================================================================================
来源：http://xe.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://ax.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://td.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://yd.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://if.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://mr.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://qv.newstarts.cn

Go:   os.Args[1:]
来源：http://pg.yuntaijiaju.cn

Ruby: ARGV
来源：http://pj.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://fa.asd995.cn

[M02] 读取环境变量
来源：http://nd.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://ou.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ub.huixiangedu.cn

JS:   process.env.HOME
来源：http://zn.nicolike.cn

TS:   process.env.HOME
来源：http://dm.hahajie.cn

Java: System.getenv("HOME")
来源：http://oc.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dv.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://bk.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fa.hnjuh.cn

[M03] 执行外部命令
来源：http://bj.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://la.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://me.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jm.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bn.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mc.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gm.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pn.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://dk.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://mp.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://et.shtwfgs.cn

PHP:  getcwd();
来源：http://ks.bjjhwx.cn

JS:   process.cwd()
来源：http://up.szxytkj.cn

TS:   process.cwd()
来源：http://fg.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://dd.szxytkj.cn

Go:   os.Getwd()
来源：http://xk.szsharing.cn

Ruby: Dir.pwd
来源：http://fr.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ti.yuntaijiaju.cn

[M05] 设置退出码
来源：http://oc.shxzskj.cn

Py:   sys.exit(1)
来源：http://kv.shxzskj.cn

PHP:  exit(1);
来源：http://nz.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://ai.huixiangedu.cn

TS:   process.exit(1)
来源：http://ge.yuexingan06.cn

Java: System.exit(1)
来源：http://wn.panjiajie.cn

Go:   os.Exit(1)
来源：http://qx.panjiajie.cn

Ruby: exit 1
来源：http://lr.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jv.wgjwhj.cn

[M06] 向标准错误输出
来源：http://eo.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://vk.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cj.bookmarksfly.cn

JS:   console.error("err")
来源：http://dn.nicolike.cn

TS:   console.error("err")
来源：http://bi.chemitech.net.cn

Java: System.err.println("err")
来源：http://ew.wgjwhj.cn


<!-- 参考信息 -->