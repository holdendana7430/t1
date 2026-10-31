代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://da.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gb.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cn.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mw.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rf.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://np.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ee.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pt.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gw.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xf.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://go.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bl.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rt.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://hp.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hs.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pu.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lt.shxzukj.cn

TS:   /error/gim
来源：http://xq.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://if.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bf.colortex.cn

Ruby: s.scan(/error/i)
来源：http://ad.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hn.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://gk.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ar.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dw.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fn.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sx.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ur.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sx.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bn.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://or.yuntaijiaju.cn

================================================================================
来源：http://ee.chemitech.net.cn

J. 日期与时间
来源：http://se.newstarts.cn

================================================================================
来源：http://em.haigaiapp.cn

[J01] 获取当前时间
来源：http://sk.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mp.huanxung.cn

JS:   new Date();  Date.now()
来源：http://rm.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://tk.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jw.bookmarksfly.cn

Go:   time.Now()
来源：http://kk.muxihuayi.cn

Ruby: Time.now
来源：http://hi.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ir.asd995.cn

[J02] 格式化输出
来源：http://mc.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nl.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eh.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qj.bookmarksfly.cn

TS:   d.toISOString()
来源：http://pt.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hx.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tg.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://go.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jj.9csxet.cn

[J03] 字符串解析为日期
来源：http://hr.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bd.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://an.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://fv.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://nz.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xl.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://up.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://kz.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qu.nicolike.cn

[J04] 时间戳与日期互转
来源：http://vu.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rk.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yd.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cq.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dp.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ns.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lx.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pt.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oh.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://cw.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://xs.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uh.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fo.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xc.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://hi.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ip.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://xy.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mr.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://iw.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://mp.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://bn.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kk.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sw.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sw.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://vs.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://cc.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://ek.521024.cn

[J07] 比较两个日期
来源：http://gm.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://ly.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rz.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ho.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dz.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ju.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eq.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://um.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://wz.huanxung.cn

[J08] 提取年月日与星期
来源：http://bz.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ni.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cc.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dj.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vv.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qz.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hq.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ll.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xy.asd995.cn

[J09] 时区处理
来源：http://fp.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zz.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yj.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jq.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sv.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ij.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dg.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mt.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://my.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://zw.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wa.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pk.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qi.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ce.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zn.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dl.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ql.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ex.panjiajie.cn

================================================================================
来源：http://ux.huixiangedu.cn

K. JSON 与序列化
来源：http://wy.asd995.cn

================================================================================
来源：http://dq.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://bi.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://un.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dx.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://oo.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://me.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jj.nszjky.cn

Go:   json.Marshal(obj)
来源：http://fz.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oq.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rw.newstarts.cn

[K02] JSON 字符串转对象
来源：http://ev.panjiajie.cn

Py:   json.loads(s)
来源：http://qe.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kj.szxytkj.cn

JS:   JSON.parse(s)
来源：http://lw.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://qk.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oj.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ln.9csxet.cn

Ruby: JSON.parse(s)
来源：http://ba.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kq.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://yw.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ur.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ox.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ys.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qj.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qf.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xo.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sf.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wo.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://ta.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xn.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yu.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kr.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ie.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://de.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uq.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://an.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kc.haigaiapp.cn

[K05] 深拷贝对象
来源：http://nq.521024.cn

Py:   copy.deepcopy(obj)
来源：http://of.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://uq.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://pp.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://ja.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ej.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wg.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yp.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xm.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://jt.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://if.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mr.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jy.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yd.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jl.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jb.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nb.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ht.bjjhwx.cn

[K07] 进制转换
来源：http://zq.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aj.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nq.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bu.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vm.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ux.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ra.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qh.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dc.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://fc.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://wt.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kd.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://pb.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://zk.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nt.jianghongdianzi.cn

Go:   encoding/gob
来源：http://xq.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://se.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sd.szsharing.cn

================================================================================
来源：http://zy.bjjhwx.cn

L. 网络请求
来源：http://mo.hahajie.cn

================================================================================
来源：http://ry.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://vi.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qy.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://li.szsharing.cn

JS:   await fetch(url)
来源：http://ti.yuexingan06.cn

TS:   await fetch(url)
来源：http://gy.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oy.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://mb.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vl.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://je.shxzukj.cn

[L02] 发送 POST JSON
来源：http://bt.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mw.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ff.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wc.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lm.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ki.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uc.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dk.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ar.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://kd.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qg.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://id.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iu.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vj.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ko.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ah.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://md.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oe.bookmarksfly.cn

[L04] 设置超时
来源：http://js.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://xs.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cc.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pz.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qz.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xt.chemitech.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ty.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bx.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pf.szsharing.cn

[L05] 上传文件（multipart）
来源：http://wm.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://us.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ns.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bu.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ep.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yj.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jq.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ta.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://av.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://uo.muxihuayi.cn

Py:   resp.json()
来源：http://eu.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://pz.yuexingan06.cn

JS:   await resp.json()
来源：http://kr.shxzskj.cn

TS:   await resp.json()
来源：http://ie.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dx.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://py.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://lq.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ph.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://zu.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bv.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cx.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://ah.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://bi.shtwfgs.cn

Java: resp.statusCode()
来源：http://sl.asd995.cn

Go:   resp.StatusCode
来源：http://wg.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://hd.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://ou.huanxung.cn

[L08] 并发请求多个地址
来源：http://er.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ph.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://vx.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sk.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dt.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yc.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qa.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kl.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://co.huixinmuqiang.cn

================================================================================
来源：http://fr.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://xn.jctech888.com.cn

================================================================================
来源：http://ci.shxzskj.cn

[M01] 读取命令行参数
来源：http://xm.shxzskj.cn

Py:   sys.argv[1:]
来源：http://su.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://os.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://or.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://og.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://yw.newstarts.cn

Go:   os.Args[1:]
来源：http://ep.szxytkj.cn

Ruby: ARGV
来源：http://tr.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://pj.chemitech.net.cn

[M02] 读取环境变量
来源：http://mn.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://in.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gs.asd995.cn

JS:   process.env.HOME
来源：http://ln.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://kz.nszjky.cn

Java: System.getenv("HOME")
来源：http://vh.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fl.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://ob.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zr.huanxung.cn

[M03] 执行外部命令
来源：http://ol.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yt.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://on.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mr.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fo.nicolike.cn


<!-- 参考信息 -->