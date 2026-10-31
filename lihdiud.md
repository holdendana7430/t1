代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://om.521024.cn

[H04] 自定义异常类型
来源：http://gj.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://rk.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://aa.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://lp.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://es.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://xq.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tf.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://da.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://ak.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://zg.gzmigu.cn

Py:   except ValueError as e:
来源：http://pb.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://no.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://oj.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://cd.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://xl.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uy.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://es.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://im.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://ir.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://td.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tt.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uu.hahajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rj.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mk.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ga.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://xw.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://wm.colortex.cn

[H07] 断言
来源：http://rl.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://on.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://cp.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://wx.9csxet.cn

TS:   console.assert(x > 0);
来源：http://zq.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://qe.yuntaijiaju.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jk.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ye.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://vo.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://da.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://el.gzmigu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ck.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://pa.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ly.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lu.shxzukj.cn

Go:   err.Error()
来源：http://zl.hahajie.cn

Ruby: e.message;  e.backtrace
来源：http://rr.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://bb.panjiajie.cn

[H09] 带错误码的异常
来源：http://pa.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://us.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://no.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vw.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sx.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://az.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mp.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://np.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wd.huanxung.cn

[H10] 资源自动释放
来源：http://bo.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://de.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qi.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ne.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pt.gzmigu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zr.colortex.cn

Go:   defer f.Close()
来源：http://eo.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ir.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kc.chemitech.net.cn

================================================================================
来源：http://xn.newstarts.cn

I. 正则表达式
来源：http://oj.gzmigu.cn

================================================================================
来源：http://fk.nicolike.cn

[I01] 判断是否匹配
来源：http://ik.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mi.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lb.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://lg.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://mx.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ax.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ot.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://th.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://in.521024.cn

[I02] 提取所有匹配
来源：http://zu.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://hi.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sz.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zi.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://qt.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vv.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qm.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://ro.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hg.panjiajie.cn

[I03] 提取捕获分组
来源：http://yb.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rk.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fq.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ws.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oy.yuexingan06.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kk.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vy.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gs.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xp.shxzskj.cn

[I04] 正则替换
来源：http://td.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://as.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xr.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qs.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ez.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cx.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oq.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vg.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://in.9csxet.cn

[I05] 按正则拆分
来源：http://lc.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dn.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vg.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://ru.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://qn.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://ds.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://is.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zr.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://al.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rs.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tj.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qk.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pl.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xz.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://am.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xy.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ui.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oa.szxytkj.cn

[I07] 忽略大小写与多行模式
来源：http://ef.bjjhwx.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jn.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sh.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qk.bjjhwx.cn

TS:   /error/gim
来源：http://tz.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://we.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kl.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://of.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eg.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://jw.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bf.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://of.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mr.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ek.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ti.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nl.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lp.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pw.9csxet.cn

================================================================================
来源：http://qc.bjjhwx.cn

J. 日期与时间
来源：http://gr.panjiajie.cn

================================================================================
来源：http://aw.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://jp.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yw.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zr.lnxyls.cn

JS:   new Date();  Date.now()
来源：http://en.asd995.cn

TS:   new Date();  Date.now()
来源：http://be.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uc.nszjky.cn

Go:   time.Now()
来源：http://hj.huanxung.cn

Ruby: Time.now
来源：http://cn.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nr.bjjhwx.cn

[J02] 格式化输出
来源：http://lw.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mr.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qs.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://do.haigaiapp.cn

TS:   d.toISOString()
来源：http://vq.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://by.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hp.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yh.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tu.nszjky.cn

[J03] 字符串解析为日期
来源：http://xq.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lg.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eu.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://hh.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://of.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fd.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pe.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://uu.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rt.asd995.cn

[J04] 时间戳与日期互转
来源：http://wi.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ud.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yf.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nq.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lx.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ba.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ne.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://of.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fc.521024.cn

[J05] 时间加减（加 7 天）
来源：http://qo.colortex.cn

Py:   now + timedelta(days=7)
来源：http://ch.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://la.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yj.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qx.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://ts.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mm.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://en.szsharing.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yj.shtwfgs.cn

[J06] 计算两时间之差
来源：http://th.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://du.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://xr.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://na.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rt.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tx.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://gy.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://re.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://lm.newstarts.cn

[J07] 比较两个日期
来源：http://pz.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://su.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ne.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ix.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mf.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zh.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://or.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yw.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ym.asd995.cn

[J08] 提取年月日与星期
来源：http://jn.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wd.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lv.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cs.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://te.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://br.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://og.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qq.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fr.colortex.cn

[J09] 时区处理
来源：http://bl.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://io.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ej.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://re.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xx.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xm.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pe.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hs.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xq.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://me.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ir.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jb.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xt.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mg.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ld.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cd.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://de.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://im.chemitech.net.cn

================================================================================
来源：http://my.newstarts.cn

K. JSON 与序列化
来源：http://nf.521024.cn

================================================================================
来源：http://bg.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://pq.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wm.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ui.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://ed.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://cp.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dc.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://gm.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vl.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ek.nicolike.cn

[K02] JSON 字符串转对象
来源：http://ud.yuexingan06.cn

Py:   json.loads(s)
来源：http://ie.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vi.9csxet.cn

JS:   JSON.parse(s)
来源：http://vm.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://kn.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vw.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://gv.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://dn.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pq.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://hf.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ji.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fq.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fw.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vc.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cx.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ld.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://je.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bv.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://ix.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nb.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vn.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ng.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://is.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dq.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ps.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rr.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aw.panjiajie.cn

[K05] 深拷贝对象
来源：http://vi.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://sh.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://je.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://tq.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://eh.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ki.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xz.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fy.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kk.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://lt.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cy.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ns.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dc.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zl.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kp.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ny.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mq.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bv.huanxung.cn

[K07] 进制转换
来源：http://iw.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wo.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zw.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vs.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bl.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mu.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lm.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yx.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vx.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://gi.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://gz.gzmigu.cn


<!-- 参考信息 -->