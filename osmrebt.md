代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ir.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zp.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://da.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://me.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rw.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xl.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gy.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jc.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ds.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://sw.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bj.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xt.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zz.gzmigu.cn

TS:   /error/gim
来源：http://zw.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pv.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zz.colortex.cn

Ruby: s.scan(/error/i)
来源：http://zy.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ka.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://ww.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pg.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fc.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tf.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xq.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ri.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://to.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oc.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bc.asd995.cn

================================================================================
来源：http://gy.jianghongdianzi.cn

J. 日期与时间
来源：http://pe.asd995.cn

================================================================================
来源：http://ef.colortex.cn

[J01] 获取当前时间
来源：http://fd.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://od.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bf.asd995.cn

JS:   new Date();  Date.now()
来源：http://qj.asd995.cn

TS:   new Date();  Date.now()
来源：http://kg.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ul.nicolike.cn

Go:   time.Now()
来源：http://hv.szsharing.cn

Ruby: Time.now
来源：http://yl.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ei.chemitech.net.cn

[J02] 格式化输出
来源：http://eg.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zf.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bn.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mj.bjjhwx.cn

TS:   d.toISOString()
来源：http://kq.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ea.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ss.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://me.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qr.panjiajie.cn

[J03] 字符串解析为日期
来源：http://xd.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ot.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hn.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://xr.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://do.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://di.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lx.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://kj.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nb.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://ri.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ss.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dk.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ib.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bo.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nh.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zy.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qm.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ew.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://fs.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://zt.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://oa.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ec.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xk.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://gw.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://as.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://ku.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://el.szxytkj.cn

[J06] 计算两时间之差
来源：http://rt.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://zh.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://bg.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wg.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lh.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zw.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://tv.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://gr.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://hy.shxzskj.cn

[J07] 比较两个日期
来源：http://au.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://ww.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pm.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mq.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://af.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qw.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dn.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://by.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://to.newstarts.cn

[J08] 提取年月日与星期
来源：http://mt.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qz.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gn.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fc.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ld.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xn.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nt.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://um.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://py.shxzukj.cn

[J09] 时区处理
来源：http://bu.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nn.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mg.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ig.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yf.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jt.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rg.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bb.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jd.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://mw.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gr.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://na.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hx.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xn.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ms.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ax.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sh.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bk.huixiangedu.cn

================================================================================
来源：http://dl.lnxyls.cn

K. JSON 与序列化
来源：http://ej.hahajie.cn

================================================================================
来源：http://gc.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://wk.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gx.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://af.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://ds.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://op.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qy.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://pn.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dk.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://az.huanxung.cn

[K02] JSON 字符串转对象
来源：http://qw.muxihuayi.cn

Py:   json.loads(s)
来源：http://zf.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://au.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://hr.nszjky.cn

TS:   JSON.parse(s)
来源：http://hi.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jg.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ty.huanxung.cn

Ruby: JSON.parse(s)
来源：http://lm.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xp.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://gf.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cb.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jo.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gj.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lq.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zy.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dp.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ax.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kx.newstarts.cn

[K04] 读取 JSON 文件
来源：http://ml.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bx.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qg.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eb.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dt.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jo.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ms.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ht.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pj.bjjhwx.cn

[K05] 深拷贝对象
来源：http://pm.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://gn.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://ja.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://fh.shxzukj.cn

TS:   structuredClone(obj)
来源：http://lk.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tl.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gr.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lv.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nz.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://ta.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tl.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://my.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dt.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rc.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wv.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rl.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yc.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ie.jctech888.com.cn

[K07] 进制转换
来源：http://rh.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vk.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wb.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vq.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ii.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sn.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zv.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ai.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://li.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://wc.colortex.cn

Py:   pickle.dumps(obj)
来源：http://uu.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gn.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://yi.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://wz.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pk.huixiangedu.cn

Go:   encoding/gob
来源：http://rl.521024.cn

Ruby: Marshal.dump(obj)
来源：http://sf.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aw.hnjuh.cn

================================================================================
来源：http://yh.shxzukj.cn

L. 网络请求
来源：http://yf.bookmarksfly.cn

================================================================================
来源：http://ns.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://nd.shxzukj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bp.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ga.panjiajie.cn

JS:   await fetch(url)
来源：http://xe.hnjuh.cn

TS:   await fetch(url)
来源：http://rn.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mn.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://zc.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gb.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jz.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://ob.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yr.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://io.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kg.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://us.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eb.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fq.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://id.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zs.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://bm.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pc.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kb.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://si.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kc.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rb.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jl.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ug.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zh.huixinmuqiang.cn

[L04] 设置超时
来源：http://ka.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://yr.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aq.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yw.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kj.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zb.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fu.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xc.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nl.colortex.cn

[L05] 上传文件（multipart）
来源：http://nm.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ne.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cj.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gl.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ut.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qm.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://be.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bo.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://za.newstarts.cn

[L06] 解析响应为 JSON
来源：http://ey.nicolike.cn

Py:   resp.json()
来源：http://xi.szsharing.cn

PHP:  json_decode($body, true);
来源：http://db.shxzukj.cn

JS:   await resp.json()
来源：http://wn.jctech888.com.cn

TS:   await resp.json()
来源：http://eb.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rr.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uw.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://yg.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cc.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://bj.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ze.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bm.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://jl.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://hj.nicolike.cn

Java: resp.statusCode()
来源：http://iu.szxytkj.cn

Go:   resp.StatusCode
来源：http://yl.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://ul.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://to.hahajie.cn

[L08] 并发请求多个地址
来源：http://yo.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jv.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://uy.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sq.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sc.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vf.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lu.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ta.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qi.jctech888.com.cn

================================================================================
来源：http://of.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://ha.muxihuayi.cn

================================================================================
来源：http://ha.shxzukj.cn

[M01] 读取命令行参数
来源：http://hv.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://dx.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://rh.huanxung.cn

JS:   process.argv.slice(2)
来源：http://ah.hahajie.cn

TS:   process.argv.slice(2)
来源：http://pk.asd995.cn

Java: args 数组（main 方法参数）
来源：http://xr.szsharing.cn

Go:   os.Args[1:]
来源：http://xv.hahajie.cn

Ruby: ARGV
来源：http://jo.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://ka.gzmigu.cn

[M02] 读取环境变量
来源：http://fg.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://tk.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kh.hahajie.cn

JS:   process.env.HOME
来源：http://qt.shxzskj.cn

TS:   process.env.HOME
来源：http://ri.szsharing.cn

Java: System.getenv("HOME")
来源：http://fa.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yt.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://sq.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oe.colortex.cn

[M03] 执行外部命令
来源：http://an.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xe.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aw.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nw.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pa.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eo.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eu.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cz.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://ii.panjiajie.cn


<!-- 参考信息 -->