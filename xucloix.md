代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ke.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ff.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://hx.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://ue.nszjky.cn

[H07] 断言
来源：http://gx.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://xi.szxytkj.cn

PHP:  assert($x > 0);
来源：http://nj.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://uu.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://sk.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://ic.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tb.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lx.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://li.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://ul.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://xe.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ui.9csxet.cn

JS:   e.message;  e.stack
来源：http://in.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dk.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yn.haigaiapp.cn

Go:   err.Error()
来源：http://nb.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://pe.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://om.shtwfgs.cn

[H09] 带错误码的异常
来源：http://lm.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kj.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hp.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://no.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bb.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ll.asd995.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zr.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pv.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rc.szsharing.cn

[H10] 资源自动释放
来源：http://kw.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fz.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iv.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jy.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ce.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ee.colortex.cn

Go:   defer f.Close()
来源：http://cg.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://va.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nv.jianghongdianzi.cn

================================================================================
来源：http://nk.shtwfgs.cn

I. 正则表达式
来源：http://vy.chemitech.net.cn

================================================================================
来源：http://tm.9csxet.cn

[I01] 判断是否匹配
来源：http://zh.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ie.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yk.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://rm.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://uy.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nn.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yr.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://kx.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tp.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://pk.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://kf.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nr.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jy.colortex.cn

TS:   s.match(/\d+/g)
来源：http://ib.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sx.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bd.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://tf.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://he.asd995.cn

[I03] 提取捕获分组
来源：http://jk.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bt.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gd.nszjky.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bs.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ia.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qg.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vj.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://te.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jp.9csxet.cn

[I04] 正则替换
来源：http://mg.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pv.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://up.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jr.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bs.haigaiapp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wb.huanxung.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gw.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fh.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zl.muxihuayi.cn

[I05] 按正则拆分
来源：http://ry.nszjky.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://we.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mc.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://md.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://pw.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://rv.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://im.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mq.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ur.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://su.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xx.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wa.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pk.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vd.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cu.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hs.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yv.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ec.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://eg.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dk.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tk.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mj.szsharing.cn

TS:   /error/gim
来源：http://tv.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xy.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jj.colortex.cn

Ruby: s.scan(/error/i)
来源：http://uv.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sd.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://ri.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nf.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lc.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gf.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xs.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hh.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sg.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bt.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kp.panjiajie.cn

================================================================================
来源：http://lu.shxzskj.cn

J. 日期与时间
来源：http://rs.muxihuayi.cn

================================================================================
来源：http://qo.shtwfgs.cn

[J01] 获取当前时间
来源：http://gp.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zi.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kr.hahajie.cn

JS:   new Date();  Date.now()
来源：http://ew.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://qj.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://aw.nszjky.cn

Go:   time.Now()
来源：http://zp.muxihuayi.cn

Ruby: Time.now
来源：http://eb.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ta.panjiajie.cn

[J02] 格式化输出
来源：http://zo.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ik.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nq.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ky.hahajie.cn

TS:   d.toISOString()
来源：http://im.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fl.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://me.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lw.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qd.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://oa.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ln.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lh.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://xy.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://zo.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hz.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mt.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://om.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qg.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://me.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://la.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uq.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kh.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tt.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gv.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://us.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mj.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ej.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://rb.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://nc.jianghongdianzi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pr.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hy.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://co.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://pl.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sq.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://xn.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tm.huixiangedu.cn

[J06] 计算两时间之差
来源：http://tt.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://xx.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://dr.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yg.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ys.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hv.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://xn.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://fc.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://rr.jctech888.com.cn

[J07] 比较两个日期
来源：http://zn.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://cx.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qg.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ce.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vy.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ve.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yq.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://au.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://hf.colortex.cn

[J08] 提取年月日与星期
来源：http://ij.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://go.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hy.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oz.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bd.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vx.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mz.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ia.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://er.nszjky.cn

[J09] 时区处理
来源：http://ic.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://la.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://em.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ji.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ut.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cn.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xc.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kh.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yy.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://gm.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gg.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ox.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://me.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wm.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cu.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bx.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qz.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://un.asd995.cn

================================================================================
来源：http://mq.huanxung.cn

K. JSON 与序列化
来源：http://qu.yuexingan06.cn

================================================================================
来源：http://jh.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://jz.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ty.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mh.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://iz.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://hj.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ye.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://pi.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tw.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tl.hahajie.cn

[K02] JSON 字符串转对象
来源：http://pw.hahajie.cn

Py:   json.loads(s)
来源：http://jg.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://al.colortex.cn

JS:   JSON.parse(s)
来源：http://fn.gzmigu.cn

TS:   JSON.parse(s)
来源：http://hx.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iq.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://oc.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://he.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pj.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://jv.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vn.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bm.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oy.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uf.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jz.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://au.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tk.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qi.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://oi.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ta.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fl.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rv.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mr.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wj.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bt.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oc.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rj.hnjuh.cn

[K05] 深拷贝对象
来源：http://vo.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://bo.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://st.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://fu.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://vy.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vh.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mt.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ls.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hf.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://kk.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vt.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yk.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xv.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mm.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cw.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mq.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zn.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dn.yuntaijiaju.cn

[K07] 进制转换
来源：http://pi.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fe.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xu.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qh.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gp.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mf.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ym.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ce.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jc.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://eh.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://vs.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sa.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://aq.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://in.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://of.lnxyls.cn

Go:   encoding/gob
来源：http://kk.bookmarksfly.cn

Ruby: Marshal.dump(obj)
来源：http://ew.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cc.colortex.cn

================================================================================
来源：http://uj.chemitech.net.cn

L. 网络请求
来源：http://uy.bookmarksfly.cn

================================================================================
来源：http://va.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://sl.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xx.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lm.shxzskj.cn

JS:   await fetch(url)
来源：http://ue.bookmarksfly.cn

TS:   await fetch(url)
来源：http://yk.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bk.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://jt.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lf.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rb.szxytkj.cn

[L02] 发送 POST JSON
来源：http://qv.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://be.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sf.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ol.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gc.bjjhwx.cn


<!-- 参考信息 -->