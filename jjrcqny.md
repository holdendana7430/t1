代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fa.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jw.wgjwhj.cn

[I04] 正则替换
来源：http://tk.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rs.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qf.szxytkj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://at.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://er.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kg.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pu.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tm.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ni.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://ug.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nh.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wl.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://sp.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://av.bookmarksfly.cn

Java: s.split("\\s*,\\s*")
来源：http://ih.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xf.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gy.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wz.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bm.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oc.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fk.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kq.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vd.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lk.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yp.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gv.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hc.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://wj.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xl.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bt.bjjhwx.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wp.colortex.cn

TS:   /error/gim
来源：http://lo.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ov.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://of.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://ga.szsharing.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rg.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://gt.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gr.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nh.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hr.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://to.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nl.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ty.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oe.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://om.shxzskj.cn

================================================================================
来源：http://lf.szsharing.cn

J. 日期与时间
来源：http://wa.nicolike.cn

================================================================================
来源：http://zw.huixiangedu.cn

[J01] 获取当前时间
来源：http://ah.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xd.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tk.szsharing.cn

JS:   new Date();  Date.now()
来源：http://kq.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://oc.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ee.bjjhwx.cn

Go:   time.Now()
来源：http://zc.521024.cn

Ruby: Time.now
来源：http://pr.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bn.asd995.cn

[J02] 格式化输出
来源：http://to.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kv.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ut.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hf.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://md.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gw.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aw.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ih.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nh.shxzskj.cn

[J03] 字符串解析为日期
来源：http://ti.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ae.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://to.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://zh.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://zm.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jr.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vs.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://gc.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cz.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://rc.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sf.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zs.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aq.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rb.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xv.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zp.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://db.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qp.521024.cn

[J05] 时间加减（加 7 天）
来源：http://mr.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://vt.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://al.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cx.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tf.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://rl.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dx.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://ox.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yi.newstarts.cn

[J06] 计算两时间之差
来源：http://nl.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://eh.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://ax.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xg.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kz.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hd.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://ua.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://ge.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://lp.bjjhwx.cn

[J07] 比较两个日期
来源：http://fm.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://tg.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dx.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ec.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ok.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mo.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dw.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hj.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://hx.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://ao.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://no.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kv.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ei.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ni.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ro.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vt.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qd.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pb.yuexingan06.cn

[J09] 时区处理
来源：http://dq.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wj.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://af.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://al.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ka.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xf.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kf.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yv.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gy.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://qa.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bn.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bo.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qg.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bz.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kt.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qx.shxzukj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ln.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ph.huanxung.cn

================================================================================
来源：http://qf.haigaiapp.cn

K. JSON 与序列化
来源：http://my.bjjhwx.cn

================================================================================
来源：http://sh.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://ug.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jn.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zx.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://ib.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://gm.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://de.9csxet.cn

Go:   json.Marshal(obj)
来源：http://vo.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ws.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xr.colortex.cn

[K02] JSON 字符串转对象
来源：http://kn.wgjwhj.cn

Py:   json.loads(s)
来源：http://ap.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lm.nszjky.cn

JS:   JSON.parse(s)
来源：http://nv.colortex.cn

TS:   JSON.parse(s)
来源：http://pt.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yb.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://jp.newstarts.cn

Ruby: JSON.parse(s)
来源：http://pn.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dq.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://el.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zq.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mb.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xw.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mi.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ix.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://et.521024.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hc.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dr.huanxung.cn

[K04] 读取 JSON 文件
来源：http://lp.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ay.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://em.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vn.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pg.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ai.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oo.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kf.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jc.gzmigu.cn

[K05] 深拷贝对象
来源：http://fj.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://fm.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://td.hnjuh.cn

JS:   structuredClone(obj)
来源：http://hm.panjiajie.cn

TS:   structuredClone(obj)
来源：http://on.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ei.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ro.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://my.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mf.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://kq.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zi.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zg.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hq.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://se.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://su.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lb.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://av.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://to.nicolike.cn

[K07] 进制转换
来源：http://mm.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ik.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kj.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qx.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hd.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://de.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zd.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tm.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ah.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://xy.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://ig.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pe.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://xb.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://dm.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://va.szsharing.cn

Go:   encoding/gob
来源：http://zn.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://xd.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dh.shtwfgs.cn

================================================================================
来源：http://cf.szxytkj.cn

L. 网络请求
来源：http://vc.jianghongdianzi.cn

================================================================================
来源：http://gs.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://uu.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mv.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lc.bjjhwx.cn

JS:   await fetch(url)
来源：http://vg.wgjwhj.cn

TS:   await fetch(url)
来源：http://hb.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://al.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://wo.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ri.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bl.nicolike.cn

[L02] 发送 POST JSON
来源：http://fy.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fe.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ou.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jf.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qs.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://px.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ks.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ny.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sq.shxzskj.cn

[L03] 设置自定义请求头
来源：http://fy.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ii.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gm.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ru.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qh.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pd.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lc.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uq.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hf.huixiangedu.cn

[L04] 设置超时
来源：http://tt.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://ap.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://re.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://or.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bw.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://io.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pa.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wz.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ml.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://ru.9csxet.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jt.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ml.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jl.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yz.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cl.szxytkj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zf.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lh.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iz.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://ik.huanxung.cn

Py:   resp.json()
来源：http://jj.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://rw.shxzukj.cn

JS:   await resp.json()
来源：http://uu.521024.cn

TS:   await resp.json()
来源：http://ds.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zi.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ts.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://jt.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qz.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://pd.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fa.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zj.colortex.cn

JS:   resp.ok;  resp.status
来源：http://jk.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://sx.newstarts.cn

Java: resp.statusCode()
来源：http://xy.hnjuh.cn

Go:   resp.StatusCode
来源：http://rh.colortex.cn

Ruby: resp.code.to_i
来源：http://jg.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://qi.huanxung.cn

[L08] 并发请求多个地址
来源：http://oc.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xq.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://bq.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mj.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aa.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pb.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://li.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xy.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://az.jianghongdianzi.cn

================================================================================
来源：http://kd.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://rh.haigaiapp.cn

================================================================================
来源：http://mv.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://ua.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://vr.hahajie.cn

PHP:  $argv;  $argc;
来源：http://wd.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://oa.huanxung.cn

TS:   process.argv.slice(2)
来源：http://ge.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://bs.jctech888.com.cn

Go:   os.Args[1:]
来源：http://pz.gzmigu.cn


<!-- 参考信息 -->