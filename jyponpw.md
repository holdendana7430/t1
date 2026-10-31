代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ka.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ek.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://gb.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://ul.colortex.cn

[H07] 断言
来源：http://kn.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://go.panjiajie.cn

PHP:  assert($x > 0);
来源：http://hz.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://zy.szsharing.cn

TS:   console.assert(x > 0);
来源：http://jh.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://cf.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kq.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yd.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://iy.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://vi.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://qt.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lt.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://cc.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ci.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vt.hnjuh.cn

Go:   err.Error()
来源：http://dy.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://fl.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://ne.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://ob.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bd.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ms.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dw.newstarts.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fa.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yr.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lz.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nq.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fq.yuexingan06.cn

[H10] 资源自动释放
来源：http://fk.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dj.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vx.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ne.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mo.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ze.szxytkj.cn

Go:   defer f.Close()
来源：http://wi.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ot.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wy.nszjky.cn

================================================================================
来源：http://ay.shtwfgs.cn

I. 正则表达式
来源：http://uw.huanxung.cn

================================================================================
来源：http://jp.jctech888.com.cn

[I01] 判断是否匹配
来源：http://wg.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bd.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zl.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://ct.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://hs.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ws.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wh.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://pm.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uq.jctech888.com.cn

[I02] 提取所有匹配
来源：http://nd.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://nx.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nm.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ys.bjjhwx.cn

TS:   s.match(/\d+/g)
来源：http://pp.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://la.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sg.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://wj.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ut.gzmigu.cn

[I03] 提取捕获分组
来源：http://wd.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ua.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ib.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nm.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kk.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jz.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://to.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lw.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qc.szxytkj.cn

[I04] 正则替换
来源：http://zv.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ap.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gs.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cg.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oe.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ap.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ac.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ix.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bl.muxihuayi.cn

[I05] 按正则拆分
来源：http://no.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hy.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tv.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://fy.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://tq.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://th.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mk.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bs.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pk.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://on.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sl.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nr.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nl.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ar.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ra.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mx.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cc.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hd.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://hc.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vg.colortex.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sf.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://td.chemitech.net.cn

TS:   /error/gim
来源：http://io.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://em.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dv.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://lb.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ww.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://lu.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xe.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tw.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cb.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zz.bookmarksfly.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ot.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gk.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mi.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hy.shxzukj.cn

================================================================================
来源：http://qa.nszjky.cn

J. 日期与时间
来源：http://fp.huixiangedu.cn

================================================================================
来源：http://lu.haigaiapp.cn

[J01] 获取当前时间
来源：http://cx.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://op.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://av.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://ri.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://iz.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zu.9csxet.cn

Go:   time.Now()
来源：http://bf.huanxung.cn

Ruby: Time.now
来源：http://cs.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://os.hnjuh.cn

[J02] 格式化输出
来源：http://fz.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eq.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hb.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ct.szxytkj.cn

TS:   d.toISOString()
来源：http://al.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tr.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mz.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://km.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qp.9csxet.cn

[J03] 字符串解析为日期
来源：http://hb.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jt.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gz.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://mh.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://hh.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hi.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rk.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://ar.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qt.nszjky.cn

[J04] 时间戳与日期互转
来源：http://ng.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cz.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tc.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tb.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ex.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dw.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mo.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pu.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eh.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://tn.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://wh.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gg.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uy.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gc.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://vd.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pz.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://ek.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rx.shtwfgs.cn

[J06] 计算两时间之差
来源：http://ud.colortex.cn

Py:   (end - start).total_seconds()
来源：http://ux.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://uw.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iv.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gb.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cs.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://xw.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://kf.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://ld.nicolike.cn

[J07] 比较两个日期
来源：http://eg.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://rx.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://em.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://em.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wb.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ko.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sh.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ii.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://eq.lnxyls.cn

[J08] 提取年月日与星期
来源：http://zm.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qg.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nm.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qk.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rp.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uu.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://it.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://it.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pq.yuntaijiaju.cn

[J09] 时区处理
来源：http://bk.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fa.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qp.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://db.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jj.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pl.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gf.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hh.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dp.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://om.jctech888.com.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vq.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://na.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://in.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tg.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zq.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mj.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gj.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pz.9csxet.cn

================================================================================
来源：http://ec.bookmarksfly.cn

K. JSON 与序列化
来源：http://pb.newstarts.cn

================================================================================
来源：http://sn.wgjwhj.cn

[K01] 对象转 JSON 字符串
来源：http://pu.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bl.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kv.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://yx.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://ud.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ix.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://kn.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lt.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mv.colortex.cn

[K02] JSON 字符串转对象
来源：http://pz.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://cq.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zj.nicolike.cn

JS:   JSON.parse(s)
来源：http://wa.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://ug.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vz.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://lb.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://ai.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fx.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://nx.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://td.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qw.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ro.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oe.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sr.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fy.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rj.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hh.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://it.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pq.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iv.szsharing.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ry.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hs.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bq.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hu.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ic.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dt.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://ge.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://gh.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://kd.huanxung.cn

JS:   structuredClone(obj)
来源：http://fs.nicolike.cn

TS:   structuredClone(obj)
来源：http://aq.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qy.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rt.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xf.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bh.9csxet.cn

[K06] 解析 URL 查询串
来源：http://qc.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jl.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sj.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rs.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fw.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xo.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hc.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bk.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ff.haigaiapp.cn

[K07] 进制转换
来源：http://ao.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zf.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nx.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hq.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ry.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gj.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iw.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hb.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ay.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://bn.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://ls.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xy.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://eq.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://cn.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vr.haigaiapp.cn

Go:   encoding/gob
来源：http://nb.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://jj.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://da.huixiangedu.cn

================================================================================
来源：http://fi.gzmigu.cn

L. 网络请求
来源：http://yn.newstarts.cn

================================================================================
来源：http://kl.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://tg.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vz.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xq.huanxung.cn

JS:   await fetch(url)
来源：http://ku.szxytkj.cn

TS:   await fetch(url)
来源：http://ax.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xk.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://ra.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uj.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eu.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://fj.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://by.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jp.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cj.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://so.jctech888.com.cn


<!-- 参考信息 -->