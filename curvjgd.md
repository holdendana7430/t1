代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qi.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pb.shtwfgs.cn

[I04] 正则替换
来源：http://js.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fu.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gq.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ib.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cv.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ne.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uw.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hu.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ah.muxihuayi.cn

[I05] 按正则拆分
来源：http://fo.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://be.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eu.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://yn.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ai.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://qh.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fp.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://za.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pj.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yq.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://et.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hn.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hv.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xt.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rg.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xv.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ja.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mo.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://nx.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ga.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nt.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cy.newstarts.cn

TS:   /error/gim
来源：http://um.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kl.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://al.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://ci.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bk.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://pk.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ni.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gr.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yj.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ru.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wl.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://le.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pg.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ks.haigaiapp.cn

================================================================================
来源：http://xq.jctech888.com.cn

J. 日期与时间
来源：http://vu.shxzskj.cn

================================================================================
来源：http://ep.shtwfgs.cn

[J01] 获取当前时间
来源：http://rx.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://um.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mj.nicolike.cn

JS:   new Date();  Date.now()
来源：http://na.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://ca.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ew.yuntaijiaju.cn

Go:   time.Now()
来源：http://un.shtwfgs.cn

Ruby: Time.now
来源：http://ka.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vj.szxytkj.cn

[J02] 格式化输出
来源：http://fe.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gw.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zl.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pl.jctech888.com.cn

TS:   d.toISOString()
来源：http://cg.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ya.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vb.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lr.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xh.hahajie.cn

[J03] 字符串解析为日期
来源：http://uq.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sf.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nc.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://jh.asd995.cn

TS:   new Date("2024-01-02")
来源：http://vy.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lp.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://np.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://ej.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rs.9csxet.cn

[J04] 时间戳与日期互转
来源：http://at.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ib.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vp.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sd.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ok.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pz.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wt.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jt.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cx.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://pb.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://ne.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ng.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ea.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gj.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://qy.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://as.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://zm.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gl.szxytkj.cn

[J06] 计算两时间之差
来源：http://ko.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://vk.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://rw.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jb.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fw.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fz.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://wm.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://ec.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://zr.chemitech.net.cn

[J07] 比较两个日期
来源：http://bh.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://fx.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gs.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kz.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bo.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://su.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vy.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bf.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://zf.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://lr.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ek.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yx.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gx.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pw.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vz.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vx.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ak.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xt.haigaiapp.cn

[J09] 时区处理
来源：http://xi.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fw.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://de.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ir.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xd.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nf.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://un.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ad.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hf.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://ng.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vx.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ed.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iu.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ah.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vt.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fd.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ey.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ox.muxihuayi.cn

================================================================================
来源：http://fa.wgjwhj.cn

K. JSON 与序列化
来源：http://we.yuntaijiaju.cn

================================================================================
来源：http://bv.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://ix.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ll.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vv.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://jx.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://rk.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oa.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://wn.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zq.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zu.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://hc.muxihuayi.cn

Py:   json.loads(s)
来源：http://tr.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jk.szxytkj.cn

JS:   JSON.parse(s)
来源：http://nk.colortex.cn

TS:   JSON.parse(s)
来源：http://nc.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vw.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://dj.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://lf.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sw.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://wp.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qm.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vo.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qn.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jd.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pj.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oh.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://md.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gi.9csxet.cn

[K04] 读取 JSON 文件
来源：http://su.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vs.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tg.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xh.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qg.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xn.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wn.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vx.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wg.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://ep.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://ol.lnxyls.cn

PHP:  unserialize(serialize($obj));
来源：http://in.shxzskj.cn

JS:   structuredClone(obj)
来源：http://mv.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://uy.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fs.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://az.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://et.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fy.yuexingan06.cn

[K06] 解析 URL 查询串
来源：http://dz.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zy.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sd.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bd.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zk.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gc.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xt.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ir.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://om.shtwfgs.cn

[K07] 进制转换
来源：http://iw.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qb.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ee.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dt.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://of.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rz.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mm.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bx.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xp.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://kd.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://gm.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hm.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://hr.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://ae.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ac.haigaiapp.cn

Go:   encoding/gob
来源：http://ii.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://rz.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ad.shtwfgs.cn

================================================================================
来源：http://fn.huixinmuqiang.cn

L. 网络请求
来源：http://ab.bookmarksfly.cn

================================================================================
来源：http://vl.nszjky.cn

[L01] 发送 GET 请求
来源：http://lh.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ar.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ru.szsharing.cn

JS:   await fetch(url)
来源：http://yd.shtwfgs.cn

TS:   await fetch(url)
来源：http://yq.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xf.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://mk.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bx.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mn.lnxyls.cn

[L02] 发送 POST JSON
来源：http://zf.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sc.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gz.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ip.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fn.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ep.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ph.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jj.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oq.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://su.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yr.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pq.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yx.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pq.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cd.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mp.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ig.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ja.nicolike.cn

[L04] 设置超时
来源：http://cw.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://dc.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yo.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fj.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ta.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ac.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uz.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hb.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gr.asd995.cn

[L05] 上传文件（multipart）
来源：http://ry.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bx.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mp.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zv.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mo.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xq.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pg.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sl.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://if.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://uk.jianghongdianzi.cn

Py:   resp.json()
来源：http://nv.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://nu.gzmigu.cn

JS:   await resp.json()
来源：http://hr.lnxyls.cn

TS:   await resp.json()
来源：http://pk.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://du.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yh.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://zu.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gs.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://di.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gd.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qg.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://ly.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://tk.huanxung.cn

Java: resp.statusCode()
来源：http://sb.521024.cn

Go:   resp.StatusCode
来源：http://pu.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://ll.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://ek.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://pf.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qo.521024.cn

PHP:  curl_multi_init() 系列
来源：http://bd.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yf.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zi.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://va.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hg.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wj.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lt.bookmarksfly.cn

================================================================================
来源：http://id.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://ev.yuntaijiaju.cn

================================================================================
来源：http://kt.shtwfgs.cn

[M01] 读取命令行参数
来源：http://wy.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://zi.hahajie.cn

PHP:  $argv;  $argc;
来源：http://hd.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://zr.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://vl.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://ys.jctech888.com.cn

Go:   os.Args[1:]
来源：http://ih.jianghongdianzi.cn


<!-- 参考信息 -->