代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://qx.chemitech.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qt.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zy.wgjwhj.cn

[I05] 按正则拆分
来源：http://ny.nszjky.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tc.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nl.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://uy.lnxyls.cn

TS:   s.split(/\s*,\s*/)
来源：http://sa.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://hz.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pt.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fw.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ah.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bi.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bf.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kl.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sn.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://em.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tq.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qi.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iv.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sk.521024.cn

[I07] 忽略大小写与多行模式
来源：http://tm.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ym.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cb.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ai.hnjuh.cn

TS:   /error/gim
来源：http://er.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wk.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ta.521024.cn

Ruby: s.scan(/error/i)
来源：http://iq.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ch.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://kw.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ur.yuntaijiaju.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ch.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://po.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://re.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bu.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://am.szxytkj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://re.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qv.panjiajie.cn

================================================================================
来源：http://lb.gzmigu.cn

J. 日期与时间
来源：http://dy.huanxung.cn

================================================================================
来源：http://vj.bjjhwx.cn

[J01] 获取当前时间
来源：http://pz.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vr.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bg.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://kg.nicolike.cn

TS:   new Date();  Date.now()
来源：http://wa.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kh.szsharing.cn

Go:   time.Now()
来源：http://zw.yuexingan06.cn

Ruby: Time.now
来源：http://ow.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vk.bjjhwx.cn

[J02] 格式化输出
来源：http://ie.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fh.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ls.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wo.asd995.cn

TS:   d.toISOString()
来源：http://bb.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://or.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://km.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lv.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uw.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://ve.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mg.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jj.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://hj.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://lo.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ql.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pt.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://de.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ut.asd995.cn

[J04] 时间戳与日期互转
来源：http://sm.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fe.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kb.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ld.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bc.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dp.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gs.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://op.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bj.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://bo.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://sc.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ur.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tk.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jf.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://va.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hj.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://fm.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pi.huanxung.cn

[J06] 计算两时间之差
来源：http://ps.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://pa.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://jo.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ec.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sh.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://by.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://yp.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://hg.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://yd.hnjuh.cn

[J07] 比较两个日期
来源：http://cj.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://zl.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pi.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wm.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ib.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gk.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gp.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nv.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://kf.hnjuh.cn

[J08] 提取年月日与星期
来源：http://pa.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pz.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nt.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mx.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fx.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pu.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://st.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vv.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oa.huixiangedu.cn

[J09] 时区处理
来源：http://ik.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://un.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kc.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yp.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lj.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dn.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fe.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ag.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qi.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://ei.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qv.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cd.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zx.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://li.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xl.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xe.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zi.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zi.chemitech.net.cn

================================================================================
来源：http://kf.muxihuayi.cn

K. JSON 与序列化
来源：http://wd.jctech888.com.cn

================================================================================
来源：http://bz.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://od.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vk.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kp.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://bc.colortex.cn

TS:   JSON.stringify(obj)
来源：http://eg.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jp.bjjhwx.cn

Go:   json.Marshal(obj)
来源：http://gl.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lp.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zm.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://zk.szxytkj.cn

Py:   json.loads(s)
来源：http://qp.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bg.newstarts.cn

JS:   JSON.parse(s)
来源：http://wd.asd995.cn

TS:   JSON.parse(s)
来源：http://jl.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://su.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://zt.huanxung.cn

Ruby: JSON.parse(s)
来源：http://zr.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ot.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://kw.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zw.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bc.jianghongdianzi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rw.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oj.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ko.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wl.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://at.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://la.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://pa.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zv.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jg.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fy.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mh.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rl.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xd.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jo.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oe.hnjuh.cn

[K05] 深拷贝对象
来源：http://by.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://uc.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://tx.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://bx.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://rg.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://of.hnjuh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kr.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ic.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://md.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://tl.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ut.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uh.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sx.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uo.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ix.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yx.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yv.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ga.szsharing.cn

[K07] 进制转换
来源：http://ru.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sk.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vu.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dr.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ft.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bo.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vx.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ep.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sk.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://cw.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://fg.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mw.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://tw.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://pz.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eu.nicolike.cn

Go:   encoding/gob
来源：http://oq.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://ej.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kh.wgjwhj.cn

================================================================================
来源：http://br.yuexingan06.cn

L. 网络请求
来源：http://ve.hnjuh.cn

================================================================================
来源：http://lk.521024.cn

[L01] 发送 GET 请求
来源：http://qj.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ut.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kn.muxihuayi.cn

JS:   await fetch(url)
来源：http://sl.nszjky.cn

TS:   await fetch(url)
来源：http://ng.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://am.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://au.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rn.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cj.hnjuh.cn

[L02] 发送 POST JSON
来源：http://ep.colortex.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ga.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nl.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://se.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ce.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wv.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://da.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yg.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vt.asd995.cn

[L03] 设置自定义请求头
来源：http://pw.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tu.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pn.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jn.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wc.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nf.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bp.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://td.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://md.521024.cn

[L04] 设置超时
来源：http://wv.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://eh.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wv.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gj.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rw.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mk.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oq.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qn.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ng.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://pg.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gg.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kx.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jp.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gc.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qc.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vg.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gn.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qc.nszjky.cn

[L06] 解析响应为 JSON
来源：http://xl.colortex.cn

Py:   resp.json()
来源：http://ey.huanxung.cn

PHP:  json_decode($body, true);
来源：http://go.9csxet.cn

JS:   await resp.json()
来源：http://yt.huixinmuqiang.cn

TS:   await resp.json()
来源：http://jm.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fh.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vb.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://cj.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ou.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://bi.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qc.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jp.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://en.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://sx.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://ih.nszjky.cn

Go:   resp.StatusCode
来源：http://kh.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://zx.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://jp.szxytkj.cn

[L08] 并发请求多个地址
来源：http://nb.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hu.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://ix.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nj.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rs.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sz.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ek.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://od.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://te.huixiangedu.cn

================================================================================
来源：http://vm.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://qb.colortex.cn

================================================================================
来源：http://no.szxytkj.cn

[M01] 读取命令行参数
来源：http://hq.shxzskj.cn

Py:   sys.argv[1:]
来源：http://yu.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://hn.9csxet.cn

JS:   process.argv.slice(2)
来源：http://mm.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://gg.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://tl.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://ai.yuexingan06.cn

Ruby: ARGV
来源：http://ki.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://kx.wgjwhj.cn

[M02] 读取环境变量
来源：http://tw.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://jh.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pd.lnxyls.cn

JS:   process.env.HOME
来源：http://ox.haigaiapp.cn

TS:   process.env.HOME
来源：http://nn.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://lm.jctech888.com.cn


<!-- 参考信息 -->