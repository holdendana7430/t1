代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mc.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kr.huixinmuqiang.cn

[I04] 正则替换
来源：http://bg.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ap.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bi.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ln.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wa.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://td.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://om.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vc.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kc.chemitech.net.cn

[I05] 按正则拆分
来源：http://wh.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://os.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nt.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://qc.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://hf.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://rr.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xu.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xq.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://om.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qh.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rh.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hx.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://su.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vi.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ql.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fs.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lt.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rf.521024.cn

[I07] 忽略大小写与多行模式
来源：http://js.huanxung.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ol.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fu.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vt.nszjky.cn

TS:   /error/gim
来源：http://li.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ii.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://if.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://tp.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://da.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://rj.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vj.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rm.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://os.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lj.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ox.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ag.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bo.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://br.asd995.cn

================================================================================
来源：http://nv.521024.cn

J. 日期与时间
来源：http://fs.newstarts.cn

================================================================================
来源：http://gq.colortex.cn

[J01] 获取当前时间
来源：http://ow.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wh.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zs.nszjky.cn

JS:   new Date();  Date.now()
来源：http://gw.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://hv.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gl.shtwfgs.cn

Go:   time.Now()
来源：http://op.muxihuayi.cn

Ruby: Time.now
来源：http://ir.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uu.9csxet.cn

[J02] 格式化输出
来源：http://ph.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dt.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iy.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gm.bookmarksfly.cn

TS:   d.toISOString()
来源：http://tk.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zy.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fk.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nz.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bi.gzmigu.cn

[J03] 字符串解析为日期
来源：http://sb.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://au.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qg.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://qg.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://ld.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ow.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rq.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://td.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zh.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://al.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://it.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hu.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ze.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ly.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://to.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dt.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nl.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gr.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://cw.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://rq.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://aq.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iq.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ve.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://fs.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oi.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://ln.szsharing.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ij.521024.cn

[J06] 计算两时间之差
来源：http://qw.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://jf.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://nt.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pv.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zw.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xp.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://os.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://ud.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://jm.shxzskj.cn

[J07] 比较两个日期
来源：http://pf.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://yg.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pj.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jl.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fm.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hf.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jt.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pf.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://jc.hnjuh.cn

[J08] 提取年月日与星期
来源：http://fv.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ek.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fh.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://di.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ha.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mr.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wl.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jf.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fv.huixiangedu.cn

[J09] 时区处理
来源：http://yh.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xc.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cb.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rt.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zb.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cd.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fo.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ix.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ki.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://eb.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dv.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vd.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ee.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gp.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vf.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mb.shxzukj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ae.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lg.521024.cn

================================================================================
来源：http://iu.newstarts.cn

K. JSON 与序列化
来源：http://xd.shtwfgs.cn

================================================================================
来源：http://ma.521024.cn

[K01] 对象转 JSON 字符串
来源：http://eb.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gu.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mf.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://jh.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://ky.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://up.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://qr.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vz.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hp.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://cc.newstarts.cn

Py:   json.loads(s)
来源：http://su.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sx.huanxung.cn

JS:   JSON.parse(s)
来源：http://xq.lnxyls.cn

TS:   JSON.parse(s)
来源：http://tt.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bt.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://ah.colortex.cn

Ruby: JSON.parse(s)
来源：http://nz.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yg.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://hi.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bu.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ps.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mo.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yt.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://an.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ql.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qy.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zl.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://om.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dz.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fy.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xt.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ki.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qe.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xx.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ly.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ty.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://kr.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://ul.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://ok.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://vf.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://un.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vu.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kq.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uq.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wn.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://wg.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mx.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://es.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ks.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bn.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rh.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://eh.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cc.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xl.yuexingan06.cn

[K07] 进制转换
来源：http://sw.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ad.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gi.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://di.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ak.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rn.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zx.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://et.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wl.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://ar.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://ym.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vw.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://hv.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://ns.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ob.hahajie.cn

Go:   encoding/gob
来源：http://hu.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://wk.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ka.gzmigu.cn

================================================================================
来源：http://qy.panjiajie.cn

L. 网络请求
来源：http://gj.hnjuh.cn

================================================================================
来源：http://ge.colortex.cn

[L01] 发送 GET 请求
来源：http://gb.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gk.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xj.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://of.shxzskj.cn

TS:   await fetch(url)
来源：http://md.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yh.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://yt.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ty.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dw.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://vu.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nv.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sh.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uz.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nm.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zc.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ei.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hh.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://be.shxzskj.cn

[L03] 设置自定义请求头
来源：http://xp.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ui.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://un.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ql.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zj.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bd.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oa.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fx.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cl.bjjhwx.cn

[L04] 设置超时
来源：http://pr.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://ki.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sy.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lh.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kf.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ol.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lh.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jh.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tl.hahajie.cn

[L05] 上传文件（multipart）
来源：http://yj.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hs.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wh.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zo.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mj.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://px.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bb.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dl.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://he.hahajie.cn

[L06] 解析响应为 JSON
来源：http://gg.9csxet.cn

Py:   resp.json()
来源：http://td.hahajie.cn

PHP:  json_decode($body, true);
来源：http://hg.wgjwhj.cn

JS:   await resp.json()
来源：http://gy.chemitech.net.cn

TS:   await resp.json()
来源：http://nl.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://td.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vb.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://qh.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wk.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://qx.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bo.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ha.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://fw.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://pi.yuexingan06.cn

Java: resp.statusCode()
来源：http://zo.shxzukj.cn

Go:   resp.StatusCode
来源：http://jl.szsharing.cn

Ruby: resp.code.to_i
来源：http://ej.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://sc.shxzukj.cn

[L08] 并发请求多个地址
来源：http://oy.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oc.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://ao.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://be.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uy.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://la.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jp.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://de.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ij.panjiajie.cn

================================================================================
来源：http://kp.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://bu.wgjwhj.cn

================================================================================
来源：http://sn.huanxung.cn

[M01] 读取命令行参数
来源：http://dw.9csxet.cn

Py:   sys.argv[1:]
来源：http://nn.521024.cn

PHP:  $argv;  $argc;
来源：http://su.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://oc.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://ge.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://wb.jctech888.com.cn

Go:   os.Args[1:]
来源：http://ps.haigaiapp.cn


<!-- 参考信息 -->