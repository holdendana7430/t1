代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pk.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tw.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pa.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lf.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lr.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uy.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mn.bjjhwx.cn

[I05] 按正则拆分
来源：http://qs.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ge.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://ue.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://zd.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://di.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ds.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yt.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hx.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zk.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ud.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cn.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ye.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tj.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xx.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wc.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tq.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ps.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://lk.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tk.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wd.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kw.nicolike.cn

TS:   /error/gim
来源：http://xl.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rw.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wd.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://kf.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jh.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://qr.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eu.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ed.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fv.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://na.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mq.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rq.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zi.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tt.gzmigu.cn

================================================================================
来源：http://ej.nszjky.cn

J. 日期与时间
来源：http://ns.wgjwhj.cn

================================================================================
来源：http://zj.bjjhwx.cn

[J01] 获取当前时间
来源：http://yb.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ql.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ua.asd995.cn

JS:   new Date();  Date.now()
来源：http://fj.nicolike.cn

TS:   new Date();  Date.now()
来源：http://tr.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bk.huanxung.cn

Go:   time.Now()
来源：http://sk.huanxung.cn

Ruby: Time.now
来源：http://pt.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yc.huanxung.cn

[J02] 格式化输出
来源：http://xq.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pw.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ry.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://em.muxihuayi.cn

TS:   d.toISOString()
来源：http://mp.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ee.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nd.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qw.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gy.shxzukj.cn

[J03] 字符串解析为日期
来源：http://eh.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qf.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://co.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://nc.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://ww.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://en.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://au.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://xn.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pm.9csxet.cn

[J04] 时间戳与日期互转
来源：http://ar.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cs.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xr.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mj.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bf.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://se.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://py.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kr.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sb.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://qv.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://gm.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sw.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ea.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mf.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://ny.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xd.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://bb.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://de.hahajie.cn

[J06] 计算两时间之差
来源：http://np.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://va.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://xo.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cq.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uo.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lp.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://qj.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://qg.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://rg.nicolike.cn

[J07] 比较两个日期
来源：http://vk.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://lx.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aw.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nz.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tz.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ov.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pb.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yj.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://fa.nszjky.cn

[J08] 提取年月日与星期
来源：http://he.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://es.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://az.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qx.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ad.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xo.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qr.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nf.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rx.yuntaijiaju.cn

[J09] 时区处理
来源：http://jl.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://my.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sy.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ej.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ux.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://id.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://db.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fa.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jc.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://ck.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yx.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dt.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vv.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vl.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zx.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oj.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wu.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lx.nicolike.cn

================================================================================
来源：http://ik.bookmarksfly.cn

K. JSON 与序列化
来源：http://zn.muxihuayi.cn

================================================================================
来源：http://px.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://hr.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hf.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xt.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://vk.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://wx.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ql.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://kk.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tt.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fu.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://ey.shxzukj.cn

Py:   json.loads(s)
来源：http://my.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gd.szxytkj.cn

JS:   JSON.parse(s)
来源：http://fd.hahajie.cn

TS:   JSON.parse(s)
来源：http://yq.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nr.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://ua.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://fb.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sl.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://ai.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vq.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oc.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ye.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ll.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qn.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://us.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wf.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qq.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://jm.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ni.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dc.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lz.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hg.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mh.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zj.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sf.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gp.shxzskj.cn

[K05] 深拷贝对象
来源：http://xr.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://ui.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://dy.521024.cn

JS:   structuredClone(obj)
来源：http://uw.huanxung.cn

TS:   structuredClone(obj)
来源：http://vs.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sg.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qg.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lr.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uk.colortex.cn

[K06] 解析 URL 查询串
来源：http://nk.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iz.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qi.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uv.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mi.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gc.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://aa.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ky.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://um.521024.cn

[K07] 进制转换
来源：http://ux.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jm.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hu.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hm.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mi.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bu.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tp.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ri.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vq.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://ns.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://jy.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zo.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://xl.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://vp.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nb.jctech888.com.cn

Go:   encoding/gob
来源：http://mw.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://uf.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pc.szsharing.cn

================================================================================
来源：http://pv.jctech888.com.cn

L. 网络请求
来源：http://li.colortex.cn

================================================================================
来源：http://bu.gzmigu.cn

[L01] 发送 GET 请求
来源：http://uk.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://er.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://du.chemitech.net.cn

JS:   await fetch(url)
来源：http://za.haigaiapp.cn

TS:   await fetch(url)
来源：http://pr.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qv.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://ii.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vv.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gs.szsharing.cn

[L02] 发送 POST JSON
来源：http://hl.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ap.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qw.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zm.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wc.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jc.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dh.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xh.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ai.nicolike.cn

[L03] 设置自定义请求头
来源：http://un.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mw.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yn.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://he.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xg.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://md.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ba.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gt.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bv.521024.cn

[L04] 设置超时
来源：http://ef.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://rp.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ny.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gm.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kr.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yx.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://it.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qt.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qw.bjjhwx.cn

[L05] 上传文件（multipart）
来源：http://nl.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xg.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ht.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zr.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bj.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mk.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bb.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ng.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ah.asd995.cn

[L06] 解析响应为 JSON
来源：http://fw.wgjwhj.cn

Py:   resp.json()
来源：http://qq.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://tl.colortex.cn

JS:   await resp.json()
来源：http://hy.panjiajie.cn

TS:   await resp.json()
来源：http://gw.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vr.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cs.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://mu.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mv.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://gt.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gl.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gk.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://cg.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://fr.gzmigu.cn

Java: resp.statusCode()
来源：http://it.521024.cn

Go:   resp.StatusCode
来源：http://uy.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://vj.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://qj.szsharing.cn

[L08] 并发请求多个地址
来源：http://hi.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bf.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://ti.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://me.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sz.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ou.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ye.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kp.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xu.newstarts.cn

================================================================================
来源：http://om.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://cz.asd995.cn

================================================================================
来源：http://me.nszjky.cn

[M01] 读取命令行参数
来源：http://ir.huanxung.cn

Py:   sys.argv[1:]
来源：http://ea.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://fj.521024.cn

JS:   process.argv.slice(2)
来源：http://um.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://cf.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://li.9csxet.cn

Go:   os.Args[1:]
来源：http://gu.9csxet.cn

Ruby: ARGV
来源：http://sp.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://vz.newstarts.cn

[M02] 读取环境变量
来源：http://lr.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://yw.haigaiapp.cn


<!-- 参考信息 -->