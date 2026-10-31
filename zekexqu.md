代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://fk.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bc.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://pc.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://iu.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://jn.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sr.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ze.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yx.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ox.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hg.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fn.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bp.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zc.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gg.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pf.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pg.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ag.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://vu.bjjhwx.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://er.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tf.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wl.yuntaijiaju.cn

TS:   /error/gim
来源：http://uh.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dt.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gu.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://ya.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gs.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://wy.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lg.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://us.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kx.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uz.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://it.jctech888.com.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ms.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ev.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tz.jianghongdianzi.cn

================================================================================
来源：http://zi.panjiajie.cn

J. 日期与时间
来源：http://kh.shtwfgs.cn

================================================================================
来源：http://mr.yuexingan06.cn

[J01] 获取当前时间
来源：http://kg.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pi.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://st.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://hm.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://bz.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fa.muxihuayi.cn

Go:   time.Now()
来源：http://di.hahajie.cn

Ruby: Time.now
来源：http://id.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nm.bookmarksfly.cn

[J02] 格式化输出
来源：http://ql.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qy.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qf.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://os.muxihuayi.cn

TS:   d.toISOString()
来源：http://ev.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xa.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hv.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bo.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fg.szsharing.cn

[J03] 字符串解析为日期
来源：http://sy.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fp.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ig.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://nl.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://ff.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sp.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://co.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://ps.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zh.huanxung.cn

[J04] 时间戳与日期互转
来源：http://yi.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wv.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tn.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jx.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wr.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sf.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aj.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cy.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wk.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://xu.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://vm.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nw.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://os.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bm.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://hu.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jt.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://jw.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://io.shxzskj.cn

[J06] 计算两时间之差
来源：http://om.asd995.cn

Py:   (end - start).total_seconds()
来源：http://dg.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://ly.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://je.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tf.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bi.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://nd.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://du.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://ah.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://mj.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://fx.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tr.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ga.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gv.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bg.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ix.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://iu.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ne.hahajie.cn

[J08] 提取年月日与星期
来源：http://ud.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hs.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ii.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mx.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://po.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oq.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sk.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qg.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://de.shtwfgs.cn

[J09] 时区处理
来源：http://nn.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zn.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qc.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vn.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rn.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hc.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ns.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jp.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ru.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://kh.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ab.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pc.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lr.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wq.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qu.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ak.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xw.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ke.szsharing.cn

================================================================================
来源：http://qj.huanxung.cn

K. JSON 与序列化
来源：http://qm.newstarts.cn

================================================================================
来源：http://ev.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://vx.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vo.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dp.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://fz.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://iw.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sp.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://cv.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lg.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fi.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://yd.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://zj.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ej.nicolike.cn

JS:   JSON.parse(s)
来源：http://fy.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://ve.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ar.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://gh.newstarts.cn

Ruby: JSON.parse(s)
来源：http://iw.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kt.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ur.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ah.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mj.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yq.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uz.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wg.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iz.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jw.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://al.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://kr.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zs.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ct.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ba.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pq.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oy.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bo.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pi.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sr.hnjuh.cn

[K05] 深拷贝对象
来源：http://zq.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://fk.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://uz.gzmigu.cn

JS:   structuredClone(obj)
来源：http://dt.shxzskj.cn

TS:   structuredClone(obj)
来源：http://ef.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kp.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ig.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pc.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://im.9csxet.cn

[K06] 解析 URL 查询串
来源：http://an.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qh.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gd.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://az.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sb.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kp.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fl.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oe.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rv.521024.cn

[K07] 进制转换
来源：http://eg.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yj.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lr.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yn.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ka.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kx.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yh.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://co.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ei.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://fd.asd995.cn

Py:   pickle.dumps(obj)
来源：http://mo.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://to.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://pe.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://us.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ad.panjiajie.cn

Go:   encoding/gob
来源：http://xv.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://ne.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gl.muxihuayi.cn

================================================================================
来源：http://bo.hahajie.cn

L. 网络请求
来源：http://iw.521024.cn

================================================================================
来源：http://hx.lnxyls.cn

[L01] 发送 GET 请求
来源：http://uc.newstarts.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bj.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jd.nicolike.cn

JS:   await fetch(url)
来源：http://hj.chemitech.net.cn

TS:   await fetch(url)
来源：http://xy.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zg.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://ol.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pb.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ll.hahajie.cn

[L02] 发送 POST JSON
来源：http://vn.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qo.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qd.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pt.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ld.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ef.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wu.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yx.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wb.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://ps.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bj.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xp.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uf.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sh.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zu.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qn.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ts.colortex.cn

[L04] 设置超时
来源：http://cg.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://xx.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pp.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ss.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://be.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dc.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eo.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nu.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zb.asd995.cn

[L05] 上传文件（multipart）
来源：http://mi.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xg.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wy.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pm.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nt.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mt.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sr.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nu.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bp.newstarts.cn

[L06] 解析响应为 JSON
来源：http://zq.huanxung.cn

Py:   resp.json()
来源：http://tm.521024.cn

PHP:  json_decode($body, true);
来源：http://fq.jctech888.com.cn

JS:   await resp.json()
来源：http://dv.lnxyls.cn

TS:   await resp.json()
来源：http://wd.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yp.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yw.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://dd.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://db.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://zp.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hi.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yk.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://vs.asd995.cn

TS:   resp.ok;  resp.status
来源：http://nd.shxzskj.cn

Java: resp.statusCode()
来源：http://js.shxzskj.cn

Go:   resp.StatusCode
来源：http://xs.huanxung.cn

Ruby: resp.code.to_i
来源：http://bz.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://rh.huanxung.cn

[L08] 并发请求多个地址
来源：http://dy.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uv.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://lu.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://av.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hk.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://of.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fi.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nn.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ni.9csxet.cn

================================================================================
来源：http://iv.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://ze.asd995.cn

================================================================================
来源：http://qx.huixiangedu.cn

[M01] 读取命令行参数
来源：http://wp.shxzukj.cn

Py:   sys.argv[1:]
来源：http://ls.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://bi.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://rs.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://zy.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://su.asd995.cn

Go:   os.Args[1:]
来源：http://jc.hahajie.cn

Ruby: ARGV
来源：http://cf.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://ri.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://lk.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://wd.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vz.lnxyls.cn

JS:   process.env.HOME
来源：http://vk.jctech888.com.cn

TS:   process.env.HOME
来源：http://vx.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://hs.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wi.newstarts.cn

Ruby: ENV["HOME"]
来源：http://eq.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hy.lnxyls.cn

[M03] 执行外部命令
来源：http://pd.gzmigu.cn


<!-- 参考信息 -->