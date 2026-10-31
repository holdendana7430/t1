代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://gc.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://or.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://me.9csxet.cn

[I05] 按正则拆分
来源：http://cj.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ts.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nf.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://fq.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://mj.nicolike.cn

Java: s.split("\\s*,\\s*")
来源：http://qy.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cn.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pj.muxihuayi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ou.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rm.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zr.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bn.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qz.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uq.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pn.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yt.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ww.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mm.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://sl.huanxung.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vx.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kk.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://io.yuntaijiaju.cn

TS:   /error/gim
来源：http://gy.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sz.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vs.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://fx.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xd.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://bq.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ag.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ss.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ou.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bs.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bz.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://db.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qe.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wy.bookmarksfly.cn

================================================================================
来源：http://oa.colortex.cn

J. 日期与时间
来源：http://jo.huanxung.cn

================================================================================
来源：http://hs.nszjky.cn

[J01] 获取当前时间
来源：http://sp.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wh.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qo.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://xk.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://sw.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ye.shxzukj.cn

Go:   time.Now()
来源：http://mb.9csxet.cn

Ruby: Time.now
来源：http://yu.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sw.hahajie.cn

[J02] 格式化输出
来源：http://sm.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gv.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ox.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xf.haigaiapp.cn

TS:   d.toISOString()
来源：http://in.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tt.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jg.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sx.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qg.szxytkj.cn

[J03] 字符串解析为日期
来源：http://nw.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sd.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ah.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://vz.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://nt.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gc.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ng.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://vn.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lg.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://oz.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lx.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yg.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pn.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vb.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://he.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kr.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ow.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kx.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://db.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://lv.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tb.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qz.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ri.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://es.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cu.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://uw.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vf.huanxung.cn

[J06] 计算两时间之差
来源：http://wk.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://uf.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://jg.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ye.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ad.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bp.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://kh.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://mu.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://nj.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://cb.shtwfgs.cn

Py:   d1 < d2;  d1 == d2
来源：http://za.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://od.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xb.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dx.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jn.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nk.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rf.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://nn.nszjky.cn

[J08] 提取年月日与星期
来源：http://zi.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xp.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fg.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://df.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yq.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sc.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ab.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://na.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vn.shxzukj.cn

[J09] 时区处理
来源：http://qn.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ac.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fn.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ke.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jv.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hv.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zs.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://iq.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pv.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://rv.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xu.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zp.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://de.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fa.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bt.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yy.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pi.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fv.muxihuayi.cn

================================================================================
来源：http://ng.panjiajie.cn

K. JSON 与序列化
来源：http://tm.shxzukj.cn

================================================================================
来源：http://zd.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://oa.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vs.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lj.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://qh.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://vq.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mt.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://bi.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hj.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ru.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://ks.lnxyls.cn

Py:   json.loads(s)
来源：http://tm.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gc.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://xv.hnjuh.cn

TS:   JSON.parse(s)
来源：http://kj.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ko.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://ad.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://kl.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gd.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://nx.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ha.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zn.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fp.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jg.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xv.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ew.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ab.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nl.szsharing.cn

[K04] 读取 JSON 文件
来源：http://xu.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xl.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ou.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eu.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hp.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sk.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://au.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mx.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ko.9csxet.cn

[K05] 深拷贝对象
来源：http://uu.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://ic.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://vq.gzmigu.cn

JS:   structuredClone(obj)
来源：http://ik.lnxyls.cn

TS:   structuredClone(obj)
来源：http://di.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fa.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iv.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yc.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yn.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://xf.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jo.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ai.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sb.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ev.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ja.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xg.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ea.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://az.huanxung.cn

[K07] 进制转换
来源：http://ft.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dp.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://br.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fa.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ou.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nr.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://if.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iz.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jv.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://pt.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://sg.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cv.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ka.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://pc.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yf.hahajie.cn

Go:   encoding/gob
来源：http://mm.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://eq.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sy.hnjuh.cn

================================================================================
来源：http://qx.hahajie.cn

L. 网络请求
来源：http://fw.haigaiapp.cn

================================================================================
来源：http://wg.colortex.cn

[L01] 发送 GET 请求
来源：http://af.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fj.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tk.huixiangedu.cn

JS:   await fetch(url)
来源：http://nn.521024.cn

TS:   await fetch(url)
来源：http://xn.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ne.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://jh.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xg.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ic.newstarts.cn

[L02] 发送 POST JSON
来源：http://vp.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ns.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lj.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://td.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sg.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wk.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xp.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gf.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://hy.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dg.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cj.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wt.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://de.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nc.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wt.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dr.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ir.yuntaijiaju.cn

[L04] 设置超时
来源：http://qv.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://bb.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zs.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vm.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://au.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jo.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vf.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yk.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hv.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://br.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tk.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kz.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pr.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ys.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ga.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wd.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cn.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ui.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://vy.bjjhwx.cn

Py:   resp.json()
来源：http://pk.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://yt.chemitech.net.cn

JS:   await resp.json()
来源：http://gu.jianghongdianzi.cn

TS:   await resp.json()
来源：http://mo.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yj.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tg.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://nu.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nm.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://zy.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yr.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://po.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://gz.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://jg.huixiangedu.cn

Java: resp.statusCode()
来源：http://nk.9csxet.cn

Go:   resp.StatusCode
来源：http://gk.shxzukj.cn

Ruby: resp.code.to_i
来源：http://rm.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://yq.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://az.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uc.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://nb.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zq.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dh.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://px.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ku.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://go.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hk.huixinmuqiang.cn

================================================================================
来源：http://fc.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://qk.newstarts.cn

================================================================================
来源：http://al.huixiangedu.cn

[M01] 读取命令行参数
来源：http://iy.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://iz.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://hq.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://bh.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://ln.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://qe.9csxet.cn

Go:   os.Args[1:]
来源：http://bo.shxzskj.cn

Ruby: ARGV
来源：http://np.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://zu.panjiajie.cn

[M02] 读取环境变量
来源：http://vk.asd995.cn

Py:   os.environ.get("HOME")
来源：http://uv.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tg.yuexingan06.cn

JS:   process.env.HOME
来源：http://ip.jctech888.com.cn

TS:   process.env.HOME
来源：http://cy.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://nl.chemitech.net.cn


<!-- 参考信息 -->