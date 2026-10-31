代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://zg.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pk.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ow.gzmigu.cn

[I05] 按正则拆分
来源：http://mc.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kl.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://am.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://yp.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://ya.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://nc.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qc.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fk.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kr.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ow.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qe.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cj.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uc.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yq.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mx.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jr.jianghongdianzi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jd.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fu.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://px.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jd.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oi.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bi.9csxet.cn

TS:   /error/gim
来源：http://et.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vg.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kk.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://ao.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ae.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://uh.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dh.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ch.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ws.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yc.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ym.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qv.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ly.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cd.muxihuayi.cn

================================================================================
来源：http://ul.shtwfgs.cn

J. 日期与时间
来源：http://fa.huixiangedu.cn

================================================================================
来源：http://bh.9csxet.cn

[J01] 获取当前时间
来源：http://pi.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pv.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zt.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://kr.hahajie.cn

TS:   new Date();  Date.now()
来源：http://zs.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lf.szsharing.cn

Go:   time.Now()
来源：http://yz.9csxet.cn

Ruby: Time.now
来源：http://ko.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hk.wgjwhj.cn

[J02] 格式化输出
来源：http://eb.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://py.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ti.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uw.jctech888.com.cn

TS:   d.toISOString()
来源：http://ku.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uh.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xy.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ag.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gb.panjiajie.cn

[J03] 字符串解析为日期
来源：http://fc.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ah.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yc.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://bc.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://lm.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wc.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pp.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://js.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yw.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://nt.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://le.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sy.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nz.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ln.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ed.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://su.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lv.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ek.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://pk.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://cg.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ga.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bu.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fg.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://bt.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mr.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://bb.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qu.jctech888.com.cn

[J06] 计算两时间之差
来源：http://ba.521024.cn

Py:   (end - start).total_seconds()
来源：http://xp.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://ce.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ml.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://md.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oc.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://vi.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://ym.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://yf.huanxung.cn

[J07] 比较两个日期
来源：http://gy.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://zh.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xu.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bj.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vp.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bp.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uy.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yj.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://xn.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://qq.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://he.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wa.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bi.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jh.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rj.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mn.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nx.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zb.yuntaijiaju.cn

[J09] 时区处理
来源：http://sp.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ae.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wz.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rt.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://at.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tx.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wx.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zo.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nd.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://cc.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://eg.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qn.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sj.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jm.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bd.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ne.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ya.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vo.shxzskj.cn

================================================================================
来源：http://of.colortex.cn

K. JSON 与序列化
来源：http://ep.yuntaijiaju.cn

================================================================================
来源：http://ho.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://bk.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kh.gzmigu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yn.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://ih.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://te.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yp.hahajie.cn

Go:   json.Marshal(obj)
来源：http://gg.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xw.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cp.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://ag.szsharing.cn

Py:   json.loads(s)
来源：http://xw.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xo.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://vd.newstarts.cn

TS:   JSON.parse(s)
来源：http://dj.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nh.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://tx.colortex.cn

Ruby: JSON.parse(s)
来源：http://mw.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yi.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://el.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ws.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xk.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://td.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cr.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://si.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oi.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ro.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bf.szsharing.cn

[K04] 读取 JSON 文件
来源：http://pd.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yo.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wb.szxytkj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://as.gzmigu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://se.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lh.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qv.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://in.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://en.hahajie.cn

[K05] 深拷贝对象
来源：http://mc.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://ta.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://ik.nicolike.cn

JS:   structuredClone(obj)
来源：http://wx.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://fk.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ru.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uv.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pm.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://im.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://cr.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kq.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://je.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hy.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ru.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zu.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fo.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bi.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bp.huixiangedu.cn

[K07] 进制转换
来源：http://fh.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ol.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tq.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://by.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://aa.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://em.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vo.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://it.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://st.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://bs.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://pc.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gh.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://rq.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://sc.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lh.haigaiapp.cn

Go:   encoding/gob
来源：http://cf.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://sx.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tf.jctech888.com.cn

================================================================================
来源：http://eq.huixiangedu.cn

L. 网络请求
来源：http://ah.chemitech.net.cn

================================================================================
来源：http://ae.hnjuh.cn

[L01] 发送 GET 请求
来源：http://ni.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kh.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ba.hnjuh.cn

JS:   await fetch(url)
来源：http://qv.lnxyls.cn

TS:   await fetch(url)
来源：http://oe.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dn.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://dy.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ol.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ym.shxzskj.cn

[L02] 发送 POST JSON
来源：http://ue.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qv.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gr.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jv.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nw.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zi.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gs.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iq.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fn.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://vq.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bn.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mh.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dc.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hs.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://os.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yf.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lt.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wc.szsharing.cn

[L04] 设置超时
来源：http://ib.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://ur.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xu.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://du.jianghongdianzi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qa.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dw.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sl.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mw.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ys.newstarts.cn

[L05] 上传文件（multipart）
来源：http://bf.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oa.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nz.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ch.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ky.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fx.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mv.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tu.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gv.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://pq.szsharing.cn

Py:   resp.json()
来源：http://un.szsharing.cn

PHP:  json_decode($body, true);
来源：http://dy.jctech888.com.cn

JS:   await resp.json()
来源：http://hn.nszjky.cn

TS:   await resp.json()
来源：http://an.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tj.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wv.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://ev.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://da.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://gh.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ih.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ap.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://ly.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://sj.chemitech.net.cn

Java: resp.statusCode()
来源：http://kl.shxzukj.cn

Go:   resp.StatusCode
来源：http://cl.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://nq.colortex.cn

C#:   (int)resp.StatusCode
来源：http://iz.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://ol.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wv.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://cf.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tv.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fi.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pd.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hf.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dr.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yv.chemitech.net.cn

================================================================================
来源：http://bm.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://uh.asd995.cn

================================================================================
来源：http://xm.9csxet.cn

[M01] 读取命令行参数
来源：http://gh.newstarts.cn

Py:   sys.argv[1:]
来源：http://bw.nszjky.cn

PHP:  $argv;  $argc;
来源：http://is.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://xe.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://gm.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://kk.hnjuh.cn

Go:   os.Args[1:]
来源：http://nr.huixinmuqiang.cn

Ruby: ARGV
来源：http://rr.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://gk.nicolike.cn

[M02] 读取环境变量
来源：http://vk.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://xb.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bh.panjiajie.cn

JS:   process.env.HOME
来源：http://ag.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://vn.521024.cn

Java: System.getenv("HOME")
来源：http://iz.nicolike.cn


<!-- 参考信息 -->