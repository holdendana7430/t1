代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://sr.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://fv.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://ez.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://za.szxytkj.cn

JS:   e.message;  e.stack
来源：http://cn.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yt.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pf.jctech888.com.cn

Go:   err.Error()
来源：http://lp.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://qp.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://ib.chemitech.net.cn

[H09] 带错误码的异常
来源：http://eh.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sy.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://sh.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xn.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://is.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yx.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iv.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mq.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wu.haigaiapp.cn

[H10] 资源自动释放
来源：http://iw.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ab.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wo.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rp.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xg.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uw.nicolike.cn

Go:   defer f.Close()
来源：http://ma.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gj.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zb.nszjky.cn

================================================================================
来源：http://hm.bjjhwx.cn

I. 正则表达式
来源：http://uw.521024.cn

================================================================================
来源：http://ua.nszjky.cn

[I01] 判断是否匹配
来源：http://re.huixiangedu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dp.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vt.colortex.cn

JS:   /\d+/.test(s)
来源：http://re.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://og.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fh.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yz.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://ab.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bs.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://xu.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://qr.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kd.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mj.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://cv.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lj.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jk.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://oy.muxihuayi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oc.521024.cn

[I03] 提取捕获分组
来源：http://gh.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yy.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ai.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kg.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://md.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pm.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ae.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yw.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tu.bjjhwx.cn

[I04] 正则替换
来源：http://nz.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dv.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yx.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bs.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qy.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zg.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jw.chemitech.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zz.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qt.huanxung.cn

[I05] 按正则拆分
来源：http://zh.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://aq.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ml.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://xw.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://bp.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://ls.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bl.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fq.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zl.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dp.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mo.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://we.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jm.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cz.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fo.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jt.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ny.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pv.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://mv.huanxung.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lq.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kt.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ys.szsharing.cn

TS:   /error/gim
来源：http://nh.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ed.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ix.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://cu.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wl.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://im.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ny.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jd.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nm.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ri.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xa.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vd.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bl.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jp.bjjhwx.cn

================================================================================
来源：http://ip.colortex.cn

J. 日期与时间
来源：http://js.9csxet.cn

================================================================================
来源：http://bq.huanxung.cn

[J01] 获取当前时间
来源：http://fi.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dm.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yx.huanxung.cn

JS:   new Date();  Date.now()
来源：http://en.9csxet.cn

TS:   new Date();  Date.now()
来源：http://pl.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://po.jctech888.com.cn

Go:   time.Now()
来源：http://wp.shxzukj.cn

Ruby: Time.now
来源：http://pp.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hw.szxytkj.cn

[J02] 格式化输出
来源：http://hd.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hw.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bt.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yc.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://dv.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rf.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ct.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gs.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cr.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://rf.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qa.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://va.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://fs.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://qo.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xp.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pf.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://ou.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pe.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://wp.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mb.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gt.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ul.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vg.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nm.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lu.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wf.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ez.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://rk.wgjwhj.cn

Py:   now + timedelta(days=7)
来源：http://pe.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fn.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kw.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bh.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://sh.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ml.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://vq.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://be.jctech888.com.cn

[J06] 计算两时间之差
来源：http://si.colortex.cn

Py:   (end - start).total_seconds()
来源：http://cx.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://kn.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gh.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oh.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wj.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://te.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://xk.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://an.szsharing.cn

[J07] 比较两个日期
来源：http://zw.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://rn.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://or.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mo.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uw.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tx.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iu.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rt.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://dm.9csxet.cn

[J08] 提取年月日与星期
来源：http://iq.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jp.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nl.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dx.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ps.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://el.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hq.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zn.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://on.hnjuh.cn

[J09] 时区处理
来源：http://wg.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nl.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zu.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mo.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fa.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bt.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sc.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kx.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yi.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://md.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oj.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aq.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pp.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ko.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fh.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sm.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gi.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wb.szxytkj.cn

================================================================================
来源：http://id.hahajie.cn

K. JSON 与序列化
来源：http://oi.colortex.cn

================================================================================
来源：http://js.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://uf.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://id.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xv.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://pb.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://au.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://en.521024.cn

Go:   json.Marshal(obj)
来源：http://dl.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gs.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yh.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://jx.nicolike.cn

Py:   json.loads(s)
来源：http://xx.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qh.szxytkj.cn

JS:   JSON.parse(s)
来源：http://nm.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://ci.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://en.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://uz.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://fu.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bt.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://xv.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vk.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dn.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oh.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://id.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gk.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hh.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pv.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kb.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://by.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rf.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ic.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fa.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zo.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vq.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dy.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mt.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mr.nicolike.cn

[K05] 深拷贝对象
来源：http://qk.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://dw.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://ck.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://wh.9csxet.cn

TS:   structuredClone(obj)
来源：http://kx.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pc.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gz.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://im.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xx.521024.cn

[K06] 解析 URL 查询串
来源：http://rf.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mg.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rd.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dg.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ai.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ka.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://km.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ou.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tt.yuntaijiaju.cn

[K07] 进制转换
来源：http://pa.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bm.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zb.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ji.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fw.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mo.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gh.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://la.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nj.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://kt.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://cq.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dx.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://bi.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://gl.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dv.muxihuayi.cn

Go:   encoding/gob
来源：http://kg.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://wp.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jq.lnxyls.cn

================================================================================
来源：http://wp.bjjhwx.cn

L. 网络请求
来源：http://ha.shxzskj.cn

================================================================================
来源：http://wd.shxzukj.cn

[L01] 发送 GET 请求
来源：http://fy.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nd.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oi.muxihuayi.cn

JS:   await fetch(url)
来源：http://dg.nszjky.cn

TS:   await fetch(url)
来源：http://bx.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ll.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://wj.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hk.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gw.asd995.cn

[L02] 发送 POST JSON
来源：http://oi.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sw.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ek.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yz.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mq.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bb.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kh.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hw.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mm.hahajie.cn

[L03] 设置自定义请求头
来源：http://go.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kp.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nr.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qi.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ap.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qj.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uw.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oh.521024.cn


<!-- 参考信息 -->