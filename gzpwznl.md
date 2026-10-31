代发 wailian999

TS:   throw new Error("错误信息");
来源：http://qh.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vw.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qc.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qs.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sz.nszjky.cn

[H04] 自定义异常类型
来源：http://oz.asd995.cn

Py:   class MyError(Exception): pass
来源：http://ni.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ep.nszjky.cn

JS:   class MyError extends Error {}
来源：http://lw.nicolike.cn

TS:   class MyError extends Error {}
来源：http://ar.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://ao.jctech888.com.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mz.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://ai.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://vb.haigaiapp.cn

[H05] 捕获特定类型
来源：http://fl.huixiangedu.cn

Py:   except ValueError as e:
来源：http://ly.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iu.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://te.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://gh.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://od.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ks.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://qs.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uf.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://ux.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://mo.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xt.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xi.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://el.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jx.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ls.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://aj.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://mx.asd995.cn

[H07] 断言
来源：http://ux.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://ch.szxytkj.cn

PHP:  assert($x > 0);
来源：http://ux.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://xd.huanxung.cn

TS:   console.assert(x > 0);
来源：http://iv.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://dc.yuntaijiaju.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wu.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dr.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://pt.chemitech.net.cn

[H08] 获取错误信息与堆栈
来源：http://bi.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://fj.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://da.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://ob.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gt.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xf.muxihuayi.cn

Go:   err.Error()
来源：http://gj.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://da.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://bb.haigaiapp.cn

[H09] 带错误码的异常
来源：http://vv.nszjky.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cs.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wj.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://du.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zx.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bh.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ic.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mg.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nj.szxytkj.cn

[H10] 资源自动释放
来源：http://or.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://iu.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qj.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://es.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vf.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ea.szsharing.cn

Go:   defer f.Close()
来源：http://es.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://um.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kg.nszjky.cn

================================================================================
来源：http://nf.hnjuh.cn

I. 正则表达式
来源：http://xc.bookmarksfly.cn

================================================================================
来源：http://ug.hahajie.cn

[I01] 判断是否匹配
来源：http://xp.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://af.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oo.szsharing.cn

JS:   /\d+/.test(s)
来源：http://rw.nicolike.cn

TS:   /\d+/.test(s)
来源：http://nr.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sa.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mk.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://gj.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ec.yuexingan06.cn

[I02] 提取所有匹配
来源：http://zd.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://uk.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://or.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://au.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://bm.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sw.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pa.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://uw.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gr.jctech888.com.cn

[I03] 提取捕获分组
来源：http://xb.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://me.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ik.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://up.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://js.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vp.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mj.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fl.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oc.muxihuayi.cn

[I04] 正则替换
来源：http://lc.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lh.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://my.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kt.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ml.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bw.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ny.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gu.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mk.hahajie.cn

[I05] 按正则拆分
来源：http://bl.nszjky.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rk.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dq.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://ra.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://nw.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://hr.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sm.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pr.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cn.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ks.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cl.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lh.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qe.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uz.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cb.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pe.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wg.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xs.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://hx.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nq.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dv.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://je.huixinmuqiang.cn

TS:   /error/gim
来源：http://ry.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zi.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nd.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://vl.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zs.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://na.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ga.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jc.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zy.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yj.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://id.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hw.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oe.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://du.shtwfgs.cn

================================================================================
来源：http://st.chemitech.net.cn

J. 日期与时间
来源：http://mw.colortex.cn

================================================================================
来源：http://mf.9csxet.cn

[J01] 获取当前时间
来源：http://sn.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bz.jctech888.com.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gb.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://lj.nicolike.cn

TS:   new Date();  Date.now()
来源：http://rj.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yn.yuexingan06.cn

Go:   time.Now()
来源：http://cd.jianghongdianzi.cn

Ruby: Time.now
来源：http://xs.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qc.hahajie.cn

[J02] 格式化输出
来源：http://ya.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lh.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://za.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oz.asd995.cn

TS:   d.toISOString()
来源：http://fq.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jk.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ku.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fg.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nt.gzmigu.cn

[J03] 字符串解析为日期
来源：http://xl.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jf.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wq.asd995.cn

JS:   new Date("2024-01-02")
来源：http://xa.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://zo.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gr.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uo.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://sl.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://me.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://ks.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rf.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uz.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ii.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fj.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sz.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vs.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jn.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zc.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://er.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://oj.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mh.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mz.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zu.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://tf.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qk.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://mg.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jh.haigaiapp.cn

[J06] 计算两时间之差
来源：http://zn.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://gy.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://fj.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kx.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ha.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ut.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://dt.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://qj.521024.cn

C#:   (end - start).TotalSeconds
来源：http://xh.newstarts.cn

[J07] 比较两个日期
来源：http://ox.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://tr.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://af.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sr.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ev.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sa.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://to.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tr.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://zx.asd995.cn

[J08] 提取年月日与星期
来源：http://yo.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://be.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mh.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ka.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ri.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zo.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dp.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rx.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vw.muxihuayi.cn

[J09] 时区处理
来源：http://pb.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mq.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vu.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mw.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jo.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nq.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ee.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gh.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://is.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://oc.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vg.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nt.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vp.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pz.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jd.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ae.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lw.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ik.hnjuh.cn

================================================================================
来源：http://dw.nszjky.cn

K. JSON 与序列化
来源：http://cs.huixinmuqiang.cn

================================================================================
来源：http://vc.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://rc.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ty.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ve.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://sx.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://ku.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://si.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://hh.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sy.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ud.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://wl.szsharing.cn

Py:   json.loads(s)
来源：http://cp.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lh.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://ue.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://el.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eq.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://fb.nszjky.cn

Ruby: JSON.parse(s)
来源：http://xq.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://er.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://in.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tr.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ls.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://es.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pu.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qj.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zr.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ot.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ps.nicolike.cn

[K04] 读取 JSON 文件
来源：http://kl.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jx.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yn.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dk.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xt.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nm.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bl.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fi.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cx.huanxung.cn

[K05] 深拷贝对象
来源：http://pb.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://pj.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://qi.nszjky.cn

JS:   structuredClone(obj)
来源：http://dv.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://gg.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pk.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://da.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bd.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vj.asd995.cn

[K06] 解析 URL 查询串
来源：http://tq.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gd.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://no.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bf.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aq.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bp.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kl.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tv.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ry.huixinmuqiang.cn

[K07] 进制转换
来源：http://vt.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qo.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uh.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lv.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ld.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ld.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bs.asd995.cn


<!-- 参考信息 -->