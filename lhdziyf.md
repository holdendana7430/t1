代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yl.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yz.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dn.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mc.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gx.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sh.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uo.huixiangedu.cn

[I05] 按正则拆分
来源：http://uw.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wp.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ou.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ne.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://ze.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://zg.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ty.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ir.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://az.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xn.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mm.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sa.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yy.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cx.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wt.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bx.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oa.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wf.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://db.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://te.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lt.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bh.szsharing.cn

TS:   /error/gim
来源：http://ue.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gm.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fq.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://sc.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qw.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://ym.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://io.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gp.shxzukj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zo.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dc.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ev.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cc.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yb.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iu.nszjky.cn

================================================================================
来源：http://yu.colortex.cn

J. 日期与时间
来源：http://sp.wgjwhj.cn

================================================================================
来源：http://fg.huanxung.cn

[J01] 获取当前时间
来源：http://it.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cc.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lv.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://pf.asd995.cn

TS:   new Date();  Date.now()
来源：http://vg.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://oy.bookmarksfly.cn

Go:   time.Now()
来源：http://ek.szxytkj.cn

Ruby: Time.now
来源：http://cm.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vx.yuntaijiaju.cn

[J02] 格式化输出
来源：http://uq.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://do.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nu.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xc.asd995.cn

TS:   d.toISOString()
来源：http://zb.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vp.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pq.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gt.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zh.panjiajie.cn

[J03] 字符串解析为日期
来源：http://om.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gl.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zh.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://ln.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://wt.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://db.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dx.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://mr.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ty.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://ni.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wd.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ru.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oi.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xs.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ia.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lw.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zn.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xp.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://jz.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://ku.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rf.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qw.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sm.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ti.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ar.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://sl.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pj.wgjwhj.cn

[J06] 计算两时间之差
来源：http://hc.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://dn.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://hu.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://je.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ji.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ej.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://gv.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://av.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://ed.521024.cn

[J07] 比较两个日期
来源：http://rs.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://dp.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://at.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gv.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qu.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pv.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sv.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gv.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://pr.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://kv.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hx.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rc.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jc.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iy.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hj.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qt.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uq.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mk.szxytkj.cn

[J09] 时区处理
来源：http://dq.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ax.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jo.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gj.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://at.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ys.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ej.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cj.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vy.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://cm.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ai.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xy.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zf.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uj.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://re.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sk.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fm.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ib.muxihuayi.cn

================================================================================
来源：http://rm.bjjhwx.cn

K. JSON 与序列化
来源：http://va.yuntaijiaju.cn

================================================================================
来源：http://xf.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://yv.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fg.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ju.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://ut.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://am.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xz.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://ds.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vr.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kz.nszjky.cn

[K02] JSON 字符串转对象
来源：http://io.nicolike.cn

Py:   json.loads(s)
来源：http://na.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qr.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://hy.asd995.cn

TS:   JSON.parse(s)
来源：http://zg.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ji.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://vu.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://jx.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bz.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://wr.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tm.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gs.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ex.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://eq.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yl.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qe.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oo.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ir.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://kd.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mf.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://si.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ku.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ax.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sl.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xc.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gx.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jg.huixiangedu.cn

[K05] 深拷贝对象
来源：http://if.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://pr.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://qc.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://rv.panjiajie.cn

TS:   structuredClone(obj)
来源：http://nc.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jv.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dm.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ic.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ig.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://pm.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ha.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://as.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bu.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wi.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xi.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sx.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xp.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ha.shxzukj.cn

[K07] 进制转换
来源：http://nx.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oh.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mh.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vt.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hm.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zx.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vy.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gs.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mk.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://ws.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://kv.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jo.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://ly.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://bk.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xb.wgjwhj.cn

Go:   encoding/gob
来源：http://gj.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://ve.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ve.jctech888.com.cn

================================================================================
来源：http://lc.haigaiapp.cn

L. 网络请求
来源：http://dx.shxzukj.cn

================================================================================
来源：http://te.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://rd.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yo.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ge.9csxet.cn

JS:   await fetch(url)
来源：http://tx.9csxet.cn

TS:   await fetch(url)
来源：http://kf.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ch.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://rm.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rm.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ai.panjiajie.cn

[L02] 发送 POST JSON
来源：http://fj.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zh.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cn.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ib.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://to.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://af.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kb.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sw.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ze.szxytkj.cn

[L03] 设置自定义请求头
来源：http://au.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kf.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wx.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ke.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://du.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vy.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uv.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lk.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kz.bookmarksfly.cn

[L04] 设置超时
来源：http://jh.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://ux.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gz.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ab.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yx.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sb.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dm.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ax.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ti.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://sj.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vi.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://af.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ye.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wy.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ke.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rb.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aw.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gx.huanxung.cn

[L06] 解析响应为 JSON
来源：http://bx.hahajie.cn

Py:   resp.json()
来源：http://us.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://zx.haigaiapp.cn

JS:   await resp.json()
来源：http://jh.shtwfgs.cn

TS:   await resp.json()
来源：http://ft.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://px.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yj.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://ez.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ov.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://kg.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kg.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ln.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://om.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://yc.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://gu.nicolike.cn

Go:   resp.StatusCode
来源：http://lt.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://pp.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://qx.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://wy.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ja.huixinmuqiang.cn

PHP:  curl_multi_init() 系列
来源：http://pf.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yi.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://im.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nx.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hb.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lg.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pm.shtwfgs.cn

================================================================================
来源：http://au.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://kg.haigaiapp.cn

================================================================================
来源：http://tp.asd995.cn

[M01] 读取命令行参数
来源：http://xe.nicolike.cn

Py:   sys.argv[1:]
来源：http://br.521024.cn

PHP:  $argv;  $argc;
来源：http://tg.521024.cn

JS:   process.argv.slice(2)
来源：http://am.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://op.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://gz.521024.cn

Go:   os.Args[1:]
来源：http://oo.hahajie.cn

Ruby: ARGV
来源：http://pt.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://bz.szxytkj.cn

[M02] 读取环境变量
来源：http://fn.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://de.muxihuayi.cn


<!-- 参考信息 -->