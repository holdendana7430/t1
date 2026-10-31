代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gj.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gy.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vp.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ye.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ak.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nu.muxihuayi.cn

[I04] 正则替换
来源：http://dy.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ps.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://br.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ye.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kd.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://st.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mq.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ke.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jd.jctech888.com.cn

[I05] 按正则拆分
来源：http://rx.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kx.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://av.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://kw.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://ro.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://mo.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://io.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vn.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ej.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bu.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://df.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dp.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vp.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vv.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gk.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://al.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cd.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xe.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://it.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fk.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zz.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hs.hahajie.cn

TS:   /error/gim
来源：http://kl.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bi.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qo.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://hv.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ex.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://rh.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yf.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://to.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://he.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ob.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cy.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ci.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qn.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dl.bookmarksfly.cn

================================================================================
来源：http://es.huanxung.cn

J. 日期与时间
来源：http://wv.bjjhwx.cn

================================================================================
来源：http://kc.shtwfgs.cn

[J01] 获取当前时间
来源：http://ye.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://le.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kd.nicolike.cn

JS:   new Date();  Date.now()
来源：http://lh.colortex.cn

TS:   new Date();  Date.now()
来源：http://rm.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hj.haigaiapp.cn

Go:   time.Now()
来源：http://mo.hahajie.cn

Ruby: Time.now
来源：http://cw.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yj.hnjuh.cn

[J02] 格式化输出
来源：http://wo.muxihuayi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ak.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lk.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fs.wgjwhj.cn

TS:   d.toISOString()
来源：http://rc.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zo.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cl.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ix.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dv.szsharing.cn

[J03] 字符串解析为日期
来源：http://ea.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ms.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jf.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://mi.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://sg.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pw.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sd.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://jh.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cz.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://gf.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ey.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yr.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://de.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zq.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jc.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://au.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hj.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ur.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://ft.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://za.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cy.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yw.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ap.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://dz.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mv.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://my.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ie.haigaiapp.cn

[J06] 计算两时间之差
来源：http://uk.colortex.cn

Py:   (end - start).total_seconds()
来源：http://al.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://cs.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ft.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ef.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://st.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://xv.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://nc.521024.cn

C#:   (end - start).TotalSeconds
来源：http://lm.huanxung.cn

[J07] 比较两个日期
来源：http://gz.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://ns.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fo.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nj.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://as.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ld.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tr.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pi.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://mh.panjiajie.cn

[J08] 提取年月日与星期
来源：http://uv.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://df.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sv.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fw.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://km.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pi.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uu.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qg.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lw.panjiajie.cn

[J09] 时区处理
来源：http://dc.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ji.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wd.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ft.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kz.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ba.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wp.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yb.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dl.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://kt.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zu.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ri.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tl.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jv.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vx.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lr.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nd.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xv.newstarts.cn

================================================================================
来源：http://hw.bookmarksfly.cn

K. JSON 与序列化
来源：http://dq.shxzukj.cn

================================================================================
来源：http://qy.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://ha.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rf.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pd.asd995.cn

JS:   JSON.stringify(obj)
来源：http://gd.asd995.cn

TS:   JSON.stringify(obj)
来源：http://ap.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cx.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://ze.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qg.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fr.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://fw.bookmarksfly.cn

Py:   json.loads(s)
来源：http://pi.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jj.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://ns.huanxung.cn

TS:   JSON.parse(s)
来源：http://ui.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kb.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://ks.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://ub.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dz.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://et.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xb.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hk.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wk.szxytkj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pr.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ow.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mc.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ym.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xg.hahajie.cn

[K04] 读取 JSON 文件
来源：http://yg.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mi.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ui.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://br.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jh.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pc.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lb.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://go.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jw.nszjky.cn

[K05] 深拷贝对象
来源：http://gv.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://vo.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://fk.lnxyls.cn

JS:   structuredClone(obj)
来源：http://et.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://wl.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kx.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sx.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dr.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cl.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://hh.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tq.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tk.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://un.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cr.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vm.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fy.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mx.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ti.nszjky.cn

[K07] 进制转换
来源：http://lj.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nr.chemitech.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://su.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pw.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oj.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xj.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gf.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zq.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ss.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://vq.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://jj.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nl.szsharing.cn

JS:   v8.serialize(obj)        // Node
来源：http://lp.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ah.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qb.chemitech.net.cn

Go:   encoding/gob
来源：http://wl.521024.cn

Ruby: Marshal.dump(obj)
来源：http://tw.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ed.nszjky.cn

================================================================================
来源：http://ht.panjiajie.cn

L. 网络请求
来源：http://go.jctech888.com.cn

================================================================================
来源：http://da.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://zr.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uz.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://et.shtwfgs.cn

JS:   await fetch(url)
来源：http://wd.szxytkj.cn

TS:   await fetch(url)
来源：http://lp.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oh.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://eb.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kk.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nn.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://rb.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://av.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nr.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zx.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://el.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://et.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sr.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iq.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ad.gzmigu.cn

[L03] 设置自定义请求头
来源：http://du.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oj.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zs.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jx.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yz.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xc.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://go.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fk.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://en.panjiajie.cn

[L04] 设置超时
来源：http://ib.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://it.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xs.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bw.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tg.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fc.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lf.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ew.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cx.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://dh.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rz.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gb.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ek.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nv.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sr.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bx.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ck.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://lg.shxzukj.cn

Py:   resp.json()
来源：http://vj.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://vr.huixiangedu.cn

JS:   await resp.json()
来源：http://qs.haigaiapp.cn

TS:   await resp.json()
来源：http://kk.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ay.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tk.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://qp.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rx.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://zv.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cb.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qi.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://ie.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://ef.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://cx.521024.cn

Go:   resp.StatusCode
来源：http://bb.asd995.cn

Ruby: resp.code.to_i
来源：http://ec.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://cg.hnjuh.cn

[L08] 并发请求多个地址
来源：http://th.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ff.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://bi.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hj.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dm.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yt.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wa.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vx.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://et.shtwfgs.cn

================================================================================
来源：http://vw.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://eu.huixiangedu.cn

================================================================================
来源：http://hs.bjjhwx.cn

[M01] 读取命令行参数
来源：http://jv.gzmigu.cn

Py:   sys.argv[1:]
来源：http://lj.szsharing.cn

PHP:  $argv;  $argc;
来源：http://qt.nszjky.cn


<!-- 参考信息 -->