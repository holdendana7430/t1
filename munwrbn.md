代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://bx.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gf.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cc.shtwfgs.cn

[I05] 按正则拆分
来源：http://tx.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xz.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ud.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://nt.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://zl.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://so.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://no.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dz.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ms.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://py.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nb.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ej.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zx.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qz.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ue.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xh.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bn.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ps.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://mw.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ze.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zm.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tg.bookmarksfly.cn

TS:   /error/gim
来源：http://nz.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zb.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qs.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://do.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pr.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://ge.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kp.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cx.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hl.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zs.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://du.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pp.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://je.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zo.bookmarksfly.cn

================================================================================
来源：http://ym.panjiajie.cn

J. 日期与时间
来源：http://sb.haigaiapp.cn

================================================================================
来源：http://cs.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://yd.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cm.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gb.hahajie.cn

JS:   new Date();  Date.now()
来源：http://jt.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://ux.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ln.muxihuayi.cn

Go:   time.Now()
来源：http://mc.lnxyls.cn

Ruby: Time.now
来源：http://ia.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uw.yuexingan06.cn

[J02] 格式化输出
来源：http://aa.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ch.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nr.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sw.hahajie.cn

TS:   d.toISOString()
来源：http://th.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ct.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://is.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ov.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://im.newstarts.cn

[J03] 字符串解析为日期
来源：http://vx.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ee.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pv.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://ih.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://mu.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xd.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gs.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://kl.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xt.colortex.cn

[J04] 时间戳与日期互转
来源：http://qh.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://we.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rx.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ty.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://st.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zn.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jk.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nf.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lq.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://bz.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://yi.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mi.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ho.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ot.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://ec.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nh.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://ns.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sc.chemitech.net.cn

[J06] 计算两时间之差
来源：http://vq.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://kf.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://vb.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ap.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qo.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://th.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://ga.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://xf.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://hj.9csxet.cn

[J07] 比较两个日期
来源：http://vt.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://ch.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://df.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xm.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dt.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ft.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rl.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ac.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://ps.hahajie.cn

[J08] 提取年月日与星期
来源：http://gc.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kw.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tl.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pm.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bg.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qy.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bm.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://on.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://af.yuntaijiaju.cn

[J09] 时区处理
来源：http://sx.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://el.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nz.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aw.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jw.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://at.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gc.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hb.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://np.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://qn.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://be.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ya.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kd.yuexingan06.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ie.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://td.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hv.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ku.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dp.jianghongdianzi.cn

================================================================================
来源：http://wz.huixinmuqiang.cn

K. JSON 与序列化
来源：http://mm.nszjky.cn

================================================================================
来源：http://kk.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://sk.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vu.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lz.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://ve.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://lt.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xh.nicolike.cn

Go:   json.Marshal(obj)
来源：http://bx.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ck.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wn.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://nm.nszjky.cn

Py:   json.loads(s)
来源：http://ga.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zq.szxytkj.cn

JS:   JSON.parse(s)
来源：http://do.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://yf.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://si.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://vf.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://ag.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ut.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://xg.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uh.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fv.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jj.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://na.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fh.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yf.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cx.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ss.colortex.cn

[K04] 读取 JSON 文件
来源：http://dk.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ro.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ld.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gu.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vz.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qz.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vz.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pa.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cb.asd995.cn

[K05] 深拷贝对象
来源：http://gy.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://zs.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://py.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://zl.521024.cn

TS:   structuredClone(obj)
来源：http://ju.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bu.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dn.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zs.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cf.newstarts.cn

[K06] 解析 URL 查询串
来源：http://tt.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://us.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nj.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://se.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mo.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ja.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fg.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vs.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cq.szxytkj.cn

[K07] 进制转换
来源：http://rw.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oe.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://we.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cm.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ch.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eq.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uk.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ey.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vr.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://vp.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://hx.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cf.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://du.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://qo.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hq.jianghongdianzi.cn

Go:   encoding/gob
来源：http://dv.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://ay.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nh.nicolike.cn

================================================================================
来源：http://mq.chemitech.net.cn

L. 网络请求
来源：http://cx.huixiangedu.cn

================================================================================
来源：http://ns.colortex.cn

[L01] 发送 GET 请求
来源：http://xm.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rt.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qi.muxihuayi.cn

JS:   await fetch(url)
来源：http://cg.wgjwhj.cn

TS:   await fetch(url)
来源：http://zx.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cf.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://uv.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ea.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qn.asd995.cn

[L02] 发送 POST JSON
来源：http://th.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ey.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ok.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tk.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sf.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gb.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gg.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pw.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lr.hahajie.cn

[L03] 设置自定义请求头
来源：http://mi.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rv.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pi.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://na.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://px.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kt.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jp.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qi.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://re.szsharing.cn

[L04] 设置超时
来源：http://yw.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://sz.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kb.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mc.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pa.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ni.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aj.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mh.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yb.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://wb.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jj.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dv.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hf.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ew.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yg.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ty.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jn.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dg.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://ei.szsharing.cn

Py:   resp.json()
来源：http://dw.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://gt.yuexingan06.cn

JS:   await resp.json()
来源：http://qx.yuntaijiaju.cn

TS:   await resp.json()
来源：http://yq.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dg.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ia.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://uw.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lk.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://uf.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iv.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ru.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://vg.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://tf.9csxet.cn

Java: resp.statusCode()
来源：http://gs.muxihuayi.cn

Go:   resp.StatusCode
来源：http://ka.newstarts.cn

Ruby: resp.code.to_i
来源：http://hq.colortex.cn

C#:   (int)resp.StatusCode
来源：http://qf.shxzskj.cn

[L08] 并发请求多个地址
来源：http://hj.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pq.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://vb.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lm.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xj.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hr.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xy.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ib.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ra.haigaiapp.cn

================================================================================
来源：http://nu.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://fv.huixinmuqiang.cn

================================================================================
来源：http://sk.bjjhwx.cn

[M01] 读取命令行参数
来源：http://hq.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://ky.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://cr.521024.cn

JS:   process.argv.slice(2)
来源：http://za.szsharing.cn

TS:   process.argv.slice(2)
来源：http://ao.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://kh.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://tx.szsharing.cn

Ruby: ARGV
来源：http://rh.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://mh.bjjhwx.cn

[M02] 读取环境变量
来源：http://zb.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://mc.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xw.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://hk.szxytkj.cn

TS:   process.env.HOME
来源：http://gz.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://nn.nszjky.cn


<!-- 参考信息 -->