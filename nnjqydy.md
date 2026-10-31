代发 wailian999

TS:   s.match(/\d+/g)
来源：http://uh.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jk.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qv.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://be.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gb.gzmigu.cn

[I03] 提取捕获分组
来源：http://vz.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qq.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vr.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wh.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jv.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zh.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://to.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bk.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sg.wgjwhj.cn

[I04] 正则替换
来源：http://qx.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yv.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://op.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ix.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zn.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bx.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ny.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://da.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://co.hnjuh.cn

[I05] 按正则拆分
来源：http://ls.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tb.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fx.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://rb.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://bs.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://ag.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://py.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dj.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xa.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bd.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jg.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kb.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bq.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ho.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zp.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ik.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://et.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dm.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://re.bjjhwx.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mp.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tz.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dv.shxzukj.cn

TS:   /error/gim
来源：http://xx.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nc.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nw.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://rm.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fv.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://lr.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ly.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qf.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wv.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pl.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vc.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ap.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ks.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://io.yuntaijiaju.cn

================================================================================
来源：http://zc.muxihuayi.cn

J. 日期与时间
来源：http://lj.asd995.cn

================================================================================
来源：http://kc.panjiajie.cn

[J01] 获取当前时间
来源：http://qu.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://by.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ri.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://fq.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://pn.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nl.521024.cn

Go:   time.Now()
来源：http://pu.521024.cn

Ruby: Time.now
来源：http://nj.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ki.chemitech.net.cn

[J02] 格式化输出
来源：http://zd.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://go.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fq.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://us.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://yc.colortex.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wv.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ew.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vv.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ib.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://wu.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hd.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ix.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://nc.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://rf.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ki.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hm.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://cx.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qx.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://iv.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lu.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wy.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sn.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vh.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rm.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mf.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ir.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ou.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://vp.asd995.cn

Py:   now + timedelta(days=7)
来源：http://wa.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cm.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hu.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qn.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://mi.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://je.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://dg.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vk.asd995.cn

[J06] 计算两时间之差
来源：http://hk.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://zg.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://og.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fl.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hv.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gx.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://oh.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://zo.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://sw.lnxyls.cn

[J07] 比较两个日期
来源：http://sn.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://jm.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nr.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ya.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://eu.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ea.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mj.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ym.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://cp.szsharing.cn

[J08] 提取年月日与星期
来源：http://zw.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tc.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://px.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nd.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xg.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sm.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gx.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eb.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xa.jianghongdianzi.cn

[J09] 时区处理
来源：http://ek.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rt.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jm.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jw.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rk.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://po.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fo.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lh.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uq.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://ys.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yp.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ah.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vd.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gc.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gf.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lx.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gp.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ge.nszjky.cn

================================================================================
来源：http://ke.chemitech.net.cn

K. JSON 与序列化
来源：http://nn.yuexingan06.cn

================================================================================
来源：http://qn.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://lv.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jn.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lv.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://yn.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://mq.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ty.521024.cn

Go:   json.Marshal(obj)
来源：http://zu.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://es.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ed.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://pt.521024.cn

Py:   json.loads(s)
来源：http://xn.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qi.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://lp.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://vv.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mh.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://jw.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://yx.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wd.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://mx.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mt.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xk.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cg.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://po.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ae.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xf.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vf.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vm.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://ob.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://av.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vc.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ig.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pu.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tw.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wy.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xs.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rx.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://ni.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://eo.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://ud.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://zu.asd995.cn

TS:   structuredClone(obj)
来源：http://px.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hl.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dq.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xu.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://it.nszjky.cn

[K06] 解析 URL 查询串
来源：http://wd.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dp.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ru.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://un.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zc.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qp.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mf.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ab.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ct.nszjky.cn

[K07] 进制转换
来源：http://rj.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qb.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fn.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ml.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vr.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ah.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://it.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gd.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sj.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://fu.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://te.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lz.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://dg.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://la.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dv.gzmigu.cn

Go:   encoding/gob
来源：http://ti.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://bf.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://px.yuexingan06.cn

================================================================================
来源：http://al.yuntaijiaju.cn

L. 网络请求
来源：http://jm.asd995.cn

================================================================================
来源：http://tt.gzmigu.cn

[L01] 发送 GET 请求
来源：http://ft.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wn.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vv.muxihuayi.cn

JS:   await fetch(url)
来源：http://dl.shxzskj.cn

TS:   await fetch(url)
来源：http://xk.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://br.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://pv.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ou.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dl.521024.cn

[L02] 发送 POST JSON
来源：http://zk.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wt.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sq.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fx.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wm.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oq.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://up.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://by.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sn.panjiajie.cn

[L03] 设置自定义请求头
来源：http://nd.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://au.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ez.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ph.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zc.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qz.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jz.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nx.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rg.wgjwhj.cn

[L04] 设置超时
来源：http://oe.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://ce.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oe.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fn.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wx.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gk.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://th.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iu.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ze.asd995.cn

[L05] 上传文件（multipart）
来源：http://sd.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qx.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kf.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sk.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ix.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ct.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ez.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jc.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sq.nszjky.cn

[L06] 解析响应为 JSON
来源：http://qh.jctech888.com.cn

Py:   resp.json()
来源：http://ju.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://kl.wgjwhj.cn

JS:   await resp.json()
来源：http://et.muxihuayi.cn

TS:   await resp.json()
来源：http://an.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hq.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ou.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://fp.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://li.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://sy.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qu.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://co.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://du.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://zm.wgjwhj.cn

Java: resp.statusCode()
来源：http://ey.nicolike.cn

Go:   resp.StatusCode
来源：http://to.huanxung.cn

Ruby: resp.code.to_i
来源：http://ie.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://aw.szsharing.cn

[L08] 并发请求多个地址
来源：http://ln.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qs.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://oi.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tz.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dr.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hg.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vp.wgjwhj.cn


<!-- 参考信息 -->