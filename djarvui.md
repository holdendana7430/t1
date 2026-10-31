代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://mi.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rt.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://nl.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://xk.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://at.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mm.9csxet.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vl.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aa.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vh.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sr.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sw.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cr.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ne.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://of.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://td.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://em.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vu.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://ac.szxytkj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pu.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fh.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tt.bookmarksfly.cn

TS:   /error/gim
来源：http://ft.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://or.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://br.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://rl.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kl.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://xu.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xn.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://np.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bq.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vs.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qm.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hb.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gm.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kz.bookmarksfly.cn

================================================================================
来源：http://pe.nszjky.cn

J. 日期与时间
来源：http://ll.yuexingan06.cn

================================================================================
来源：http://kf.shtwfgs.cn

[J01] 获取当前时间
来源：http://hp.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qt.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mi.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://oi.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://pl.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xl.muxihuayi.cn

Go:   time.Now()
来源：http://um.shtwfgs.cn

Ruby: Time.now
来源：http://om.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xa.jctech888.com.cn

[J02] 格式化输出
来源：http://st.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jx.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ow.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kb.muxihuayi.cn

TS:   d.toISOString()
来源：http://je.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ik.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bp.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yi.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wi.shxzskj.cn

[J03] 字符串解析为日期
来源：http://ud.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qu.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xe.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://jk.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://sq.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://og.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bp.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://rs.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xz.nicolike.cn

[J04] 时间戳与日期互转
来源：http://jr.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vo.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ps.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://le.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://om.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gg.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mz.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pp.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ky.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://sw.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://il.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kk.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://py.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tq.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://ti.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zi.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://mx.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ee.szsharing.cn

[J06] 计算两时间之差
来源：http://lu.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://qz.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://jn.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vr.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bh.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fa.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://ak.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://xg.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://rx.chemitech.net.cn

[J07] 比较两个日期
来源：http://oa.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://bl.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ad.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ba.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ex.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rm.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fv.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jl.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://gh.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://iv.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pe.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://td.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://my.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pd.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://id.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qd.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ie.bjjhwx.cn

[J09] 时区处理
来源：http://zx.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hl.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sd.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gx.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ip.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qp.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vs.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bz.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qm.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://wp.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rg.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iy.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rg.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ik.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vx.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ob.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gc.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qk.szxytkj.cn

================================================================================
来源：http://le.huanxung.cn

K. JSON 与序列化
来源：http://tj.asd995.cn

================================================================================
来源：http://td.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://pm.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dq.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://of.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://xw.huanxung.cn

TS:   JSON.stringify(obj)
来源：http://bf.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uj.bjjhwx.cn

Go:   json.Marshal(obj)
来源：http://ye.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ys.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kc.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://hk.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://hf.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kt.shxzskj.cn

JS:   JSON.parse(s)
来源：http://sp.szxytkj.cn

TS:   JSON.parse(s)
来源：http://nk.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mz.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://cd.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://zq.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ha.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://ay.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bx.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zf.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://th.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vi.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ws.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xp.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ze.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ys.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://pe.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aw.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://co.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bi.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fm.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lm.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nc.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oz.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sb.shxzukj.cn

[K05] 深拷贝对象
来源：http://pg.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://ff.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://qw.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://un.hnjuh.cn

TS:   structuredClone(obj)
来源：http://rr.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uj.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xh.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lk.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nw.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://so.huixinmuqiang.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ix.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yl.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lr.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qm.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://go.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gk.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vg.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sa.lnxyls.cn

[K07] 进制转换
来源：http://yf.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qq.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gj.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://el.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hk.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bq.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qt.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://de.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://on.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://da.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://qb.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rq.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ee.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://cm.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ch.shtwfgs.cn

Go:   encoding/gob
来源：http://py.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://bq.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tc.bookmarksfly.cn

================================================================================
来源：http://ll.asd995.cn

L. 网络请求
来源：http://wt.yuexingan06.cn

================================================================================
来源：http://fk.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://tb.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cc.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vp.newstarts.cn

JS:   await fetch(url)
来源：http://he.shxzukj.cn

TS:   await fetch(url)
来源：http://ud.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://et.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://vc.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://om.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qf.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://co.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bx.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rp.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dp.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fj.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cf.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eb.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ch.bjjhwx.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ci.huanxung.cn

[L03] 设置自定义请求头
来源：http://ih.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tm.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vs.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xn.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ut.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ax.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dg.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qa.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ss.nszjky.cn

[L04] 设置超时
来源：http://oz.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://xl.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ws.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vf.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qu.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ub.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oi.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bu.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ed.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://tf.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pw.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fr.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cr.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ka.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vc.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bi.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sf.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jb.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://vb.huanxung.cn

Py:   resp.json()
来源：http://cq.szsharing.cn

PHP:  json_decode($body, true);
来源：http://ah.muxihuayi.cn

JS:   await resp.json()
来源：http://pf.chemitech.net.cn

TS:   await resp.json()
来源：http://fw.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wt.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qh.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://dw.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ch.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://nc.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sw.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fz.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://or.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://zv.gzmigu.cn

Java: resp.statusCode()
来源：http://wj.yuexingan06.cn

Go:   resp.StatusCode
来源：http://pb.nszjky.cn

Ruby: resp.code.to_i
来源：http://fd.asd995.cn

C#:   (int)resp.StatusCode
来源：http://nz.huanxung.cn

[L08] 并发请求多个地址
来源：http://zj.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ad.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://al.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wq.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://js.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lb.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lr.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kr.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pj.shtwfgs.cn

================================================================================
来源：http://fd.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://tz.yuntaijiaju.cn

================================================================================
来源：http://gu.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://ng.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://pw.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://bx.nicolike.cn

JS:   process.argv.slice(2)
来源：http://aa.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://ka.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://nl.panjiajie.cn

Go:   os.Args[1:]
来源：http://cn.szsharing.cn

Ruby: ARGV
来源：http://hq.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://yd.muxihuayi.cn

[M02] 读取环境变量
来源：http://fk.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://db.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mv.nszjky.cn

JS:   process.env.HOME
来源：http://ue.hnjuh.cn

TS:   process.env.HOME
来源：http://yu.hnjuh.cn

Java: System.getenv("HOME")
来源：http://em.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://je.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://id.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ug.muxihuayi.cn

[M03] 执行外部命令
来源：http://fs.nszjky.cn


<!-- 参考信息 -->