代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://oa.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jd.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ps.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://fj.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bt.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zi.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://gn.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://xw.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://jk.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cl.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zm.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pt.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wa.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dv.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oa.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yu.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oo.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ky.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yc.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rz.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vp.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://je.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mx.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cg.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nz.chemitech.net.cn

TS:   /error/gim
来源：http://jd.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pc.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xm.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://dd.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bw.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://rd.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qn.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pp.shxzukj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cr.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oi.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xr.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xn.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://az.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yj.yuntaijiaju.cn

================================================================================
来源：http://ut.szxytkj.cn

J. 日期与时间
来源：http://gx.shxzukj.cn

================================================================================
来源：http://fs.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://gx.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ko.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yv.521024.cn

JS:   new Date();  Date.now()
来源：http://xw.huanxung.cn

TS:   new Date();  Date.now()
来源：http://te.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cs.colortex.cn

Go:   time.Now()
来源：http://xc.huanxung.cn

Ruby: Time.now
来源：http://dq.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ar.521024.cn

[J02] 格式化输出
来源：http://xw.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ti.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://le.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qp.shxzskj.cn

TS:   d.toISOString()
来源：http://hl.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ph.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pp.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dm.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zd.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://yp.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hm.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ki.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://gg.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://fk.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bn.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tq.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://yt.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ss.521024.cn

[J04] 时间戳与日期互转
来源：http://mb.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cl.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yl.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xr.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ja.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wa.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xe.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vd.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yy.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://cw.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://bc.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ag.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ok.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wy.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://au.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://al.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://tc.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hu.huanxung.cn

[J06] 计算两时间之差
来源：http://gi.asd995.cn

Py:   (end - start).total_seconds()
来源：http://pf.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://qw.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cm.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dy.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jo.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://kw.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://th.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://ec.shxzskj.cn

[J07] 比较两个日期
来源：http://pq.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://mh.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jd.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nz.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yo.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kq.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://el.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uu.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://gj.shxzskj.cn

[J08] 提取年月日与星期
来源：http://eh.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mp.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pj.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://az.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bt.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wp.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://de.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bx.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uo.yuntaijiaju.cn

[J09] 时区处理
来源：http://zm.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zo.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fl.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kx.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qr.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://il.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sh.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sn.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fe.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://xk.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rq.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uk.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uw.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bo.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qq.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dd.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yb.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://od.panjiajie.cn

================================================================================
来源：http://dh.colortex.cn

K. JSON 与序列化
来源：http://bt.newstarts.cn

================================================================================
来源：http://oq.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://xa.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tg.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://px.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://ou.huanxung.cn

TS:   JSON.stringify(obj)
来源：http://fb.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ig.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://qu.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hd.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vp.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://mk.szxytkj.cn

Py:   json.loads(s)
来源：http://bt.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yy.nicolike.cn

JS:   JSON.parse(s)
来源：http://ea.hahajie.cn

TS:   JSON.parse(s)
来源：http://gc.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ln.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://lu.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://ij.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qn.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://hf.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qh.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ph.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ww.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cc.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hu.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wg.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qc.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fi.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://zs.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ye.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jf.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sm.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ec.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kp.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jt.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ac.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hd.shxzskj.cn

[K05] 深拷贝对象
来源：http://uf.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://yu.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://kb.shxzukj.cn

JS:   structuredClone(obj)
来源：http://hr.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://kw.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hu.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ml.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cn.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://au.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://up.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ft.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yk.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cl.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pk.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://au.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ec.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wj.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yz.bjjhwx.cn

[K07] 进制转换
来源：http://dv.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xh.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aj.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ls.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tm.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xk.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sp.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vi.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qx.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://lx.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://ud.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wp.521024.cn

JS:   v8.serialize(obj)        // Node
来源：http://dq.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://fc.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cg.szsharing.cn

Go:   encoding/gob
来源：http://hx.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://nr.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cd.nszjky.cn

================================================================================
来源：http://ty.hahajie.cn

L. 网络请求
来源：http://wg.nszjky.cn

================================================================================
来源：http://ui.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://yu.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ky.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qr.nszjky.cn

JS:   await fetch(url)
来源：http://ms.szxytkj.cn

TS:   await fetch(url)
来源：http://xc.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mz.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://mh.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kp.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eg.9csxet.cn

[L02] 发送 POST JSON
来源：http://yj.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://si.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ao.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hu.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ar.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iv.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ci.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xp.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qn.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://xv.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vo.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ry.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hg.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ri.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pc.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bj.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pw.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jd.lnxyls.cn

[L04] 设置超时
来源：http://gb.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://bb.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xj.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lt.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gk.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ea.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pr.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lp.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wa.nicolike.cn

[L05] 上传文件（multipart）
来源：http://at.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://am.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jq.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uh.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sw.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wr.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://of.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mn.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nm.asd995.cn

[L06] 解析响应为 JSON
来源：http://fl.bookmarksfly.cn

Py:   resp.json()
来源：http://cb.newstarts.cn

PHP:  json_decode($body, true);
来源：http://ws.huanxung.cn

JS:   await resp.json()
来源：http://qh.muxihuayi.cn

TS:   await resp.json()
来源：http://kg.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qf.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wk.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://yc.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rq.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://jo.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yu.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qr.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://ka.asd995.cn

TS:   resp.ok;  resp.status
来源：http://zf.szxytkj.cn

Java: resp.statusCode()
来源：http://bz.szsharing.cn

Go:   resp.StatusCode
来源：http://ps.hnjuh.cn

Ruby: resp.code.to_i
来源：http://ly.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://mo.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://zx.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cy.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://qy.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fs.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ud.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://no.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kf.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zj.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eq.shxzskj.cn

================================================================================
来源：http://rc.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://ad.shxzskj.cn

================================================================================
来源：http://pj.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://js.colortex.cn

Py:   sys.argv[1:]
来源：http://wk.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://za.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://sb.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://sg.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://wg.panjiajie.cn

Go:   os.Args[1:]
来源：http://qw.newstarts.cn

Ruby: ARGV
来源：http://fh.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://ko.chemitech.net.cn

[M02] 读取环境变量
来源：http://wr.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://fi.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hf.asd995.cn

JS:   process.env.HOME
来源：http://fc.huixiangedu.cn

TS:   process.env.HOME
来源：http://aj.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://ip.nszjky.cn


<!-- 参考信息 -->