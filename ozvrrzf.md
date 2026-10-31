代发 wailian999

TS:   throw new Error("错误信息");
来源：http://vy.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hr.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hc.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tj.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://up.szxytkj.cn

[H04] 自定义异常类型
来源：http://mt.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://bj.shtwfgs.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cj.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://pd.szsharing.cn

TS:   class MyError extends Error {}
来源：http://ok.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://gx.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rp.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://jl.asd995.cn

C#:   class MyException : Exception {}
来源：http://mb.szsharing.cn

[H05] 捕获特定类型
来源：http://wc.gzmigu.cn

Py:   except ValueError as e:
来源：http://mt.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ip.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://ni.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ue.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://rm.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oo.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://pd.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hc.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://vf.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://az.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cq.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hj.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://iq.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cy.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ji.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://el.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://cx.haigaiapp.cn

[H07] 断言
来源：http://tg.shxzukj.cn

Py:   assert x > 0, "必须为正"
来源：http://if.newstarts.cn

PHP:  assert($x > 0);
来源：http://nw.colortex.cn

JS:   console.assert(x > 0);
来源：http://cz.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://ct.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://cb.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wt.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xj.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://um.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://zb.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://bk.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mb.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://gr.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hp.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nt.chemitech.net.cn

Go:   err.Error()
来源：http://sk.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://mp.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://bq.asd995.cn

[H09] 带错误码的异常
来源：http://qa.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ot.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nc.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rj.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gk.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zt.asd995.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sl.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dd.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nl.huanxung.cn

[H10] 资源自动释放
来源：http://ix.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kt.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://am.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oy.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cf.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nf.hnjuh.cn

Go:   defer f.Close()
来源：http://hh.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rr.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://me.wgjwhj.cn

================================================================================
来源：http://kw.huixinmuqiang.cn

I. 正则表达式
来源：http://ow.haigaiapp.cn

================================================================================
来源：http://jw.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://ut.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oe.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zo.521024.cn

JS:   /\d+/.test(s)
来源：http://jt.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://mu.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cg.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ei.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://ve.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uy.hnjuh.cn

[I02] 提取所有匹配
来源：http://cy.521024.cn

Py:   re.findall(r"\d+", s)
来源：http://zw.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ku.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uj.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://fj.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wp.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pk.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://lh.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://du.521024.cn

[I03] 提取捕获分组
来源：http://tc.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cu.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://as.nszjky.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jx.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ag.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cb.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fb.muxihuayi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cr.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ov.gzmigu.cn

[I04] 正则替换
来源：http://ld.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sk.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tt.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mn.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vo.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xf.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vy.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ci.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rn.yuexingan06.cn

[I05] 按正则拆分
来源：http://oz.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gf.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xh.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://mo.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://vy.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://zs.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cu.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ci.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ja.bjjhwx.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lp.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gu.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sy.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jz.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hg.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://un.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yk.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fo.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oq.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://ml.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ly.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qi.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dq.chemitech.net.cn

TS:   /error/gim
来源：http://hu.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rs.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sp.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://lm.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lf.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://sr.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ay.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hj.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ka.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dk.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kq.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fs.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ks.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dn.shxzskj.cn

================================================================================
来源：http://em.521024.cn

J. 日期与时间
来源：http://ae.huixiangedu.cn

================================================================================
来源：http://em.huanxung.cn

[J01] 获取当前时间
来源：http://dz.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gh.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vw.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://se.asd995.cn

TS:   new Date();  Date.now()
来源：http://kc.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ug.huixinmuqiang.cn

Go:   time.Now()
来源：http://gk.bookmarksfly.cn

Ruby: Time.now
来源：http://tz.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jm.huixinmuqiang.cn

[J02] 格式化输出
来源：http://mx.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ta.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gp.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iu.jctech888.com.cn

TS:   d.toISOString()
来源：http://pb.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://te.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ox.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ak.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xz.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://tl.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wn.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dq.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://fu.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://nn.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fk.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bf.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://eb.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ga.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://xi.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zu.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cb.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pz.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mw.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tz.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zz.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gl.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jz.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://os.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://kk.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mq.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ov.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ta.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://xn.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mj.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://ki.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mn.521024.cn

[J06] 计算两时间之差
来源：http://oy.521024.cn

Py:   (end - start).total_seconds()
来源：http://zx.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://ud.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ly.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ym.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zo.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://cj.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://vx.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://ya.szxytkj.cn

[J07] 比较两个日期
来源：http://bu.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://kw.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ig.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sz.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ye.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ce.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mg.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ll.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://ig.gzmigu.cn

[J08] 提取年月日与星期
来源：http://cn.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xm.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ik.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rd.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pe.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ce.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qi.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hp.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wa.shtwfgs.cn

[J09] 时区处理
来源：http://oy.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jk.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ec.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bf.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lx.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dh.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ch.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://si.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ux.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://pp.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jh.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vr.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fr.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ub.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nb.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ii.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uu.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ff.nszjky.cn

================================================================================
来源：http://ex.panjiajie.cn

K. JSON 与序列化
来源：http://ph.jianghongdianzi.cn

================================================================================
来源：http://ry.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://eh.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qo.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pe.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://fu.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://bc.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://au.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://zq.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://le.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ml.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://yk.bjjhwx.cn

Py:   json.loads(s)
来源：http://kb.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://du.szsharing.cn

JS:   JSON.parse(s)
来源：http://zt.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://li.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://db.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://bd.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://pt.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cm.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://pd.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wh.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ar.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gj.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ha.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rm.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ho.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ul.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wy.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://vf.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eh.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bw.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vw.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xg.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zz.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wx.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xl.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dg.newstarts.cn

[K05] 深拷贝对象
来源：http://ks.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://mu.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://fr.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://my.521024.cn

TS:   structuredClone(obj)
来源：http://qw.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sb.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wr.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jt.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yz.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://yp.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fr.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lf.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yh.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://is.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hs.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bx.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bo.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xc.yuntaijiaju.cn

[K07] 进制转换
来源：http://pw.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nw.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pi.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rc.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zg.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fr.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://it.huixinmuqiang.cn


<!-- 参考信息 -->