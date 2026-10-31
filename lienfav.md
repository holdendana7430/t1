代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vf.chemitech.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://he.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://mf.szxytkj.cn

C#:   obj?.A?.B ?? default
来源：http://mj.hnjuh.cn

[H07] 断言
来源：http://ye.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://ww.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://nx.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://yp.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://aj.newstarts.cn

Java: assert x > 0 : "必须为正";
来源：http://dr.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sf.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tz.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://no.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://po.yuexingan06.cn

Py:   str(e);  traceback.format_exc()
来源：http://qx.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lf.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://cf.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hq.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yd.yuntaijiaju.cn

Go:   err.Error()
来源：http://xm.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://ds.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://fm.9csxet.cn

[H09] 带错误码的异常
来源：http://fs.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pj.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tb.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ri.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lg.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kr.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sb.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://do.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qh.chemitech.net.cn

[H10] 资源自动释放
来源：http://nh.huixinmuqiang.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wi.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bh.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zt.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ft.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pn.521024.cn

Go:   defer f.Close()
来源：http://km.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jf.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://px.bookmarksfly.cn

================================================================================
来源：http://na.haigaiapp.cn

I. 正则表达式
来源：http://vt.newstarts.cn

================================================================================
来源：http://zx.gzmigu.cn

[I01] 判断是否匹配
来源：http://fj.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fc.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dp.huanxung.cn

JS:   /\d+/.test(s)
来源：http://yk.nszjky.cn

TS:   /\d+/.test(s)
来源：http://gc.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kr.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ip.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://dg.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://og.asd995.cn

[I02] 提取所有匹配
来源：http://jk.bjjhwx.cn

Py:   re.findall(r"\d+", s)
来源：http://zq.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zq.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ya.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://nq.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jp.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://st.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://hh.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cn.lnxyls.cn

[I03] 提取捕获分组
来源：http://ks.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sl.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rz.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ef.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tx.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ar.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pr.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pl.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vp.yuntaijiaju.cn

[I04] 正则替换
来源：http://hv.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tc.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fc.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ud.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yg.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pj.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kj.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://oj.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hj.nicolike.cn

[I05] 按正则拆分
来源：http://do.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uk.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://he.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://sx.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://az.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://re.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gn.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zz.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hh.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xz.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jj.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tu.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tt.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://se.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qf.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hp.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qw.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yk.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://ff.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://no.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dk.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sa.huixinmuqiang.cn

TS:   /error/gim
来源：http://wk.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tz.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://no.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://wz.521024.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oo.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://mx.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hw.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rz.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uo.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ar.yuntaijiaju.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bh.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://av.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://az.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yr.bookmarksfly.cn

================================================================================
来源：http://fg.asd995.cn

J. 日期与时间
来源：http://wm.yuexingan06.cn

================================================================================
来源：http://sp.shxzukj.cn

[J01] 获取当前时间
来源：http://kf.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://aa.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vr.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://rw.szsharing.cn

TS:   new Date();  Date.now()
来源：http://oi.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sw.szxytkj.cn

Go:   time.Now()
来源：http://cc.yuntaijiaju.cn

Ruby: Time.now
来源：http://dk.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uc.chemitech.net.cn

[J02] 格式化输出
来源：http://ah.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zz.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uf.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ue.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://nt.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tc.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tb.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bk.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jc.colortex.cn

[J03] 字符串解析为日期
来源：http://ig.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://we.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vh.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://pt.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://km.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ln.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://od.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://xg.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ae.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://jd.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jb.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jc.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ay.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://br.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mj.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://io.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nd.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oa.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://sk.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://jz.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://du.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cx.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dg.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://ze.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mg.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://zm.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zh.hahajie.cn

[J06] 计算两时间之差
来源：http://cf.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://xn.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://ft.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fg.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rp.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ot.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://nw.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://zk.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://au.wgjwhj.cn

[J07] 比较两个日期
来源：http://qx.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://hq.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dm.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qt.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wg.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sd.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oh.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wk.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://kz.9csxet.cn

[J08] 提取年月日与星期
来源：http://tv.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pi.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ry.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mi.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fl.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hg.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ak.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ul.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://li.gzmigu.cn

[J09] 时区处理
来源：http://qn.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pu.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fj.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ek.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pw.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iy.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ms.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wo.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lx.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://tj.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jv.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://el.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fw.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://id.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gf.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://si.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oo.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cy.nicolike.cn

================================================================================
来源：http://de.bjjhwx.cn

K. JSON 与序列化
来源：http://bv.shxzukj.cn

================================================================================
来源：http://aa.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://xk.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ke.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xi.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://ww.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://vt.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lp.huanxung.cn

Go:   json.Marshal(obj)
来源：http://er.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://od.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pg.newstarts.cn

[K02] JSON 字符串转对象
来源：http://ar.bookmarksfly.cn

Py:   json.loads(s)
来源：http://tj.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gc.nszjky.cn

JS:   JSON.parse(s)
来源：http://ga.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://mi.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ep.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://nu.huanxung.cn

Ruby: JSON.parse(s)
来源：http://sw.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fc.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://fo.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ty.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kb.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wi.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tu.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ct.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sy.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://da.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ca.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://eu.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tv.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aq.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://re.gzmigu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qp.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vh.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qj.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uy.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://if.gzmigu.cn

[K05] 深拷贝对象
来源：http://op.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://oa.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://mm.colortex.cn

JS:   structuredClone(obj)
来源：http://eg.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://mc.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yl.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pc.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oe.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fk.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://gp.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ym.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://we.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bk.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nu.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xc.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nb.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://em.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ob.yuexingan06.cn

[K07] 进制转换
来源：http://eb.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nw.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://py.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://in.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nd.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wq.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://td.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ye.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eq.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://kb.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://zb.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://di.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ln.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://ev.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wq.bookmarksfly.cn

Go:   encoding/gob
来源：http://sa.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://kd.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wq.shxzskj.cn

================================================================================
来源：http://pl.bookmarksfly.cn

L. 网络请求
来源：http://pa.huanxung.cn

================================================================================
来源：http://fw.521024.cn

[L01] 发送 GET 请求
来源：http://rt.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jp.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ri.521024.cn

JS:   await fetch(url)
来源：http://ic.shtwfgs.cn

TS:   await fetch(url)
来源：http://xz.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uo.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://bk.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ru.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yy.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://go.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vl.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bj.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dh.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ti.hahajie.cn


<!-- 参考信息 -->