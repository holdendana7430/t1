代发 wailian999

TS:   throw new Error("错误信息");
来源：http://sp.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://eq.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yl.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ox.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kb.shtwfgs.cn

[H04] 自定义异常类型
来源：http://tg.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://bf.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ah.asd995.cn

JS:   class MyError extends Error {}
来源：http://jy.nicolike.cn

TS:   class MyError extends Error {}
来源：http://eu.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://yx.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://li.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://df.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://xt.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://ua.chemitech.net.cn

Py:   except ValueError as e:
来源：http://te.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rq.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://tl.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://xp.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://vs.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://as.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://jc.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zq.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://di.szsharing.cn

Py:   value = d.get("k") or default
来源：http://sc.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qi.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fo.hahajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ze.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oa.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lu.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://se.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://rn.jianghongdianzi.cn

[H07] 断言
来源：http://pt.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://cr.asd995.cn

PHP:  assert($x > 0);
来源：http://il.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://rp.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://pi.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://ov.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fa.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ep.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://xr.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://fr.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://kq.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gj.9csxet.cn

JS:   e.message;  e.stack
来源：http://lu.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ba.huixinmuqiang.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cr.shxzukj.cn

Go:   err.Error()
来源：http://fs.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://is.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://xi.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://ei.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qy.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mn.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rh.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pf.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yv.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://em.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fa.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ma.szsharing.cn

[H10] 资源自动释放
来源：http://gk.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lp.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jd.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mh.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kv.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://li.9csxet.cn

Go:   defer f.Close()
来源：http://fu.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xk.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eq.shxzukj.cn

================================================================================
来源：http://ys.asd995.cn

I. 正则表达式
来源：http://uj.shtwfgs.cn

================================================================================
来源：http://fk.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://zo.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vi.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://iq.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://tj.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://tc.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ne.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ny.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://xh.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yf.wgjwhj.cn

[I02] 提取所有匹配
来源：http://rg.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://zx.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uq.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mk.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://qg.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zm.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gt.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://mf.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uj.panjiajie.cn

[I03] 提取捕获分组
来源：http://mr.hnjuh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dy.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pw.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lx.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ts.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bu.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pi.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rm.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lg.jianghongdianzi.cn

[I04] 正则替换
来源：http://uh.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vj.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zi.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rh.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pn.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://im.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lh.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mk.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tc.colortex.cn

[I05] 按正则拆分
来源：http://mb.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zt.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cu.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://dp.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://rs.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://tu.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zh.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ms.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ju.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sc.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dl.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://on.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xn.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://np.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ic.bookmarksfly.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oe.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://am.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mk.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://oa.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yp.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ji.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lv.nszjky.cn

TS:   /error/gim
来源：http://dw.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rs.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pd.asd995.cn

Ruby: s.scan(/error/i)
来源：http://lm.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yy.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://qu.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ic.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qz.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://td.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hq.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ng.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hd.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uc.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ld.wgjwhj.cn

================================================================================
来源：http://ne.wgjwhj.cn

J. 日期与时间
来源：http://ke.huixiangedu.cn

================================================================================
来源：http://jh.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://ap.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://na.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cg.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://lq.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://qv.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://di.hnjuh.cn

Go:   time.Now()
来源：http://ft.muxihuayi.cn

Ruby: Time.now
来源：http://nr.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://em.huixinmuqiang.cn

[J02] 格式化输出
来源：http://be.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jq.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uy.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lr.bjjhwx.cn

TS:   d.toISOString()
来源：http://ub.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sf.521024.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lp.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ny.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ic.szsharing.cn

[J03] 字符串解析为日期
来源：http://nl.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kg.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ll.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://jo.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://dh.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vn.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rw.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://tc.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bi.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://rk.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gn.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xj.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vx.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://me.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wd.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ps.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mk.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vs.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://od.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://xd.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qs.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hl.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pb.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://ey.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lh.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://qd.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cx.shxzskj.cn

[J06] 计算两时间之差
来源：http://uy.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://zt.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://sl.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://md.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lp.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sm.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://lv.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://ud.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://ro.muxihuayi.cn

[J07] 比较两个日期
来源：http://id.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://kl.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qn.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fv.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sy.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://io.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vc.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ww.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://sa.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://jx.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sz.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ig.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ct.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dq.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gd.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oy.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://km.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oo.szxytkj.cn

[J09] 时区处理
来源：http://ij.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fr.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zu.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ll.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nh.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wt.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dz.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ph.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yq.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://dq.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ue.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kp.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hs.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uc.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ut.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rh.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xb.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://en.hnjuh.cn

================================================================================
来源：http://vp.huixiangedu.cn

K. JSON 与序列化
来源：http://vn.shxzskj.cn

================================================================================
来源：http://rm.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://kf.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rp.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://by.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://rz.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://ul.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://em.521024.cn

Go:   json.Marshal(obj)
来源：http://zx.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fy.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xk.hahajie.cn

[K02] JSON 字符串转对象
来源：http://ys.muxihuayi.cn

Py:   json.loads(s)
来源：http://th.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ml.shxzukj.cn

JS:   JSON.parse(s)
来源：http://bd.lnxyls.cn

TS:   JSON.parse(s)
来源：http://we.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hy.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://yo.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://lw.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://av.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://gq.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ym.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://td.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ht.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nt.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gs.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nc.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fv.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ja.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://uw.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gc.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fk.szxytkj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dl.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lk.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://io.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nf.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yx.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dg.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://ch.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://fc.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://uz.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://to.hahajie.cn

TS:   structuredClone(obj)
来源：http://hh.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://re.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bn.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zj.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ll.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://od.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://va.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rt.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ri.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ly.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://do.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ig.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aq.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://df.hnjuh.cn

[K07] 进制转换
来源：http://sn.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pk.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://os.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jq.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qe.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ro.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yx.yuntaijiaju.cn


<!-- 参考信息 -->