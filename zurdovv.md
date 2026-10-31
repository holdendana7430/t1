代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xo.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ef.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://cl.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://ec.lnxyls.cn

[H07] 断言
来源：http://ry.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://yf.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://jr.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://ji.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://gb.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://eh.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ey.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kp.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://us.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://wy.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://le.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yy.szsharing.cn

JS:   e.message;  e.stack
来源：http://yd.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yb.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ii.yuntaijiaju.cn

Go:   err.Error()
来源：http://va.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://xa.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://lv.gzmigu.cn

[H09] 带错误码的异常
来源：http://an.shtwfgs.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fj.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://el.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zq.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ot.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rd.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uo.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ty.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xy.asd995.cn

[H10] 资源自动释放
来源：http://ot.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vt.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nc.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ak.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ie.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://es.haigaiapp.cn

Go:   defer f.Close()
来源：http://tj.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zl.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rs.newstarts.cn

================================================================================
来源：http://qz.szsharing.cn

I. 正则表达式
来源：http://dg.muxihuayi.cn

================================================================================
来源：http://sb.jctech888.com.cn

[I01] 判断是否匹配
来源：http://so.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ss.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://aq.521024.cn

JS:   /\d+/.test(s)
来源：http://sz.asd995.cn

TS:   /\d+/.test(s)
来源：http://lp.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ap.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oz.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://hr.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nz.jctech888.com.cn

[I02] 提取所有匹配
来源：http://ou.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://xj.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ht.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kr.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://kq.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ex.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fd.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://zp.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kq.hahajie.cn

[I03] 提取捕获分组
来源：http://yy.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ok.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://un.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tu.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rj.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bw.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rs.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://it.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mn.521024.cn

[I04] 正则替换
来源：http://oe.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lz.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://py.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zo.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nw.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://un.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hk.nicolike.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wi.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wa.gzmigu.cn

[I05] 按正则拆分
来源：http://iw.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oo.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ic.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://rw.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://il.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://fd.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uw.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zd.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pl.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cr.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kt.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wx.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mv.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zo.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ow.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mc.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fr.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xl.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://xu.szxytkj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zi.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uu.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://em.newstarts.cn

TS:   /error/gim
来源：http://ar.yuexingan06.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kp.hnjuh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ej.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://si.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nh.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://bf.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fj.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yh.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qv.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xi.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nh.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hm.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yc.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tf.jianghongdianzi.cn

================================================================================
来源：http://xe.lnxyls.cn

J. 日期与时间
来源：http://bc.szxytkj.cn

================================================================================
来源：http://um.szxytkj.cn

[J01] 获取当前时间
来源：http://fv.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bw.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bl.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://xy.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://zc.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fp.szxytkj.cn

Go:   time.Now()
来源：http://cm.9csxet.cn

Ruby: Time.now
来源：http://im.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tc.shtwfgs.cn

[J02] 格式化输出
来源：http://xp.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://am.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://os.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rz.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://bn.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gm.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dq.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xz.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oc.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://or.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tq.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jj.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://me.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://ee.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mk.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rv.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://lt.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yh.huanxung.cn

[J04] 时间戳与日期互转
来源：http://aq.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xj.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ss.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hp.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bi.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kx.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ed.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lm.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jv.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://hh.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://sy.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sx.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wj.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cz.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://qa.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ws.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://ws.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zz.shxzskj.cn

[J06] 计算两时间之差
来源：http://cl.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://wr.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://vw.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hb.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xb.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zh.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://vp.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://ya.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://lh.chemitech.net.cn

[J07] 比较两个日期
来源：http://pd.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://zx.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ps.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jx.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ou.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ci.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wr.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://la.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://rc.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://fi.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mk.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ls.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tu.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://py.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vn.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mi.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ks.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vl.haigaiapp.cn

[J09] 时区处理
来源：http://gn.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lb.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pu.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ec.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jd.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vl.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mf.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zq.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pt.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://gl.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nj.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xd.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kj.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iw.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pj.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ja.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zr.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nh.shxzskj.cn

================================================================================
来源：http://oo.jianghongdianzi.cn

K. JSON 与序列化
来源：http://nh.muxihuayi.cn

================================================================================
来源：http://dq.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://zq.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ql.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pt.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://uv.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://qh.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zz.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://rp.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tj.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ee.newstarts.cn

[K02] JSON 字符串转对象
来源：http://xp.nszjky.cn

Py:   json.loads(s)
来源：http://mk.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lb.newstarts.cn

JS:   JSON.parse(s)
来源：http://ge.shxzskj.cn

TS:   JSON.parse(s)
来源：http://bf.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://la.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://aj.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://ar.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aw.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://lg.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kq.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qr.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kg.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ca.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aq.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wo.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gt.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hd.9csxet.cn

[K04] 读取 JSON 文件
来源：http://gm.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jo.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uf.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ee.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yl.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gq.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zh.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ui.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gw.bjjhwx.cn

[K05] 深拷贝对象
来源：http://wz.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://bp.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://sg.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://zp.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://zu.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sx.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hm.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://us.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qg.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://se.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rc.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qo.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ep.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gk.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ld.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rc.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wm.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ob.asd995.cn

[K07] 进制转换
来源：http://wy.panjiajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ts.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lx.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wu.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zs.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pq.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bn.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bc.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aa.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://xt.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://aq.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vn.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ui.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://kx.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ai.nicolike.cn

Go:   encoding/gob
来源：http://qu.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://mn.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tz.nicolike.cn

================================================================================
来源：http://lc.muxihuayi.cn

L. 网络请求
来源：http://fa.huixiangedu.cn

================================================================================
来源：http://jj.521024.cn

[L01] 发送 GET 请求
来源：http://km.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jg.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dj.asd995.cn

JS:   await fetch(url)
来源：http://uu.newstarts.cn

TS:   await fetch(url)
来源：http://pg.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nl.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://xi.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gl.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xi.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://gm.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bo.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sn.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vv.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gf.9csxet.cn


<!-- 参考信息 -->