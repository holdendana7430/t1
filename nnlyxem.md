代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://zb.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ng.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mv.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nv.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fy.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://md.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://af.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hf.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jj.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ll.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kt.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ve.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ew.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://dw.szxytkj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eu.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yu.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sj.asd995.cn

TS:   /error/gim
来源：http://xq.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vw.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lf.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://wo.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xe.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://nc.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sp.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ko.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fa.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ho.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tj.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vi.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wp.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jx.szsharing.cn

================================================================================
来源：http://pw.panjiajie.cn

J. 日期与时间
来源：http://xc.asd995.cn

================================================================================
来源：http://hb.bjjhwx.cn

[J01] 获取当前时间
来源：http://re.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mx.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ds.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://mx.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://lj.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://an.wgjwhj.cn

Go:   time.Now()
来源：http://pj.szxytkj.cn

Ruby: Time.now
来源：http://sg.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vh.muxihuayi.cn

[J02] 格式化输出
来源：http://ve.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qs.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://if.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sr.hahajie.cn

TS:   d.toISOString()
来源：http://bd.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xw.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dy.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bi.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zm.hnjuh.cn

[J03] 字符串解析为日期
来源：http://gt.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://va.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mm.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://kf.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://hg.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nr.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cr.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://pr.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ql.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://be.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lq.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mp.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iv.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ml.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gm.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jk.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jz.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://be.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://lx.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://vq.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sb.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wn.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hs.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://bc.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ck.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://vh.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dl.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://ju.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://ak.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://ua.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dg.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://iv.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nu.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://yo.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://hq.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://fz.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://fh.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://js.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uk.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ii.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yo.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zp.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jx.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ky.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://ww.521024.cn

[J08] 提取年月日与星期
来源：http://zv.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ju.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xk.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tw.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cy.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nr.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lf.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wx.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tb.jianghongdianzi.cn

[J09] 时区处理
来源：http://aw.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rp.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bl.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pv.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zi.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ie.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cz.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tv.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bc.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://ut.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mb.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gb.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pz.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mr.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nb.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wc.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ca.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rv.szxytkj.cn

================================================================================
来源：http://ud.panjiajie.cn

K. JSON 与序列化
来源：http://jn.newstarts.cn

================================================================================
来源：http://vw.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://jj.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iu.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hw.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://nt.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://mr.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zt.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://pp.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ac.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pb.nszjky.cn

[K02] JSON 字符串转对象
来源：http://wv.9csxet.cn

Py:   json.loads(s)
来源：http://ib.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hx.lnxyls.cn

JS:   JSON.parse(s)
来源：http://xp.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://tq.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://np.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://un.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://qd.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ds.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://fy.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qw.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wk.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ze.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://km.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yb.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oz.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rh.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ch.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://ug.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wy.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bp.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oc.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qk.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eq.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ma.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fn.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ol.szsharing.cn

[K05] 深拷贝对象
来源：http://ic.521024.cn

Py:   copy.deepcopy(obj)
来源：http://yi.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://qb.szxytkj.cn

JS:   structuredClone(obj)
来源：http://mz.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://fn.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://si.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sn.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uv.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vj.newstarts.cn

[K06] 解析 URL 查询串
来源：http://ar.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uq.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yv.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yf.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pj.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dp.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rn.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gn.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://un.chemitech.net.cn

[K07] 进制转换
来源：http://vd.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ez.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kh.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bk.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jx.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cx.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pl.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uo.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wp.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://wp.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://zn.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jz.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://ca.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://be.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qg.szxytkj.cn

Go:   encoding/gob
来源：http://uh.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://oy.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iz.yuexingan06.cn

================================================================================
来源：http://xl.hnjuh.cn

L. 网络请求
来源：http://gg.9csxet.cn

================================================================================
来源：http://dz.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://jv.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://az.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ii.panjiajie.cn

JS:   await fetch(url)
来源：http://oa.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://zf.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ez.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://lf.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oa.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eu.hahajie.cn

[L02] 发送 POST JSON
来源：http://lk.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://go.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xu.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dk.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ha.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xu.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vn.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kr.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://um.panjiajie.cn

[L03] 设置自定义请求头
来源：http://mh.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://st.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yp.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fb.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xk.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sk.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iy.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yt.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bl.wgjwhj.cn

[L04] 设置超时
来源：http://dh.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://fz.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zg.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ik.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hm.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xn.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qi.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cq.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gr.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://un.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hv.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fu.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fz.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jz.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rl.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xo.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ss.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bn.nicolike.cn

[L06] 解析响应为 JSON
来源：http://ni.bjjhwx.cn

Py:   resp.json()
来源：http://px.yuntaijiaju.cn

PHP:  json_decode($body, true);
来源：http://bx.colortex.cn

JS:   await resp.json()
来源：http://yv.newstarts.cn

TS:   await resp.json()
来源：http://em.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jn.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ht.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://gt.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kj.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://lu.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sz.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ev.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://ss.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://pz.huanxung.cn

Java: resp.statusCode()
来源：http://tn.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://wu.lnxyls.cn

Ruby: resp.code.to_i
来源：http://st.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://rh.9csxet.cn

[L08] 并发请求多个地址
来源：http://ek.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://su.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://tk.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lg.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ra.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://go.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wd.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wc.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ho.muxihuayi.cn

================================================================================
来源：http://gy.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://jd.nszjky.cn

================================================================================
来源：http://ug.nicolike.cn

[M01] 读取命令行参数
来源：http://vg.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://du.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://ou.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://jt.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://fr.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://zq.yuexingan06.cn

Go:   os.Args[1:]
来源：http://pa.9csxet.cn

Ruby: ARGV
来源：http://so.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://ox.nicolike.cn

[M02] 读取环境变量
来源：http://vl.521024.cn

Py:   os.environ.get("HOME")
来源：http://mr.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://if.huixiangedu.cn

JS:   process.env.HOME
来源：http://bv.bjjhwx.cn

TS:   process.env.HOME
来源：http://mv.shxzskj.cn

Java: System.getenv("HOME")
来源：http://rl.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qp.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://ys.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://js.haigaiapp.cn

[M03] 执行外部命令
来源：http://sy.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lt.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gy.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jz.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lc.nszjky.cn


<!-- 参考信息 -->