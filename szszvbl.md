代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://bb.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ex.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zo.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qg.521024.cn

[H03] 主动抛出异常
来源：http://oz.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://ri.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pp.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://yp.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://hl.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dj.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xt.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jm.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://en.haigaiapp.cn

[H04] 自定义异常类型
来源：http://yj.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://jc.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dm.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://yt.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://kw.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://fk.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fx.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://xs.521024.cn

C#:   class MyException : Exception {}
来源：http://zc.hnjuh.cn

[H05] 捕获特定类型
来源：http://pm.nszjky.cn

Py:   except ValueError as e:
来源：http://zh.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ib.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://zx.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://mz.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://so.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xf.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://vz.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kz.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://rt.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://so.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rp.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://il.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jb.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://py.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://he.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://jy.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://vo.szxytkj.cn

[H07] 断言
来源：http://tw.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://kf.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://bi.newstarts.cn

JS:   console.assert(x > 0);
来源：http://ni.asd995.cn

TS:   console.assert(x > 0);
来源：http://yl.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://jh.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://me.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cq.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://hh.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://kg.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://cr.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ti.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://jv.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xm.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cc.shxzukj.cn

Go:   err.Error()
来源：http://mq.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://xv.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://oo.wgjwhj.cn

[H09] 带错误码的异常
来源：http://rp.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pk.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://le.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yb.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vq.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yr.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jm.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ym.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ml.bookmarksfly.cn

[H10] 资源自动释放
来源：http://sv.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kn.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xj.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vr.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kt.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bp.521024.cn

Go:   defer f.Close()
来源：http://vj.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kv.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dz.hahajie.cn

================================================================================
来源：http://pg.hnjuh.cn

I. 正则表达式
来源：http://jo.gzmigu.cn

================================================================================
来源：http://xj.nicolike.cn

[I01] 判断是否匹配
来源：http://vr.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nu.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://au.szsharing.cn

JS:   /\d+/.test(s)
来源：http://if.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://qm.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wd.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fx.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://bi.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vi.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://ye.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://gh.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qy.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ij.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://he.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wk.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iq.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://qq.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vc.szxytkj.cn

[I03] 提取捕获分组
来源：http://wm.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oc.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yp.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kj.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fo.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nb.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jm.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ls.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iw.szxytkj.cn

[I04] 正则替换
来源：http://nq.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dj.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sj.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ks.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dk.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vb.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nc.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://op.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://br.newstarts.cn

[I05] 按正则拆分
来源：http://bx.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mm.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jz.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://wz.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://qo.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://zg.bookmarksfly.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jh.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vp.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ii.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vo.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://di.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wl.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tg.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wj.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gf.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mc.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://em.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://id.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://ix.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ki.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hi.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vb.panjiajie.cn

TS:   /error/gim
来源：http://gq.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lp.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pv.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://ec.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pm.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://eb.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xb.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zi.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://up.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fd.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qz.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qu.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cg.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ws.shtwfgs.cn

================================================================================
来源：http://qe.huanxung.cn

J. 日期与时间
来源：http://vw.yuexingan06.cn

================================================================================
来源：http://fi.huanxung.cn

[J01] 获取当前时间
来源：http://tq.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zp.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mt.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://dy.asd995.cn

TS:   new Date();  Date.now()
来源：http://on.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cw.muxihuayi.cn

Go:   time.Now()
来源：http://bs.hnjuh.cn

Ruby: Time.now
来源：http://xw.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sz.haigaiapp.cn

[J02] 格式化输出
来源：http://ux.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tv.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fj.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oc.jctech888.com.cn

TS:   d.toISOString()
来源：http://fi.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xc.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wf.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dr.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ak.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://zk.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://va.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ol.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://eo.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://xt.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sp.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vx.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://ec.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wk.nszjky.cn

[J04] 时间戳与日期互转
来源：http://oy.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://za.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cx.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mj.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wd.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://we.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wv.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mv.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rd.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://fk.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://aj.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xd.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ht.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kt.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://ds.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ey.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://sp.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://di.bjjhwx.cn

[J06] 计算两时间之差
来源：http://pl.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://bt.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://ih.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://is.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jn.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qr.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://wh.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://mz.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://er.asd995.cn

[J07] 比较两个日期
来源：http://uo.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://kw.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tl.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nd.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ee.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fm.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mj.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ta.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://yt.panjiajie.cn

[J08] 提取年月日与星期
来源：http://wv.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uf.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xo.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yb.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cf.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jw.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yu.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oe.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sa.bookmarksfly.cn

[J09] 时区处理
来源：http://vf.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ne.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qy.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yv.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nf.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qm.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://re.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dv.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fp.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://en.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zl.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bz.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pm.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://al.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wr.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iu.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://el.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ni.huanxung.cn

================================================================================
来源：http://ea.bjjhwx.cn

K. JSON 与序列化
来源：http://ox.szxytkj.cn

================================================================================
来源：http://kh.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://pt.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ng.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hx.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://sc.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://rz.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bw.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://ol.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dz.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bw.521024.cn

[K02] JSON 字符串转对象
来源：http://bv.shxzskj.cn

Py:   json.loads(s)
来源：http://ml.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rt.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://oj.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://kh.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ic.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://le.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://ct.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sp.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ak.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://es.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xc.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zv.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pr.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xh.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cl.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pi.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ti.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://yj.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ag.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fb.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ua.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ir.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lk.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://it.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ew.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://de.shxzskj.cn

[K05] 深拷贝对象
来源：http://hb.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://po.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://as.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://vq.nicolike.cn

TS:   structuredClone(obj)
来源：http://rf.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sn.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hb.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bx.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kv.colortex.cn

[K06] 解析 URL 查询串
来源：http://op.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xv.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yb.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bd.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ct.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fg.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wm.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bq.huanxung.cn


<!-- 参考信息 -->