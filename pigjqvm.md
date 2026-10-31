代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://cx.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ka.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lb.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gb.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gc.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ui.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zm.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pp.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pj.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hq.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ot.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zk.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wx.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://mg.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xg.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qe.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ly.chemitech.net.cn

TS:   /error/gim
来源：http://ak.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yf.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dr.521024.cn

Ruby: s.scan(/error/i)
来源：http://zt.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oz.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ua.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uj.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://od.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hu.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gl.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nb.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xm.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hw.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tm.colortex.cn

================================================================================
来源：http://bq.szsharing.cn

J. 日期与时间
来源：http://eh.yuexingan06.cn

================================================================================
来源：http://aq.9csxet.cn

[J01] 获取当前时间
来源：http://em.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nt.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://ky.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://kn.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pn.huixinmuqiang.cn

Go:   time.Now()
来源：http://kw.szxytkj.cn

Ruby: Time.now
来源：http://ej.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nd.bjjhwx.cn

[J02] 格式化输出
来源：http://tk.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://of.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dn.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cn.panjiajie.cn

TS:   d.toISOString()
来源：http://dl.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hn.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pp.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dk.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zy.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://fc.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hy.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tq.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://xa.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://tc.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cq.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xs.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://hw.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zk.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://vl.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qk.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mo.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ex.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ye.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jv.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://au.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sh.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qp.521024.cn

[J05] 时间加减（加 7 天）
来源：http://fi.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://wg.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ub.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://su.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://az.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://pm.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wz.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://lf.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hx.szxytkj.cn

[J06] 计算两时间之差
来源：http://tf.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://jv.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://mv.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kh.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sw.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sk.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://oc.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://gl.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://hl.haigaiapp.cn

[J07] 比较两个日期
来源：http://ji.shtwfgs.cn

Py:   d1 < d2;  d1 == d2
来源：http://mg.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dl.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ig.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rt.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ke.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ju.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qb.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://qo.gzmigu.cn

[J08] 提取年月日与星期
来源：http://ch.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zq.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ga.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://og.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gf.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hb.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://br.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xr.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fh.wgjwhj.cn

[J09] 时区处理
来源：http://au.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dk.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tm.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gi.jctech888.com.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ty.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yw.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zp.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kt.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gl.521024.cn

[J10] 取今天 / 本月第一天
来源：http://ov.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gc.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kp.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vc.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vy.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ag.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fu.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mf.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cv.huixiangedu.cn

================================================================================
来源：http://is.newstarts.cn

K. JSON 与序列化
来源：http://sm.jianghongdianzi.cn

================================================================================
来源：http://ml.521024.cn

[K01] 对象转 JSON 字符串
来源：http://aw.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rs.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ev.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://ns.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://zb.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ba.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://uk.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ne.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fw.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://yr.szsharing.cn

Py:   json.loads(s)
来源：http://ic.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jz.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://in.szxytkj.cn

TS:   JSON.parse(s)
来源：http://sz.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://op.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://cs.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://fk.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ia.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ke.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cx.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://im.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ab.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wx.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cw.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oq.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gw.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fc.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://fb.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ky.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hh.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://az.gzmigu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uq.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fz.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ac.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ut.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rn.shtwfgs.cn

[K05] 深拷贝对象
来源：http://ae.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://io.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://qv.gzmigu.cn

JS:   structuredClone(obj)
来源：http://ej.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://bi.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qt.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fe.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pl.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://am.nszjky.cn

[K06] 解析 URL 查询串
来源：http://fd.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vi.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ql.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rc.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dm.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jh.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qc.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nd.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fv.yuexingan06.cn

[K07] 进制转换
来源：http://pr.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ce.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ot.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dw.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qh.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hn.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cd.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vs.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wk.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://sj.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://hg.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jc.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://ga.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://qm.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jb.lnxyls.cn

Go:   encoding/gob
来源：http://lv.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://kt.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://im.shtwfgs.cn

================================================================================
来源：http://cf.jianghongdianzi.cn

L. 网络请求
来源：http://zc.haigaiapp.cn

================================================================================
来源：http://gq.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://sz.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hd.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xc.jctech888.com.cn

JS:   await fetch(url)
来源：http://ki.jctech888.com.cn

TS:   await fetch(url)
来源：http://kl.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pc.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://ce.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nj.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://io.shxzskj.cn

[L02] 发送 POST JSON
来源：http://mt.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vf.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ub.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ea.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yn.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gt.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bj.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rn.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oj.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://pl.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sm.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lx.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ox.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://my.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zc.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vh.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://la.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yg.chemitech.net.cn

[L04] 设置超时
来源：http://je.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://rg.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cn.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hp.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zm.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sy.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bm.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iw.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gw.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://tf.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ao.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lq.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://em.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://av.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zy.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pc.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uv.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xp.newstarts.cn

[L06] 解析响应为 JSON
来源：http://ai.yuntaijiaju.cn

Py:   resp.json()
来源：http://hj.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://dr.yuexingan06.cn

JS:   await resp.json()
来源：http://sy.nicolike.cn

TS:   await resp.json()
来源：http://ha.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kq.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yz.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://zp.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hp.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://gk.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ee.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gx.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://ic.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://xk.huixiangedu.cn

Java: resp.statusCode()
来源：http://fm.asd995.cn

Go:   resp.StatusCode
来源：http://io.shxzukj.cn

Ruby: resp.code.to_i
来源：http://ch.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://qj.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://dm.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nq.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://hh.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zl.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zy.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qj.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fo.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sv.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pj.muxihuayi.cn

================================================================================
来源：http://gu.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://uq.szsharing.cn

================================================================================
来源：http://tb.huixiangedu.cn

[M01] 读取命令行参数
来源：http://kn.lnxyls.cn

Py:   sys.argv[1:]
来源：http://yn.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://nj.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://aa.521024.cn

TS:   process.argv.slice(2)
来源：http://gf.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://rh.9csxet.cn

Go:   os.Args[1:]
来源：http://ck.bookmarksfly.cn

Ruby: ARGV
来源：http://kk.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://in.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://lm.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://gg.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ib.yuexingan06.cn

JS:   process.env.HOME
来源：http://ha.wgjwhj.cn

TS:   process.env.HOME
来源：http://ro.asd995.cn

Java: System.getenv("HOME")
来源：http://xb.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wh.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://mr.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tg.gzmigu.cn

[M03] 执行外部命令
来源：http://mo.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vc.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oj.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zl.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lf.lnxyls.cn


<!-- 参考信息 -->