代发 wailian999

TS:   s.match(/\d+/g)
来源：http://uu.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iv.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tw.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://wl.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://de.yuexingan06.cn

[I03] 提取捕获分组
来源：http://ns.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rr.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qi.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://de.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iw.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nn.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zv.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sp.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ry.bookmarksfly.cn

[I04] 正则替换
来源：http://vw.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gq.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cx.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hj.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://za.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://au.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nx.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ff.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qi.szsharing.cn

[I05] 按正则拆分
来源：http://ve.9csxet.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nx.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sy.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://yv.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://vm.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://mv.bookmarksfly.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ab.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hi.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://do.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mj.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zp.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vr.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pv.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ay.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wn.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tt.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://po.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hn.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://nl.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ko.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fc.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ls.yuexingan06.cn

TS:   /error/gim
来源：http://hs.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ga.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://br.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://fw.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tt.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://fj.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cp.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zx.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cq.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rm.bookmarksfly.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vw.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uz.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nv.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wq.panjiajie.cn

================================================================================
来源：http://qy.shtwfgs.cn

J. 日期与时间
来源：http://ml.panjiajie.cn

================================================================================
来源：http://sy.9csxet.cn

[J01] 获取当前时间
来源：http://im.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yz.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oz.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://iq.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://zl.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nh.szxytkj.cn

Go:   time.Now()
来源：http://ox.bookmarksfly.cn

Ruby: Time.now
来源：http://zr.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fq.jctech888.com.cn

[J02] 格式化输出
来源：http://oz.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ts.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oc.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rt.jctech888.com.cn

TS:   d.toISOString()
来源：http://zk.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xy.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qv.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qf.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ce.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://wm.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jl.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cr.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://ak.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://ld.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yc.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vt.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://fp.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pl.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://lb.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://my.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xq.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sw.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ik.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wz.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xi.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cp.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ca.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://vx.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://cq.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mf.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zi.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eu.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://lb.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hc.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://vy.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cx.panjiajie.cn

[J06] 计算两时间之差
来源：http://ma.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://gf.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://hv.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kb.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qf.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sc.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://qz.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://fy.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://ns.szxytkj.cn

[J07] 比较两个日期
来源：http://io.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://ui.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dt.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lz.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ia.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://im.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yy.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://oe.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://aw.panjiajie.cn

[J08] 提取年月日与星期
来源：http://zs.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vc.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gp.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ty.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eh.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ut.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qo.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mo.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mh.yuntaijiaju.cn

[J09] 时区处理
来源：http://ih.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ic.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ol.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ol.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ju.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dm.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xx.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yk.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://du.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://la.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sd.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bc.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sp.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ml.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tf.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://aq.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xs.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://za.huixinmuqiang.cn

================================================================================
来源：http://hu.gzmigu.cn

K. JSON 与序列化
来源：http://bz.huixiangedu.cn

================================================================================
来源：http://re.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://ih.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ns.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fe.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://hf.colortex.cn

TS:   JSON.stringify(obj)
来源：http://hn.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wa.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://ut.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tf.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kt.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://cp.newstarts.cn

Py:   json.loads(s)
来源：http://za.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gz.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://bl.asd995.cn

TS:   JSON.parse(s)
来源：http://xr.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ln.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://ws.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://bs.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eo.bookmarksfly.cn

[K03] JSON 美化输出（带缩进）
来源：http://zk.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wh.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gv.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mj.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ur.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qf.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pg.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dj.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rb.521024.cn

[K04] 读取 JSON 文件
来源：http://op.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ra.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bc.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://df.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vw.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ws.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mx.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gu.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pb.huanxung.cn

[K05] 深拷贝对象
来源：http://gt.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://wn.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://kh.shxzukj.cn

JS:   structuredClone(obj)
来源：http://yf.szxytkj.cn

TS:   structuredClone(obj)
来源：http://qe.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jl.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fy.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://im.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://du.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://el.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tw.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rv.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ff.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ko.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yd.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kg.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pc.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://co.szxytkj.cn

[K07] 进制转换
来源：http://ct.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xr.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pt.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gh.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fk.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://la.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gj.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gf.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xl.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://si.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://fj.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mw.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://jb.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://kz.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gh.shxzskj.cn

Go:   encoding/gob
来源：http://tb.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://gf.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kj.chemitech.net.cn

================================================================================
来源：http://za.lnxyls.cn

L. 网络请求
来源：http://tg.asd995.cn

================================================================================
来源：http://ii.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://ys.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sh.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sc.bookmarksfly.cn

JS:   await fetch(url)
来源：http://di.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://nh.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://go.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://ps.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://po.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hi.hnjuh.cn

[L02] 发送 POST JSON
来源：http://ut.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kg.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gt.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lq.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ui.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rn.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ii.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ne.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bb.lnxyls.cn

[L03] 设置自定义请求头
来源：http://tp.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gy.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://er.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pv.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tj.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ek.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gy.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yo.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cd.newstarts.cn

[L04] 设置超时
来源：http://zh.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://ty.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wm.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tt.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vo.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bb.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sw.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ai.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vl.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://ml.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xr.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mc.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sb.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rj.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ju.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://av.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tc.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://un.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://et.nszjky.cn

Py:   resp.json()
来源：http://cb.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://bp.jctech888.com.cn

JS:   await resp.json()
来源：http://uv.haigaiapp.cn

TS:   await resp.json()
来源：http://di.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zw.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nd.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://nv.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ix.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://ta.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ty.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wu.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://st.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://vo.521024.cn

Java: resp.statusCode()
来源：http://bm.lnxyls.cn

Go:   resp.StatusCode
来源：http://vy.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://jb.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://sx.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://sl.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lh.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://uj.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cb.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vc.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://av.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gp.shxzukj.cn


<!-- 参考信息 -->