代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uy.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hs.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://ha.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pe.9csxet.cn

[I02] 提取所有匹配
来源：http://oz.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://lo.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nh.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://be.521024.cn

TS:   s.match(/\d+/g)
来源：http://ms.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lo.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pz.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://ng.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qa.9csxet.cn

[I03] 提取捕获分组
来源：http://jr.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://db.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ft.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ub.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ag.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ip.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qm.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mw.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jt.chemitech.net.cn

[I04] 正则替换
来源：http://qt.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wz.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yp.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tp.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zc.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nk.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rv.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hq.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://na.huanxung.cn

[I05] 按正则拆分
来源：http://fp.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nf.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dr.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://tm.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://fx.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://cj.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ve.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wo.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ie.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xr.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ff.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vs.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://us.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tk.huanxung.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xz.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dq.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bt.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pp.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://gr.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ep.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yj.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yd.nszjky.cn

TS:   /error/gim
来源：http://dw.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pl.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kx.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://pe.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ue.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://tb.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xf.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xt.shxzukj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tq.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ly.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ij.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gj.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bz.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ad.nszjky.cn

================================================================================
来源：http://lb.panjiajie.cn

J. 日期与时间
来源：http://eo.panjiajie.cn

================================================================================
来源：http://nu.nszjky.cn

[J01] 获取当前时间
来源：http://tt.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tv.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dq.newstarts.cn

JS:   new Date();  Date.now()
来源：http://zc.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://vo.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://no.chemitech.net.cn

Go:   time.Now()
来源：http://md.nicolike.cn

Ruby: Time.now
来源：http://pz.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rp.wgjwhj.cn

[J02] 格式化输出
来源：http://vo.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kc.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://af.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ur.nicolike.cn

TS:   d.toISOString()
来源：http://uu.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ly.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zy.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hu.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wq.szsharing.cn

[J03] 字符串解析为日期
来源：http://hc.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vw.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ey.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://bx.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://mn.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ei.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jx.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://kv.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bg.9csxet.cn

[J04] 时间戳与日期互转
来源：http://go.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qo.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wb.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wo.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sm.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ca.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yb.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://om.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cv.521024.cn

[J05] 时间加减（加 7 天）
来源：http://vx.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://ca.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rj.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://en.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wk.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://rl.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gx.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://ut.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ab.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://mz.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://on.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://oa.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kh.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://om.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sq.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://fx.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://uh.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://bb.szsharing.cn

[J07] 比较两个日期
来源：http://uz.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://yl.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oz.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ai.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dc.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bl.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vi.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wh.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://dw.9csxet.cn

[J08] 提取年月日与星期
来源：http://jn.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nz.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://al.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qc.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gs.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tm.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ez.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pi.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vz.jianghongdianzi.cn

[J09] 时区处理
来源：http://gs.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wv.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ah.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tw.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yl.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sf.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hh.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rf.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cx.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://ga.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://st.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tm.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sd.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ys.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gn.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ju.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hy.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lv.hnjuh.cn

================================================================================
来源：http://lk.huixiangedu.cn

K. JSON 与序列化
来源：http://er.bjjhwx.cn

================================================================================
来源：http://bd.521024.cn

[K01] 对象转 JSON 字符串
来源：http://kj.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vd.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://up.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://id.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://fy.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vh.hahajie.cn

Go:   json.Marshal(obj)
来源：http://sw.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zt.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cc.521024.cn

[K02] JSON 字符串转对象
来源：http://jz.nszjky.cn

Py:   json.loads(s)
来源：http://ez.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sv.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://hu.asd995.cn

TS:   JSON.parse(s)
来源：http://rz.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hb.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://rt.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://bt.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ki.bookmarksfly.cn

[K03] JSON 美化输出（带缩进）
来源：http://go.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lj.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oh.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cl.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ht.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fh.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ke.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fk.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cb.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://xm.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lx.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://af.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wq.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://on.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ir.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://md.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gq.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zv.gzmigu.cn

[K05] 深拷贝对象
来源：http://am.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://tm.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://gj.nicolike.cn

JS:   structuredClone(obj)
来源：http://sa.521024.cn

TS:   structuredClone(obj)
来源：http://xj.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dk.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dc.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jc.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rj.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://so.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pa.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ry.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pk.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xu.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vy.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pk.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qa.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yh.shxzukj.cn

[K07] 进制转换
来源：http://na.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hx.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ml.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ft.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xq.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mz.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://px.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mm.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kj.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://pk.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://wa.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wo.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://mp.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://gq.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wa.shxzukj.cn

Go:   encoding/gob
来源：http://ro.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://bh.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ea.jianghongdianzi.cn

================================================================================
来源：http://dg.hnjuh.cn

L. 网络请求
来源：http://dh.colortex.cn

================================================================================
来源：http://ms.asd995.cn

[L01] 发送 GET 请求
来源：http://jy.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://he.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rt.wgjwhj.cn

JS:   await fetch(url)
来源：http://ev.hnjuh.cn

TS:   await fetch(url)
来源：http://qq.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rs.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://fs.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bz.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zh.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://us.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://su.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gt.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bw.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qc.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pj.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qo.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://it.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fo.szxytkj.cn

[L03] 设置自定义请求头
来源：http://yu.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ku.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zm.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ki.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fv.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sv.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jj.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gy.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qe.newstarts.cn

[L04] 设置超时
来源：http://yb.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://fe.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pr.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iq.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zv.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://go.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ps.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lt.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nv.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://as.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ug.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sy.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fh.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fb.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ak.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ov.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ys.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://va.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://pp.bjjhwx.cn

Py:   resp.json()
来源：http://fv.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://be.haigaiapp.cn

JS:   await resp.json()
来源：http://ky.jianghongdianzi.cn

TS:   await resp.json()
来源：http://nw.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oh.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uf.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://ow.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zt.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://rn.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yr.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nv.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://zo.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://bg.chemitech.net.cn

Java: resp.statusCode()
来源：http://el.hnjuh.cn

Go:   resp.StatusCode
来源：http://vv.asd995.cn

Ruby: resp.code.to_i
来源：http://xn.shxzskj.cn


<!-- 参考信息 -->