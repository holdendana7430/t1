代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iv.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ju.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kq.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cx.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fy.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sr.wgjwhj.cn

[I04] 正则替换
来源：http://wb.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bl.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pa.lnxyls.cn

JS:   s.replace(/\d+/g, "#")
来源：http://be.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xg.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lz.yuntaijiaju.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fp.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nk.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oj.panjiajie.cn

[I05] 按正则拆分
来源：http://hb.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oz.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://of.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://ku.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://ln.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://lb.bookmarksfly.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zd.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cx.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bo.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gu.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://if.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pt.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dz.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ff.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mw.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sx.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rk.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fb.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://gm.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mn.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fo.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://md.huixiangedu.cn

TS:   /error/gim
来源：http://vj.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ai.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ex.szxytkj.cn

Ruby: s.scan(/error/i)
来源：http://sd.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qg.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://lq.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vl.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ya.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ra.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xz.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yx.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mf.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gt.colortex.cn

================================================================================
来源：http://bw.szxytkj.cn

J. 日期与时间
来源：http://wb.asd995.cn

================================================================================
来源：http://mw.nszjky.cn

[J01] 获取当前时间
来源：http://ln.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dq.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://op.hahajie.cn

JS:   new Date();  Date.now()
来源：http://tv.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://xr.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mo.huixiangedu.cn

Go:   time.Now()
来源：http://zo.yuexingan06.cn

Ruby: Time.now
来源：http://gk.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sk.panjiajie.cn

[J02] 格式化输出
来源：http://bn.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rq.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jj.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oq.panjiajie.cn

TS:   d.toISOString()
来源：http://mn.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cv.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cm.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ib.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kk.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://xh.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mr.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gd.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://rh.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://yy.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cn.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iz.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ot.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fc.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://ri.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ks.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xo.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vh.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ln.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nu.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ay.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ii.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://le.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://qg.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://az.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vk.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kh.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hf.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://br.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ih.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://zq.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dj.panjiajie.cn

[J06] 计算两时间之差
来源：http://tb.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://io.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://ff.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fe.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://om.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mz.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://pw.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://na.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://zd.haigaiapp.cn

[J07] 比较两个日期
来源：http://tv.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://nr.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ji.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sf.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ok.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://to.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iu.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fy.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://va.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://fz.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://he.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nn.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kb.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ic.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ob.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xb.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hl.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nc.9csxet.cn

[J09] 时区处理
来源：http://qs.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yg.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pn.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oh.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qr.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hi.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://om.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jr.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ip.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://iu.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ds.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nn.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kb.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gy.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cc.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ko.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://th.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tp.huixinmuqiang.cn

================================================================================
来源：http://jz.huixiangedu.cn

K. JSON 与序列化
来源：http://xo.colortex.cn

================================================================================
来源：http://lv.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://tn.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pk.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hv.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://ks.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://uo.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ou.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://ew.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fi.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bj.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://ji.gzmigu.cn

Py:   json.loads(s)
来源：http://yg.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rf.szxytkj.cn

JS:   JSON.parse(s)
来源：http://kg.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://bs.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ia.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://qw.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://sy.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ys.bookmarksfly.cn

[K03] JSON 美化输出（带缩进）
来源：http://ar.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yx.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rg.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ks.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vv.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yc.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lb.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lf.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vr.newstarts.cn

[K04] 读取 JSON 文件
来源：http://jm.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rg.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iv.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oh.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xw.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tz.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ft.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vm.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aw.hnjuh.cn

[K05] 深拷贝对象
来源：http://ib.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://mb.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://qp.newstarts.cn

JS:   structuredClone(obj)
来源：http://zz.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://vj.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jf.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lk.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gf.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yd.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://vc.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kt.huixinmuqiang.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://of.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ij.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qj.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rr.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ga.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iv.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nw.asd995.cn

[K07] 进制转换
来源：http://ug.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://io.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pg.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nm.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ru.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://su.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rx.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nm.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qz.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://ms.521024.cn

Py:   pickle.dumps(obj)
来源：http://os.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gf.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://mq.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://vc.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ss.szxytkj.cn

Go:   encoding/gob
来源：http://vi.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://lr.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pk.chemitech.net.cn

================================================================================
来源：http://un.shtwfgs.cn

L. 网络请求
来源：http://tj.chemitech.net.cn

================================================================================
来源：http://ta.asd995.cn

[L01] 发送 GET 请求
来源：http://ca.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://og.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xw.jctech888.com.cn

JS:   await fetch(url)
来源：http://yy.yuexingan06.cn

TS:   await fetch(url)
来源：http://nl.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ah.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://qa.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://km.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pf.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://pg.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kv.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nd.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://of.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sz.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ds.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cn.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gv.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pt.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://pw.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vd.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gi.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yg.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gu.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tr.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mp.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ke.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zc.huixiangedu.cn

[L04] 设置超时
来源：http://az.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://no.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dq.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rc.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ly.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://om.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qg.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bp.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mn.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://si.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xc.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oh.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dj.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zr.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wv.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zk.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bc.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oy.colortex.cn

[L06] 解析响应为 JSON
来源：http://jm.colortex.cn

Py:   resp.json()
来源：http://hc.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://wk.shtwfgs.cn

JS:   await resp.json()
来源：http://vu.bookmarksfly.cn

TS:   await resp.json()
来源：http://wj.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gl.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qg.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://hw.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zp.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://oi.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fq.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aw.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://qk.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://ct.bookmarksfly.cn

Java: resp.statusCode()
来源：http://hn.haigaiapp.cn

Go:   resp.StatusCode
来源：http://tx.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://ax.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://af.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://no.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fu.huixinmuqiang.cn

PHP:  curl_multi_init() 系列
来源：http://uk.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gy.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hg.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ki.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fk.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ku.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mc.shxzukj.cn

================================================================================
来源：http://lm.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://mn.yuntaijiaju.cn

================================================================================
来源：http://wy.shxzukj.cn

[M01] 读取命令行参数
来源：http://ct.nszjky.cn

Py:   sys.argv[1:]
来源：http://et.newstarts.cn

PHP:  $argv;  $argc;
来源：http://kz.asd995.cn


<!-- 参考信息 -->