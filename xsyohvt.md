代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sd.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zg.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://qt.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://oe.wgjwhj.cn

[H07] 断言
来源：http://lf.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://dj.newstarts.cn

PHP:  assert($x > 0);
来源：http://qn.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://jy.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://ec.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://ou.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hl.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://me.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://mu.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://mq.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://ot.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nb.newstarts.cn

JS:   e.message;  e.stack
来源：http://hg.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vj.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kr.panjiajie.cn

Go:   err.Error()
来源：http://ge.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://ts.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://qt.huixiangedu.cn

[H09] 带错误码的异常
来源：http://zx.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zb.muxihuayi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hl.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://em.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qw.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gd.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://at.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ew.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ex.9csxet.cn

[H10] 资源自动释放
来源：http://mt.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qc.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qx.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ix.chemitech.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gl.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oi.chemitech.net.cn

Go:   defer f.Close()
来源：http://bd.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pm.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mg.yuntaijiaju.cn

================================================================================
来源：http://hy.nszjky.cn

I. 正则表达式
来源：http://ar.jianghongdianzi.cn

================================================================================
来源：http://ke.shxzskj.cn

[I01] 判断是否匹配
来源：http://au.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pf.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sj.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://di.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://vq.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wm.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://th.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://sa.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://co.yuexingan06.cn

[I02] 提取所有匹配
来源：http://hw.shxzukj.cn

Py:   re.findall(r"\d+", s)
来源：http://ah.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gl.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zv.colortex.cn

TS:   s.match(/\d+/g)
来源：http://bx.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qf.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fz.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://uq.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lw.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://ld.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zm.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tj.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vb.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ry.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wl.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://go.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mh.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dx.shtwfgs.cn

[I04] 正则替换
来源：http://hx.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hr.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bp.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jk.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bq.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ut.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sg.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vr.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bp.newstarts.cn

[I05] 按正则拆分
来源：http://jp.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zo.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xj.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://mf.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://pk.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://fo.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qy.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fr.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bc.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lq.hnjuh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://we.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xx.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ia.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://et.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yv.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hc.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fy.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nk.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://tz.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nv.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fj.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qb.yuexingan06.cn

TS:   /error/gim
来源：http://af.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wb.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wj.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://zg.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bh.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://jn.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kh.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mo.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gl.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://de.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ok.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nt.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hg.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nx.szxytkj.cn

================================================================================
来源：http://eb.newstarts.cn

J. 日期与时间
来源：http://us.9csxet.cn

================================================================================
来源：http://dc.nszjky.cn

[J01] 获取当前时间
来源：http://zn.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jf.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iv.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://ff.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://jl.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ow.nszjky.cn

Go:   time.Now()
来源：http://nb.muxihuayi.cn

Ruby: Time.now
来源：http://hh.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bo.panjiajie.cn

[J02] 格式化输出
来源：http://pp.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yf.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ci.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qt.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://vw.colortex.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vv.newstarts.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jx.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nn.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bp.szsharing.cn

[J03] 字符串解析为日期
来源：http://yx.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rp.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bc.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://gb.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://ej.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nr.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wg.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://jc.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dq.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://cb.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xj.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bm.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://go.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lj.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ck.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nd.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mo.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://li.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://mk.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://bc.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gi.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://al.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mq.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ax.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lt.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://sj.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tz.bjjhwx.cn

[J06] 计算两时间之差
来源：http://cp.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://gd.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://mu.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://og.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lk.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pk.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://oj.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://cq.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://xq.newstarts.cn

[J07] 比较两个日期
来源：http://gv.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://ge.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ek.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://py.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fm.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ay.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zx.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zb.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://de.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://ra.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uk.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gn.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sn.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yj.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rg.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bf.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vb.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gd.9csxet.cn

[J09] 时区处理
来源：http://wv.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zu.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mh.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fj.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jn.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fe.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://km.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vs.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zg.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://wx.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yn.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nl.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sl.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cj.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gu.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://se.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gn.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ty.nicolike.cn

================================================================================
来源：http://hd.jianghongdianzi.cn

K. JSON 与序列化
来源：http://id.hahajie.cn

================================================================================
来源：http://kk.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://oq.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eu.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ac.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://ei.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://he.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iz.nicolike.cn

Go:   json.Marshal(obj)
来源：http://ae.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://om.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jy.szsharing.cn

[K02] JSON 字符串转对象
来源：http://ag.yuexingan06.cn

Py:   json.loads(s)
来源：http://qu.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lq.colortex.cn

JS:   JSON.parse(s)
来源：http://lt.szxytkj.cn

TS:   JSON.parse(s)
来源：http://rz.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oy.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://ma.hahajie.cn

Ruby: JSON.parse(s)
来源：http://le.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mb.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://xq.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hi.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fm.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hf.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ad.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ei.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eo.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pg.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cz.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://bw.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gb.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jh.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ef.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://io.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mg.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wo.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ez.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pz.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://vo.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://ga.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://zm.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://ui.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://pk.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ok.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hw.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ci.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ev.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://fa.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pg.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nc.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pc.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rh.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vt.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lx.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ii.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://es.muxihuayi.cn

[K07] 进制转换
来源：http://pl.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iu.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eb.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cd.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://po.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://li.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xb.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lr.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gu.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://il.colortex.cn

Py:   pickle.dumps(obj)
来源：http://db.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ky.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://gv.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://wf.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jv.gzmigu.cn

Go:   encoding/gob
来源：http://xb.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://fn.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xr.wgjwhj.cn

================================================================================
来源：http://oj.muxihuayi.cn

L. 网络请求
来源：http://lc.huixiangedu.cn

================================================================================
来源：http://gz.shxzskj.cn

[L01] 发送 GET 请求
来源：http://bk.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ed.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gq.lnxyls.cn

JS:   await fetch(url)
来源：http://cm.shtwfgs.cn

TS:   await fetch(url)
来源：http://pu.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jc.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://pj.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://di.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mu.panjiajie.cn

[L02] 发送 POST JSON
来源：http://bi.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rc.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zc.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://av.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gq.521024.cn


<!-- 参考信息 -->