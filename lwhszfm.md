代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://hx.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ss.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cp.haigaiapp.cn

[I05] 按正则拆分
来源：http://eu.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jd.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://on.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://vz.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ip.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://aj.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oa.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nm.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hk.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nj.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xy.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://av.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ij.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ii.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xl.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mu.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eb.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qj.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://mp.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pa.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cn.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qt.huixiangedu.cn

TS:   /error/gim
来源：http://mi.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://as.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lt.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://xb.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yz.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://na.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ag.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cd.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qp.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ix.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vw.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pt.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vm.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gy.bookmarksfly.cn

================================================================================
来源：http://im.lnxyls.cn

J. 日期与时间
来源：http://bk.wgjwhj.cn

================================================================================
来源：http://ga.newstarts.cn

[J01] 获取当前时间
来源：http://jr.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gw.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dg.nicolike.cn

JS:   new Date();  Date.now()
来源：http://rv.521024.cn

TS:   new Date();  Date.now()
来源：http://pp.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yn.wgjwhj.cn

Go:   time.Now()
来源：http://ij.asd995.cn

Ruby: Time.now
来源：http://fn.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gr.yuexingan06.cn

[J02] 格式化输出
来源：http://xp.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ds.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://du.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oa.shxzskj.cn

TS:   d.toISOString()
来源：http://jp.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mj.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cl.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ze.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jz.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://oi.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tw.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pn.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://kc.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://rv.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uo.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vm.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://nb.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ic.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://am.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://da.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sj.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ii.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hn.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ha.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dn.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hu.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ar.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://ui.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://ql.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bd.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ny.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mp.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://hl.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nq.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://ky.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zl.521024.cn

[J06] 计算两时间之差
来源：http://ti.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://da.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://rh.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qe.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gp.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lj.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://lg.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://ru.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://xe.lnxyls.cn

[J07] 比较两个日期
来源：http://fr.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://cn.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ee.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hi.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fe.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ur.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cv.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wm.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://mr.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://eq.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qk.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pl.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sj.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rp.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qo.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://en.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yz.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lo.haigaiapp.cn

[J09] 时区处理
来源：http://gw.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qr.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yf.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uw.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cn.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zh.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ql.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wf.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pf.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://dp.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ie.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iw.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vh.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zt.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xv.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ln.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gt.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eg.szxytkj.cn

================================================================================
来源：http://jz.asd995.cn

K. JSON 与序列化
来源：http://nd.chemitech.net.cn

================================================================================
来源：http://ji.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://ud.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://im.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://di.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://sp.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://vx.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sp.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://qj.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jg.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yv.nicolike.cn

[K02] JSON 字符串转对象
来源：http://tb.bookmarksfly.cn

Py:   json.loads(s)
来源：http://tp.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xe.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://xe.gzmigu.cn

TS:   JSON.parse(s)
来源：http://pc.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ra.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://cv.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://hx.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qu.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://qx.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kb.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sz.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://es.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ct.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ld.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vv.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ow.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qa.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://fw.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gr.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rw.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mg.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jh.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bj.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ct.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hn.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eh.panjiajie.cn

[K05] 深拷贝对象
来源：http://sf.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://hb.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://lq.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://rg.newstarts.cn

TS:   structuredClone(obj)
来源：http://ve.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kq.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lb.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rs.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wu.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://me.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nn.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zt.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qs.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tl.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uv.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://th.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kd.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hq.521024.cn

[K07] 进制转换
来源：http://lg.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hk.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zb.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nm.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xy.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aj.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sn.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mz.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dt.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://os.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://ix.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nk.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://fu.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://mq.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sd.newstarts.cn

Go:   encoding/gob
来源：http://gw.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://xz.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gt.jctech888.com.cn

================================================================================
来源：http://zw.huanxung.cn

L. 网络请求
来源：http://eg.panjiajie.cn

================================================================================
来源：http://my.lnxyls.cn

[L01] 发送 GET 请求
来源：http://gv.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://id.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vv.asd995.cn

JS:   await fetch(url)
来源：http://kg.nszjky.cn

TS:   await fetch(url)
来源：http://gi.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://da.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://qx.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://im.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wz.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://dp.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ni.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://us.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eu.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sf.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gr.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hr.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bp.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yo.colortex.cn

[L03] 设置自定义请求头
来源：http://gu.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yl.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wc.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lt.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://za.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://om.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pk.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ka.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vy.huixiangedu.cn

[L04] 设置超时
来源：http://im.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://le.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bv.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wc.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wc.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qd.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dn.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sk.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uk.521024.cn

[L05] 上传文件（multipart）
来源：http://th.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bk.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pa.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vf.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gz.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ae.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tv.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ua.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fr.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://fw.huanxung.cn

Py:   resp.json()
来源：http://em.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://iq.asd995.cn

JS:   await resp.json()
来源：http://gx.wgjwhj.cn

TS:   await resp.json()
来源：http://xv.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zk.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://df.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://xh.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zd.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://if.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gf.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://em.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://cu.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://qq.bookmarksfly.cn

Java: resp.statusCode()
来源：http://vc.shtwfgs.cn

Go:   resp.StatusCode
来源：http://qe.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://up.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://fs.hnjuh.cn

[L08] 并发请求多个地址
来源：http://fk.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ay.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://eo.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://im.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ca.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wa.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qx.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dy.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://be.shxzskj.cn

================================================================================
来源：http://jm.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://pl.jianghongdianzi.cn

================================================================================
来源：http://wq.shxzukj.cn

[M01] 读取命令行参数
来源：http://xq.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://dx.huanxung.cn

PHP:  $argv;  $argc;
来源：http://ux.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://wk.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://wj.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://cg.521024.cn

Go:   os.Args[1:]
来源：http://th.shxzukj.cn

Ruby: ARGV
来源：http://wy.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://gi.huixiangedu.cn

[M02] 读取环境变量
来源：http://bi.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://cb.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cr.jctech888.com.cn

JS:   process.env.HOME
来源：http://fa.newstarts.cn

TS:   process.env.HOME
来源：http://hx.hnjuh.cn

Java: System.getenv("HOME")
来源：http://vt.bookmarksfly.cn


<!-- 参考信息 -->