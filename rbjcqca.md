代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ui.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dl.asd995.cn

[I04] 正则替换
来源：http://yr.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wl.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://of.lnxyls.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ih.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sj.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uf.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fp.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wq.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ms.panjiajie.cn

[I05] 按正则拆分
来源：http://cy.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ei.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ty.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://uh.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://jt.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://ax.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ss.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kt.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ge.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tj.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tt.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bs.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kj.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ep.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bv.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ig.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vk.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gs.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://fl.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ed.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nk.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xj.wgjwhj.cn

TS:   /error/gim
来源：http://ic.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ky.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wv.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://eu.521024.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xf.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://hj.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gr.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vj.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qn.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sg.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://od.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ie.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fp.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qm.hnjuh.cn

================================================================================
来源：http://hy.panjiajie.cn

J. 日期与时间
来源：http://mc.haigaiapp.cn

================================================================================
来源：http://lq.huixiangedu.cn

[J01] 获取当前时间
来源：http://fc.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hg.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oe.asd995.cn

JS:   new Date();  Date.now()
来源：http://vp.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://iw.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yt.chemitech.net.cn

Go:   time.Now()
来源：http://qx.gzmigu.cn

Ruby: Time.now
来源：http://rm.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wl.lnxyls.cn

[J02] 格式化输出
来源：http://lb.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ng.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xf.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oc.lnxyls.cn

TS:   d.toISOString()
来源：http://qe.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sj.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oh.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lz.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wr.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://cv.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jg.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uc.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://mb.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://oj.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jp.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fs.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://qs.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ik.hahajie.cn

[J04] 时间戳与日期互转
来源：http://vc.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jq.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sl.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jj.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cf.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rf.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wc.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jr.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pu.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://yt.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://tr.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://io.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://se.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aj.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://zj.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://id.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://cs.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uc.hnjuh.cn

[J06] 计算两时间之差
来源：http://ut.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://cs.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://ra.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rq.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nv.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nf.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://yh.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://gp.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://ze.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://ru.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://ks.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kn.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kt.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ay.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pr.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kb.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vn.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://db.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://ga.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://it.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ps.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wj.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vl.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kc.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xb.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://si.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bh.colortex.cn

[J09] 时区处理
来源：http://ug.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ko.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yg.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ru.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bg.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://km.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wh.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zq.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xm.521024.cn

[J10] 取今天 / 本月第一天
来源：http://hu.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://en.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qd.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cz.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yo.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ai.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://en.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bv.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yuntaijiaju.cn

================================================================================
来源：http://um.hahajie.cn

K. JSON 与序列化
来源：http://fo.shxzskj.cn

================================================================================
来源：http://qk.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://bz.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mo.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://te.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://om.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://bc.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://it.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://ln.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uz.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bb.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://ny.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://lx.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ql.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://pa.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://ty.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gk.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://xl.9csxet.cn

Ruby: JSON.parse(s)
来源：http://ix.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ai.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://yu.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://od.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://me.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yv.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xx.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eb.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://le.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bw.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pv.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://jr.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qj.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://si.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ue.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sr.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nh.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ks.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ag.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eh.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://nu.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://gq.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://fs.panjiajie.cn

JS:   structuredClone(obj)
来源：http://ph.hnjuh.cn

TS:   structuredClone(obj)
来源：http://te.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gw.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nt.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pk.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dc.colortex.cn

[K06] 解析 URL 查询串
来源：http://wn.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ju.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fg.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ni.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pp.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ot.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://es.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://js.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gr.hnjuh.cn

[K07] 进制转换
来源：http://tx.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vc.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://px.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pc.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gj.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hp.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ew.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tr.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qc.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://xy.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://de.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xu.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://kp.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://jp.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ye.huixinmuqiang.cn

Go:   encoding/gob
来源：http://rm.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://xt.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bf.shtwfgs.cn

================================================================================
来源：http://he.9csxet.cn

L. 网络请求
来源：http://yw.asd995.cn

================================================================================
来源：http://xj.szxytkj.cn

[L01] 发送 GET 请求
来源：http://sw.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gy.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oe.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://wt.wgjwhj.cn

TS:   await fetch(url)
来源：http://by.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jo.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://po.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://iw.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tk.shxzukj.cn

[L02] 发送 POST JSON
来源：http://wr.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lg.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qi.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nu.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://es.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cj.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cr.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hg.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ov.521024.cn

[L03] 设置自定义请求头
来源：http://tv.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://km.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ag.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ly.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nz.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qw.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ek.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zm.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ic.gzmigu.cn

[L04] 设置超时
来源：http://fz.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://je.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://no.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dz.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://te.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gs.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yp.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mw.yuntaijiaju.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vv.nicolike.cn

[L05] 上传文件（multipart）
来源：http://zz.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ff.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ge.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ft.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vo.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bt.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ji.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pj.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kt.newstarts.cn

[L06] 解析响应为 JSON
来源：http://fb.huixinmuqiang.cn

Py:   resp.json()
来源：http://fz.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://rv.huixiangedu.cn

JS:   await resp.json()
来源：http://ff.nszjky.cn

TS:   await resp.json()
来源：http://qt.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uh.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ij.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://ie.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hw.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://vg.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kc.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://il.asd995.cn

JS:   resp.ok;  resp.status
来源：http://np.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://fr.9csxet.cn

Java: resp.statusCode()
来源：http://fj.9csxet.cn

Go:   resp.StatusCode
来源：http://dg.hnjuh.cn

Ruby: resp.code.to_i
来源：http://jy.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://jn.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://dg.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zj.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://wb.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zz.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hy.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jg.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wg.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xs.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dh.hnjuh.cn

================================================================================
来源：http://pd.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://wq.shtwfgs.cn

================================================================================
来源：http://gy.huanxung.cn

[M01] 读取命令行参数
来源：http://pj.gzmigu.cn

Py:   sys.argv[1:]
来源：http://uy.hahajie.cn

PHP:  $argv;  $argc;
来源：http://qe.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://nx.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://gk.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://vf.haigaiapp.cn

Go:   os.Args[1:]
来源：http://sr.colortex.cn


<!-- 参考信息 -->