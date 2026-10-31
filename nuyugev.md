代发 wailian999

Py:   value = d.get("k") or default
来源：http://ki.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zl.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ei.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qk.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fk.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bu.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://dv.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://ff.huixiangedu.cn

[H07] 断言
来源：http://pp.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://bb.shxzskj.cn

PHP:  assert($x > 0);
来源：http://cf.chemitech.net.cn

JS:   console.assert(x > 0);
来源：http://ag.szsharing.cn

TS:   console.assert(x > 0);
来源：http://uc.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://tp.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pc.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jo.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://zd.hahajie.cn

[H08] 获取错误信息与堆栈
来源：http://ny.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://zb.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dw.panjiajie.cn

JS:   e.message;  e.stack
来源：http://ne.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jd.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bf.huixiangedu.cn

Go:   err.Error()
来源：http://rr.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://im.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://tv.huanxung.cn

[H09] 带错误码的异常
来源：http://sy.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ft.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qm.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fe.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rw.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://af.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fl.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rs.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sq.lnxyls.cn

[H10] 资源自动释放
来源：http://af.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bd.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dy.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zj.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nk.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jy.shxzskj.cn

Go:   defer f.Close()
来源：http://qt.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fd.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sk.haigaiapp.cn

================================================================================
来源：http://cq.jianghongdianzi.cn

I. 正则表达式
来源：http://xw.muxihuayi.cn

================================================================================
来源：http://aw.chemitech.net.cn

[I01] 判断是否匹配
来源：http://ub.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pj.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eq.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://aq.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://bc.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ij.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eu.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://zi.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ht.521024.cn

[I02] 提取所有匹配
来源：http://zy.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://jo.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ab.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jd.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://sd.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zu.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ei.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://ir.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jz.shxzukj.cn

[I03] 提取捕获分组
来源：http://ut.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zm.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zp.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bu.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ky.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ix.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rq.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xi.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ls.wgjwhj.cn

[I04] 正则替换
来源：http://re.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kh.huanxung.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nk.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uh.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qx.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dk.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kh.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mi.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://te.huanxung.cn

[I05] 按正则拆分
来源：http://aq.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ep.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ox.colortex.cn

JS:   s.split(/\s*,\s*/)
来源：http://lh.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://xd.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://um.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fn.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ee.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oq.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gr.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sw.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bf.hahajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fp.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ev.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ry.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wb.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://is.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dy.521024.cn

[I07] 忽略大小写与多行模式
来源：http://zb.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oc.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fo.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vr.jctech888.com.cn

TS:   /error/gim
来源：http://ec.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nu.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://be.shxzskj.cn

Ruby: s.scan(/error/i)
来源：http://si.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ig.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://km.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hc.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ms.shxzukj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zt.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://px.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xl.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gh.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ee.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wu.9csxet.cn

================================================================================
来源：http://fg.haigaiapp.cn

J. 日期与时间
来源：http://xt.shxzskj.cn

================================================================================
来源：http://kc.9csxet.cn

[J01] 获取当前时间
来源：http://fx.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ni.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rp.521024.cn

JS:   new Date();  Date.now()
来源：http://tj.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://qy.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bq.gzmigu.cn

Go:   time.Now()
来源：http://af.hahajie.cn

Ruby: Time.now
来源：http://ya.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nx.huixiangedu.cn

[J02] 格式化输出
来源：http://eb.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mm.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://je.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bq.muxihuayi.cn

TS:   d.toISOString()
来源：http://mg.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ro.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://je.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hk.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://my.szxytkj.cn

[J03] 字符串解析为日期
来源：http://nh.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ii.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oj.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://mi.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://ox.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fb.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lx.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://wg.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hg.huanxung.cn

[J04] 时间戳与日期互转
来源：http://zz.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qd.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ua.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dw.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://by.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bg.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fe.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ag.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kf.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://mt.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://my.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ub.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dh.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fi.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://ta.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ju.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://fg.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fx.521024.cn

[J06] 计算两时间之差
来源：http://bq.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://jr.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://su.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://be.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://po.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ll.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://qd.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://rr.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://kb.haigaiapp.cn

[J07] 比较两个日期
来源：http://uo.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://ed.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ps.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rg.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://at.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zm.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nx.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rp.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://zd.hnjuh.cn

[J08] 提取年月日与星期
来源：http://rv.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://je.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bu.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vt.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vd.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://em.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vc.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eb.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vf.haigaiapp.cn

[J09] 时区处理
来源：http://qf.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fe.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sd.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jt.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mm.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://im.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://td.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yk.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dn.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://tw.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dc.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pz.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fh.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ao.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ke.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bg.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tm.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xs.shtwfgs.cn

================================================================================
来源：http://zj.bookmarksfly.cn

K. JSON 与序列化
来源：http://pu.huanxung.cn

================================================================================
来源：http://zb.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://ei.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dg.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://js.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://fi.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://oj.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pt.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://ap.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jx.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tw.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://lj.chemitech.net.cn

Py:   json.loads(s)
来源：http://mw.huixiangedu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xs.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://zf.newstarts.cn

TS:   JSON.parse(s)
来源：http://oq.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fe.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://gf.nszjky.cn

Ruby: JSON.parse(s)
来源：http://jn.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tw.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://ls.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uz.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zn.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pl.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qq.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qx.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gl.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hc.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cp.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://ae.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bz.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ig.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://os.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ry.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aa.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vy.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xo.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nv.colortex.cn

[K05] 深拷贝对象
来源：http://le.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://hr.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://ar.lnxyls.cn

JS:   structuredClone(obj)
来源：http://ba.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://sw.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ir.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iu.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dt.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yr.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://kb.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vb.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tw.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pf.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ik.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qm.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vn.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ps.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uz.colortex.cn

[K07] 进制转换
来源：http://us.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kq.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bo.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ik.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cu.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rr.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cl.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ef.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bc.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://ss.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://ze.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dt.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://qd.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://ql.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cc.yuexingan06.cn

Go:   encoding/gob
来源：http://bm.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://cr.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rx.hnjuh.cn

================================================================================
来源：http://gy.haigaiapp.cn

L. 网络请求
来源：http://vi.hnjuh.cn

================================================================================
来源：http://xd.huanxung.cn

[L01] 发送 GET 请求
来源：http://it.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ev.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ul.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://eg.newstarts.cn

TS:   await fetch(url)
来源：http://yc.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fh.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://ca.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dv.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gk.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://vd.nszjky.cn


<!-- 参考信息 -->