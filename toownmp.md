代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cb.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zv.nszjky.cn

[I04] 正则替换
来源：http://cu.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://li.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vq.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://oj.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lg.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://et.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jx.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yp.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tw.chemitech.net.cn

[I05] 按正则拆分
来源：http://xc.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xp.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://as.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://us.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://gj.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://lt.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wd.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wk.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nt.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ry.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ll.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yo.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ar.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bt.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sp.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dv.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fi.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://si.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://ek.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wl.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lm.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sg.shxzskj.cn

TS:   /error/gim
来源：http://bi.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vr.colortex.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://co.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://ti.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bl.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://pa.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fm.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uc.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mo.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fn.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uw.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wi.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tc.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ic.521024.cn

================================================================================
来源：http://kb.hnjuh.cn

J. 日期与时间
来源：http://sf.hahajie.cn

================================================================================
来源：http://fk.shxzukj.cn

[J01] 获取当前时间
来源：http://xk.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gr.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qb.lnxyls.cn

JS:   new Date();  Date.now()
来源：http://zk.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://aa.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uf.yuntaijiaju.cn

Go:   time.Now()
来源：http://bm.hnjuh.cn

Ruby: Time.now
来源：http://tq.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wc.shxzukj.cn

[J02] 格式化输出
来源：http://cp.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ts.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bs.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zk.hnjuh.cn

TS:   d.toISOString()
来源：http://ep.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wz.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ng.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mp.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vw.colortex.cn

[J03] 字符串解析为日期
来源：http://hd.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bd.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aw.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://me.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://zp.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ns.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ou.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://fu.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zm.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://vw.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lb.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ny.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xv.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pf.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jv.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mz.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fu.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aq.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://lq.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://hc.jianghongdianzi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nf.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zl.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lp.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://fr.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ai.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://mm.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sk.9csxet.cn

[J06] 计算两时间之差
来源：http://cm.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://zc.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://rd.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://om.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ii.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gm.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://sf.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://sk.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://zp.shtwfgs.cn

[J07] 比较两个日期
来源：http://pz.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://ov.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ts.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qm.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yo.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fb.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ec.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://th.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://al.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://sp.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nw.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://no.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cg.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xi.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bu.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tq.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sc.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dk.nicolike.cn

[J09] 时区处理
来源：http://zz.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ed.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aj.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ye.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jx.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ii.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aj.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ov.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ql.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://ii.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bq.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ub.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xi.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ap.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ak.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oc.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ca.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nj.wgjwhj.cn

================================================================================
来源：http://rt.chemitech.net.cn

K. JSON 与序列化
来源：http://xn.jctech888.com.cn

================================================================================
来源：http://gh.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://ui.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iu.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bd.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://ns.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://ly.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jm.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://ia.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://on.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yu.newstarts.cn

[K02] JSON 字符串转对象
来源：http://ul.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://rx.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tv.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://lw.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://mi.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mp.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://zr.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://mw.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sy.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://ph.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cc.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nc.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://se.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sx.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vh.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pl.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uo.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yk.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://cf.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rr.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tq.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dm.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vx.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://is.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hf.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://df.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xz.shxzukj.cn

[K05] 深拷贝对象
来源：http://sp.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://cx.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://rb.shxzskj.cn

JS:   structuredClone(obj)
来源：http://sd.9csxet.cn

TS:   structuredClone(obj)
来源：http://od.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ml.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eu.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jv.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vg.colortex.cn

[K06] 解析 URL 查询串
来源：http://uy.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vk.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mn.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://to.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ti.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ap.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://go.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ae.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tu.szxytkj.cn

[K07] 进制转换
来源：http://vs.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dz.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yy.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gm.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ga.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uc.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wo.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iw.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fb.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://zl.asd995.cn

Py:   pickle.dumps(obj)
来源：http://pz.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dv.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://ty.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://ct.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qx.521024.cn

Go:   encoding/gob
来源：http://cy.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://py.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pj.huanxung.cn

================================================================================
来源：http://bc.hahajie.cn

L. 网络请求
来源：http://or.szxytkj.cn

================================================================================
来源：http://ee.newstarts.cn

[L01] 发送 GET 请求
来源：http://kl.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cq.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jt.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://gl.haigaiapp.cn

TS:   await fetch(url)
来源：http://at.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qf.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://xq.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xt.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ic.hahajie.cn

[L02] 发送 POST JSON
来源：http://ep.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cn.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sb.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lq.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cw.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pv.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://io.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gr.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zv.hnjuh.cn

[L03] 设置自定义请求头
来源：http://cd.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xl.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zj.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fi.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bz.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vc.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vj.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rj.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vg.gzmigu.cn

[L04] 设置超时
来源：http://wb.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://zv.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uu.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sz.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kf.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iw.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ax.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://my.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dm.newstarts.cn

[L05] 上传文件（multipart）
来源：http://nk.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ns.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wb.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kh.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nt.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sw.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qa.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ky.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://le.szsharing.cn

[L06] 解析响应为 JSON
来源：http://ux.huixiangedu.cn

Py:   resp.json()
来源：http://cv.hahajie.cn

PHP:  json_decode($body, true);
来源：http://ni.jianghongdianzi.cn

JS:   await resp.json()
来源：http://dm.bjjhwx.cn

TS:   await resp.json()
来源：http://wp.shxzskj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dv.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mk.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://ux.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tg.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://cy.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oj.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pa.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://gr.521024.cn

TS:   resp.ok;  resp.status
来源：http://ge.huanxung.cn

Java: resp.statusCode()
来源：http://lr.nicolike.cn

Go:   resp.StatusCode
来源：http://fu.521024.cn

Ruby: resp.code.to_i
来源：http://pw.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://ox.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://nn.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yz.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://bo.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sy.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kb.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://la.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qh.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kw.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eq.521024.cn

================================================================================
来源：http://ye.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://gx.hnjuh.cn

================================================================================
来源：http://qw.newstarts.cn

[M01] 读取命令行参数
来源：http://qd.nszjky.cn

Py:   sys.argv[1:]
来源：http://ke.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://dd.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://pk.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://sp.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://gw.gzmigu.cn

Go:   os.Args[1:]
来源：http://jz.jianghongdianzi.cn


<!-- 参考信息 -->