代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ax.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ug.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qs.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yq.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ux.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xd.gzmigu.cn

[I04] 正则替换
来源：http://xk.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wf.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://po.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ec.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lf.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hq.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://js.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zr.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vs.haigaiapp.cn

[I05] 按正则拆分
来源：http://ob.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yo.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://by.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://si.chemitech.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://iv.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://iu.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nf.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://oy.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gl.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ic.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ai.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bc.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gs.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vt.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sj.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vz.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oz.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://th.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://db.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://to.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gq.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hf.panjiajie.cn

TS:   /error/gim
来源：http://za.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mr.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fa.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://jd.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gz.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://eb.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ho.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tb.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qk.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cb.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kt.nszjky.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sq.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fc.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dd.yuexingan06.cn

================================================================================
来源：http://tq.bjjhwx.cn

J. 日期与时间
来源：http://ur.bjjhwx.cn

================================================================================
来源：http://iu.szsharing.cn

[J01] 获取当前时间
来源：http://ld.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qq.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dt.nszjky.cn

JS:   new Date();  Date.now()
来源：http://sm.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://my.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ms.chemitech.net.cn

Go:   time.Now()
来源：http://kf.szsharing.cn

Ruby: Time.now
来源：http://ad.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dl.gzmigu.cn

[J02] 格式化输出
来源：http://lz.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mn.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xx.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fa.9csxet.cn

TS:   d.toISOString()
来源：http://fs.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ap.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ne.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://so.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pk.hahajie.cn

[J03] 字符串解析为日期
来源：http://cs.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ys.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://va.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://ic.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://bm.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ff.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mh.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://nt.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wu.521024.cn

[J04] 时间戳与日期互转
来源：http://wr.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lb.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bp.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yl.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://af.9csxet.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ud.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nd.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vy.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mk.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://tg.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://os.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://av.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yg.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iq.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://wb.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://er.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://nj.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zy.nszjky.cn

[J06] 计算两时间之差
来源：http://el.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://iz.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://my.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bf.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hu.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ar.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://jv.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://by.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://gg.huanxung.cn

[J07] 比较两个日期
来源：http://um.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://ip.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qt.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rb.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gy.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://td.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dk.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ca.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://fx.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://fq.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ie.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ie.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dr.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bs.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gc.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bi.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qq.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pi.szxytkj.cn

[J09] 时区处理
来源：http://bz.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sd.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ob.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bf.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ko.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ej.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nh.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://km.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lz.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://oy.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cr.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jw.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://em.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zs.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tw.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dc.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yn.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rc.panjiajie.cn

================================================================================
来源：http://bo.hahajie.cn

K. JSON 与序列化
来源：http://re.lnxyls.cn

================================================================================
来源：http://ht.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://rp.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nf.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tk.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://gb.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://we.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://va.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://hy.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qe.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://am.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://fd.bjjhwx.cn

Py:   json.loads(s)
来源：http://sv.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ty.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://uh.szsharing.cn

TS:   JSON.parse(s)
来源：http://xi.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ot.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://cm.newstarts.cn

Ruby: JSON.parse(s)
来源：http://jm.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vo.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://el.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ci.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://va.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://go.szxytkj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cy.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mo.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vh.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ro.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mi.nszjky.cn

[K04] 读取 JSON 文件
来源：http://zw.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sd.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xy.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wi.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cp.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://og.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://al.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rj.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lf.shtwfgs.cn

[K05] 深拷贝对象
来源：http://kh.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://xz.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://ma.panjiajie.cn

JS:   structuredClone(obj)
来源：http://ah.nszjky.cn

TS:   structuredClone(obj)
来源：http://th.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zx.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zo.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ey.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://re.szsharing.cn

[K06] 解析 URL 查询串
来源：http://rp.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pb.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://an.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://to.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sd.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ri.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ns.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ff.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vx.jianghongdianzi.cn

[K07] 进制转换
来源：http://qe.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rs.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gy.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qs.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yb.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oh.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hn.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hd.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://co.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ag.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://jx.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ej.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://ft.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://uy.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gc.nszjky.cn

Go:   encoding/gob
来源：http://ct.bookmarksfly.cn

Ruby: Marshal.dump(obj)
来源：http://ap.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ij.shtwfgs.cn

================================================================================
来源：http://zh.huanxung.cn

L. 网络请求
来源：http://zd.shxzukj.cn

================================================================================
来源：http://rt.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://yf.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ry.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ad.shxzukj.cn

JS:   await fetch(url)
来源：http://mk.muxihuayi.cn

TS:   await fetch(url)
来源：http://wn.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kw.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://hd.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xn.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ku.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://wo.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://np.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ye.wgjwhj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iq.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ri.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ey.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kn.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bx.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lw.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://qq.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iy.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ed.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wc.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iv.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ky.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iv.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gv.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fi.9csxet.cn

[L04] 设置超时
来源：http://wr.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://js.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://or.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xn.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kw.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tb.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://my.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yr.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lb.huanxung.cn

[L05] 上传文件（multipart）
来源：http://nx.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zl.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mf.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gi.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fe.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ll.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://em.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eq.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kd.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://br.huixiangedu.cn

Py:   resp.json()
来源：http://po.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://ne.colortex.cn

JS:   await resp.json()
来源：http://kv.yuntaijiaju.cn

TS:   await resp.json()
来源：http://ou.shxzskj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gd.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ui.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://rh.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vc.521024.cn

[L07] 处理 HTTP 状态码
来源：http://yk.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sw.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zu.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://zi.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://xq.nszjky.cn

Java: resp.statusCode()
来源：http://lh.hnjuh.cn

Go:   resp.StatusCode
来源：http://ou.hahajie.cn

Ruby: resp.code.to_i
来源：http://pf.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://ds.hahajie.cn

[L08] 并发请求多个地址
来源：http://uw.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gz.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://pq.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oe.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bm.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fi.yuntaijiaju.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oe.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xm.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fh.gzmigu.cn

================================================================================
来源：http://gf.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://ft.lnxyls.cn

================================================================================
来源：http://kk.521024.cn

[M01] 读取命令行参数
来源：http://ly.colortex.cn

Py:   sys.argv[1:]
来源：http://on.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://df.haigaiapp.cn


<!-- 参考信息 -->