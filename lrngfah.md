代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://uj.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://sp.yuexingan06.cn

[H09] 带错误码的异常
来源：http://pi.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lb.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qv.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jy.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ei.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fc.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mj.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://es.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ko.lnxyls.cn

[H10] 资源自动释放
来源：http://cj.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tt.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tl.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kg.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jl.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ih.colortex.cn

Go:   defer f.Close()
来源：http://hs.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gt.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://es.jianghongdianzi.cn

================================================================================
来源：http://lc.shxzskj.cn

I. 正则表达式
来源：http://uo.wgjwhj.cn

================================================================================
来源：http://yb.haigaiapp.cn

[I01] 判断是否匹配
来源：http://yz.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yq.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yd.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://um.newstarts.cn

TS:   /\d+/.test(s)
来源：http://yp.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vp.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cr.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://ix.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lp.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://ny.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://ca.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ie.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jt.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://ll.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gg.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pd.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://ml.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zx.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://vp.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wn.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hy.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dl.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cw.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yv.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tj.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uh.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vc.huixiangedu.cn

[I04] 正则替换
来源：http://qx.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gu.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bp.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ss.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rz.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jf.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ka.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://af.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fw.muxihuayi.cn

[I05] 按正则拆分
来源：http://kv.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jx.haigaiapp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sx.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://gv.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://gf.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://bz.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qe.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tl.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://so.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://si.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://es.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tk.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wj.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yj.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://az.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ym.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dn.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ns.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://wd.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sn.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://co.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hd.jianghongdianzi.cn

TS:   /error/gim
来源：http://cf.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hw.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cb.colortex.cn

Ruby: s.scan(/error/i)
来源：http://kn.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yj.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://nb.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xg.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mq.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://va.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fg.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pb.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://un.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dy.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vt.nszjky.cn

================================================================================
来源：http://vw.jianghongdianzi.cn

J. 日期与时间
来源：http://hu.bjjhwx.cn

================================================================================
来源：http://vg.bookmarksfly.cn

[J01] 获取当前时间
来源：http://ks.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mb.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vr.hahajie.cn

JS:   new Date();  Date.now()
来源：http://el.colortex.cn

TS:   new Date();  Date.now()
来源：http://qp.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cf.huixiangedu.cn

Go:   time.Now()
来源：http://wd.gzmigu.cn

Ruby: Time.now
来源：http://qp.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mc.jctech888.com.cn

[J02] 格式化输出
来源：http://je.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sm.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xq.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nm.muxihuayi.cn

TS:   d.toISOString()
来源：http://tu.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dd.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ng.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eu.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ch.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://zv.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bx.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lh.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://qi.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://ee.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://me.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tw.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://fn.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fa.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://sr.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cl.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bc.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://do.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gl.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ww.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ec.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uv.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rm.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://fh.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://yj.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cd.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gq.bookmarksfly.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vg.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://mv.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://we.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://cn.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lc.chemitech.net.cn

[J06] 计算两时间之差
来源：http://gj.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://tq.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://yt.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sr.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oo.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://im.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://qn.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://so.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://cx.muxihuayi.cn

[J07] 比较两个日期
来源：http://jd.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://xm.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vc.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sn.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dr.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mf.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ie.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ke.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://nu.9csxet.cn

[J08] 提取年月日与星期
来源：http://ks.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wn.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://si.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yf.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ct.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://io.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rr.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eo.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sc.colortex.cn

[J09] 时区处理
来源：http://vp.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uh.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qi.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cr.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ul.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ek.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dl.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rk.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ac.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://uq.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ha.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://le.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://av.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hx.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cw.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wa.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fo.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cx.nszjky.cn

================================================================================
来源：http://vx.jctech888.com.cn

K. JSON 与序列化
来源：http://zx.hahajie.cn

================================================================================
来源：http://zu.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://jn.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hh.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gn.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://si.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://zq.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://no.huanxung.cn

Go:   json.Marshal(obj)
来源：http://gs.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://md.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ke.newstarts.cn

[K02] JSON 字符串转对象
来源：http://co.nszjky.cn

Py:   json.loads(s)
来源：http://yv.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oa.colortex.cn

JS:   JSON.parse(s)
来源：http://fh.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://xu.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lu.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://ml.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://pl.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yc.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://zn.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sj.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rz.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oh.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kx.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vb.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lz.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://om.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wb.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://pk.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xg.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pf.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sn.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gp.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yl.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qw.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vx.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://po.nszjky.cn

[K05] 深拷贝对象
来源：http://gi.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://ot.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://cb.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://jd.szsharing.cn

TS:   structuredClone(obj)
来源：http://ps.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lx.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yw.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://el.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://di.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://wb.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fi.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rf.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lh.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kv.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://il.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vs.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ow.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tq.yuntaijiaju.cn

[K07] 进制转换
来源：http://sv.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wu.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yq.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://it.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zf.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bh.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xu.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hs.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sd.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://sp.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://hw.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sk.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://xn.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://rq.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lu.bjjhwx.cn

Go:   encoding/gob
来源：http://nh.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://dt.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://db.huanxung.cn

================================================================================
来源：http://gw.panjiajie.cn

L. 网络请求
来源：http://sn.yuexingan06.cn

================================================================================
来源：http://mb.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://et.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jv.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://je.muxihuayi.cn

JS:   await fetch(url)
来源：http://zi.shxzukj.cn

TS:   await fetch(url)
来源：http://co.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gk.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://vn.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ka.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dp.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://tj.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vf.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yi.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fu.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://no.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ef.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qf.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kl.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ph.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://yg.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pm.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qc.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dm.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mb.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zu.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ro.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xd.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ta.jianghongdianzi.cn

[L04] 设置超时
来源：http://mr.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://ai.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ju.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wd.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ee.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rq.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lw.huixinmuqiang.cn


<!-- 参考信息 -->