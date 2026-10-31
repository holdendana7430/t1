代发 wailian999

TS:   throw new Error("错误信息");
来源：http://qd.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nc.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ek.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fk.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cf.huixiangedu.cn

[H04] 自定义异常类型
来源：http://oy.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://zf.shtwfgs.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gg.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://aa.asd995.cn

TS:   class MyError extends Error {}
来源：http://sn.9csxet.cn

Java: class MyException extends RuntimeException {}
来源：http://hg.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pn.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://mh.521024.cn

C#:   class MyException : Exception {}
来源：http://wi.gzmigu.cn

[H05] 捕获特定类型
来源：http://uu.shxzukj.cn

Py:   except ValueError as e:
来源：http://ok.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fz.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://su.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://gy.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://fx.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dk.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://ay.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zh.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://jj.colortex.cn

Py:   value = d.get("k") or default
来源：http://wl.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yd.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zr.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vf.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ma.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kj.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://ed.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://iz.hahajie.cn

[H07] 断言
来源：http://lh.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://sg.lnxyls.cn

PHP:  assert($x > 0);
来源：http://dv.huanxung.cn

JS:   console.assert(x > 0);
来源：http://gb.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://et.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://jx.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ll.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uq.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://uy.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://gt.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://tm.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ne.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://qf.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rh.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ya.asd995.cn

Go:   err.Error()
来源：http://lq.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://et.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://vi.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://vz.nszjky.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jh.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uc.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qx.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ia.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://id.nszjky.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://da.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gj.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://re.asd995.cn

[H10] 资源自动释放
来源：http://eo.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mz.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hs.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xf.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vs.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ja.yuexingan06.cn

Go:   defer f.Close()
来源：http://vv.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ht.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ju.bjjhwx.cn

================================================================================
来源：http://nk.yuntaijiaju.cn

I. 正则表达式
来源：http://kf.colortex.cn

================================================================================
来源：http://vp.bjjhwx.cn

[I01] 判断是否匹配
来源：http://mq.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yl.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yd.nicolike.cn

JS:   /\d+/.test(s)
来源：http://qt.huanxung.cn

TS:   /\d+/.test(s)
来源：http://li.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wt.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ez.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://dr.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ym.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://wt.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://kw.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zd.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xw.asd995.cn

TS:   s.match(/\d+/g)
来源：http://sk.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kx.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ox.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://mf.muxihuayi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://po.shxzukj.cn

[I03] 提取捕获分组
来源：http://uo.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ng.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ey.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hn.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wf.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jw.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sk.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ki.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fl.shtwfgs.cn

[I04] 正则替换
来源：http://is.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ak.huanxung.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xd.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tn.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ad.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ed.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://aq.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xk.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://th.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://fe.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ha.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://la.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://tr.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://xj.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://eb.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cr.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://em.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ur.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yt.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://um.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://on.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xa.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vb.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bc.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fd.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oy.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kw.szsharing.cn

[I07] 忽略大小写与多行模式
来源：http://ev.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ko.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ww.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://er.gzmigu.cn

TS:   /error/gim
来源：http://zk.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://or.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rm.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://pn.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xk.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://tw.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tq.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mi.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tm.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dd.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hg.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rv.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oy.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pn.bookmarksfly.cn

================================================================================
来源：http://bp.chemitech.net.cn

J. 日期与时间
来源：http://wd.9csxet.cn

================================================================================
来源：http://no.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://yl.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tx.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://od.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://bv.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://lr.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://js.lnxyls.cn

Go:   time.Now()
来源：http://ox.shtwfgs.cn

Ruby: Time.now
来源：http://fs.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ur.shtwfgs.cn

[J02] 格式化输出
来源：http://ts.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lt.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tl.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lg.hahajie.cn

TS:   d.toISOString()
来源：http://wn.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://os.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xb.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lq.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ck.shxzukj.cn

[J03] 字符串解析为日期
来源：http://dy.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mj.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xv.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://dk.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://ub.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qb.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rz.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://kw.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nb.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://xe.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nt.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ix.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iq.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://oo.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zd.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ij.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yf.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fh.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://nc.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://ed.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://eh.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wa.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gk.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://dd.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hh.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://rc.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cj.nszjky.cn

[J06] 计算两时间之差
来源：http://nv.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://cp.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://wp.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://in.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://su.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mx.521024.cn

Go:   end.Sub(start).Hours()
来源：http://pf.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://te.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://ie.521024.cn

[J07] 比较两个日期
来源：http://pj.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://vq.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zh.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rs.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://po.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jv.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mm.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mn.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://gg.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://rt.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kh.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ir.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fk.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dd.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cl.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cr.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wq.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rt.muxihuayi.cn

[J09] 时区处理
来源：http://xl.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wu.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hq.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hq.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fl.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oi.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qa.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uq.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mg.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://ga.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nw.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eq.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://si.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nq.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pl.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zt.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lt.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cy.hahajie.cn

================================================================================
来源：http://sc.huixiangedu.cn

K. JSON 与序列化
来源：http://tp.szsharing.cn

================================================================================
来源：http://fu.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://ue.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dt.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hp.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://ii.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://cv.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gq.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://jx.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://os.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rh.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://eh.hnjuh.cn

Py:   json.loads(s)
来源：http://my.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://em.nicolike.cn

JS:   JSON.parse(s)
来源：http://jn.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://kk.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wo.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://cb.nicolike.cn

Ruby: JSON.parse(s)
来源：http://pw.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lb.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://fi.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pl.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qe.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ec.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://js.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ij.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cr.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kh.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bx.newstarts.cn

[K04] 读取 JSON 文件
来源：http://jl.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tj.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qd.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lu.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bb.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ja.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ir.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bz.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yf.bjjhwx.cn

[K05] 深拷贝对象
来源：http://qw.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://dl.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://yb.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://in.lnxyls.cn

TS:   structuredClone(obj)
来源：http://vm.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ng.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://of.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qh.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ae.nicolike.cn

[K06] 解析 URL 查询串
来源：http://ab.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://us.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nq.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ix.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ts.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kf.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sp.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rs.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kg.colortex.cn

[K07] 进制转换
来源：http://sw.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yy.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oo.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fq.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gw.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oj.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xo.asd995.cn


<!-- 参考信息 -->