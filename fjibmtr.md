代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://ks.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tl.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://sy.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://yh.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://gf.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://go.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dv.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kn.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yq.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jw.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nl.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://up.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sb.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lc.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://me.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pn.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pw.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://wg.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ct.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qd.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wk.nszjky.cn

TS:   /error/gim
来源：http://ms.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hi.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ko.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://wq.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tr.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://rw.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://af.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ml.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yl.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ul.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rh.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://if.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yx.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zc.huanxung.cn

================================================================================
来源：http://fr.wgjwhj.cn

J. 日期与时间
来源：http://jl.shxzskj.cn

================================================================================
来源：http://rv.nicolike.cn

[J01] 获取当前时间
来源：http://en.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jm.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fm.newstarts.cn

JS:   new Date();  Date.now()
来源：http://af.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://bu.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hr.newstarts.cn

Go:   time.Now()
来源：http://lq.bjjhwx.cn

Ruby: Time.now
来源：http://cl.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tf.9csxet.cn

[J02] 格式化输出
来源：http://zu.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kq.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kn.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://po.bookmarksfly.cn

TS:   d.toISOString()
来源：http://gn.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vm.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://by.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://td.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tv.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://vr.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xv.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pi.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://li.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://vn.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vj.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qk.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://gs.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ns.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://op.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mu.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ys.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://we.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://my.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ik.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://en.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://es.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://js.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://rg.521024.cn

Py:   now + timedelta(days=7)
来源：http://pe.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vq.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gk.bookmarksfly.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://js.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://lv.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yk.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://ip.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uo.huixiangedu.cn

[J06] 计算两时间之差
来源：http://uo.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://nu.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://vy.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pb.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://np.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xs.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://mb.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://he.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://eg.9csxet.cn

[J07] 比较两个日期
来源：http://hl.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://mq.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qd.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tr.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://to.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bd.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vt.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yp.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://at.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://zm.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kz.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sc.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tf.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fk.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kq.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fx.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gk.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mk.lnxyls.cn

[J09] 时区处理
来源：http://sf.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hf.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pv.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wk.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ep.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lm.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qy.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ji.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ut.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://qk.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oz.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fu.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zt.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://du.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xv.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bw.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ik.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ki.bookmarksfly.cn

================================================================================
来源：http://pm.szxytkj.cn

K. JSON 与序列化
来源：http://on.chemitech.net.cn

================================================================================
来源：http://sc.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://ac.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ii.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oq.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://xw.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://vc.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wa.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://qo.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gd.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xn.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://gc.szxytkj.cn

Py:   json.loads(s)
来源：http://yh.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hd.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://de.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://qd.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sa.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://mo.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://dd.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dm.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://xu.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fr.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fb.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ir.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cq.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mq.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ld.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vh.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vk.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://fo.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pm.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jg.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aa.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gk.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zg.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://po.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vx.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gq.nszjky.cn

[K05] 深拷贝对象
来源：http://vf.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://qm.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://si.9csxet.cn

JS:   structuredClone(obj)
来源：http://ge.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://qt.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xd.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rq.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dn.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hf.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://bj.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://we.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hn.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://me.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tw.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tc.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://um.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kh.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dp.521024.cn

[K07] 进制转换
来源：http://tv.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ps.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ls.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iw.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sx.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qv.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pl.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ev.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gr.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://jg.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://aj.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ts.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://wn.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://kt.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fu.huanxung.cn

Go:   encoding/gob
来源：http://no.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://hh.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ek.nszjky.cn

================================================================================
来源：http://sf.521024.cn

L. 网络请求
来源：http://dn.huixiangedu.cn

================================================================================
来源：http://bg.shxzskj.cn

[L01] 发送 GET 请求
来源：http://dm.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fx.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ad.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://mf.521024.cn

TS:   await fetch(url)
来源：http://su.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ar.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://dm.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zk.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vw.huanxung.cn

[L02] 发送 POST JSON
来源：http://be.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://oz.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ra.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://at.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qw.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fs.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://md.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mr.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hk.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://zi.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xt.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://up.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vp.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yh.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://op.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ok.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ms.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fh.jctech888.com.cn

[L04] 设置超时
来源：http://tn.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://hj.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dn.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ki.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xj.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ye.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wk.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pp.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kj.hahajie.cn

[L05] 上传文件（multipart）
来源：http://is.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://py.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mm.nszjky.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qy.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eq.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vm.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ud.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zw.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aj.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://rp.lnxyls.cn

Py:   resp.json()
来源：http://ju.huanxung.cn

PHP:  json_decode($body, true);
来源：http://ht.haigaiapp.cn

JS:   await resp.json()
来源：http://rv.shtwfgs.cn

TS:   await resp.json()
来源：http://kf.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://po.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ex.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://gw.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://az.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://bg.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yp.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vt.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://vl.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://xp.colortex.cn

Java: resp.statusCode()
来源：http://jp.wgjwhj.cn

Go:   resp.StatusCode
来源：http://qy.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://cl.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://ht.szxytkj.cn

[L08] 并发请求多个地址
来源：http://th.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://it.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://gi.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zg.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dy.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jy.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dk.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dr.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://di.chemitech.net.cn

================================================================================
来源：http://bm.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://qb.huixinmuqiang.cn

================================================================================
来源：http://ub.shtwfgs.cn

[M01] 读取命令行参数
来源：http://lc.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://dl.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://ra.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://bl.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://rx.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://xo.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://rz.bookmarksfly.cn

Ruby: ARGV
来源：http://ik.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://gu.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://cl.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://if.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fh.huixiangedu.cn

JS:   process.env.HOME
来源：http://yz.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://rb.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://el.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://il.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://kr.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vm.bookmarksfly.cn

[M03] 执行外部命令
来源：http://pc.bookmarksfly.cn


<!-- 参考信息 -->