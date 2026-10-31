代发 wailian999

TS:   throw new Error("错误信息");
来源：http://ck.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gm.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ux.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jk.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://th.521024.cn

[H04] 自定义异常类型
来源：http://js.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://ww.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ki.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://sd.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://ni.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://ji.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hf.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://dx.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://of.huanxung.cn

[H05] 捕获特定类型
来源：http://qy.jctech888.com.cn

Py:   except ValueError as e:
来源：http://pt.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tf.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://tr.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://lo.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://hf.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hv.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://xw.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nf.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://rm.asd995.cn

Py:   value = d.get("k") or default
来源：http://dz.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ji.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bv.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jp.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zc.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xu.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://il.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://uz.chemitech.net.cn

[H07] 断言
来源：http://sj.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://ni.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://id.521024.cn

JS:   console.assert(x > 0);
来源：http://hj.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://zr.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://ws.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bq.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vb.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://fz.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://ak.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://hu.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kd.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://dw.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ad.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lc.wgjwhj.cn

Go:   err.Error()
来源：http://au.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://tb.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://we.jianghongdianzi.cn

[H09] 带错误码的异常
来源：http://vv.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wk.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://sb.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nf.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://af.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kc.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ss.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nm.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qc.shtwfgs.cn

[H10] 资源自动释放
来源：http://vj.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zl.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lx.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kn.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xz.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vj.asd995.cn

Go:   defer f.Close()
来源：http://as.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eo.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ek.shxzukj.cn

================================================================================
来源：http://uq.9csxet.cn

I. 正则表达式
来源：http://le.panjiajie.cn

================================================================================
来源：http://vd.shtwfgs.cn

[I01] 判断是否匹配
来源：http://rj.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ij.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yt.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://qv.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://at.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zz.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ta.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://ya.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ng.colortex.cn

[I02] 提取所有匹配
来源：http://jj.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://zr.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://re.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bi.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://mk.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vn.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lf.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://dy.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xb.wgjwhj.cn

[I03] 提取捕获分组
来源：http://zp.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ql.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ns.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wf.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uh.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sf.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ih.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://av.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hs.jianghongdianzi.cn

[I04] 正则替换
来源：http://wn.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uj.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bu.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bb.huanxung.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dg.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rz.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wz.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kn.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uo.shxzskj.cn

[I05] 按正则拆分
来源：http://nv.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bw.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qt.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ie.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://dd.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://ba.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rk.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xj.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qo.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ol.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gg.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cc.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fl.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://go.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jg.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yu.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gc.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yr.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://gx.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://na.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zp.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wc.huixiangedu.cn

TS:   /error/gim
来源：http://mi.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lg.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://on.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://bi.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iq.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://nm.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hn.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://af.shxzukj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uq.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xi.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zf.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ct.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xz.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ds.lnxyls.cn

================================================================================
来源：http://xs.colortex.cn

J. 日期与时间
来源：http://iz.szsharing.cn

================================================================================
来源：http://ro.panjiajie.cn

[J01] 获取当前时间
来源：http://jf.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://aq.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jw.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://yz.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://dk.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vi.gzmigu.cn

Go:   time.Now()
来源：http://qp.huixiangedu.cn

Ruby: Time.now
来源：http://qn.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yf.lnxyls.cn

[J02] 格式化输出
来源：http://mv.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ou.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qc.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aa.wgjwhj.cn

TS:   d.toISOString()
来源：http://vs.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xw.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xr.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kx.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://do.shxzukj.cn

[J03] 字符串解析为日期
来源：http://qy.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qn.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://be.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://dv.colortex.cn

TS:   new Date("2024-01-02")
来源：http://ep.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jf.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pv.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://lk.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jg.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://xd.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yh.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vr.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fi.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mr.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://in.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ub.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://do.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pi.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://ud.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://qm.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dh.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pu.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ft.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://xk.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://el.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://vb.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jj.colortex.cn

[J06] 计算两时间之差
来源：http://ec.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://bi.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://wt.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mu.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xy.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ya.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://jm.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://rv.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://jq.bookmarksfly.cn

[J07] 比较两个日期
来源：http://eu.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://nv.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xe.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tb.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ka.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://es.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fh.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://se.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://la.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://vo.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ke.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ni.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aa.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ps.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zl.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dc.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://go.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://he.colortex.cn

[J09] 时区处理
来源：http://rn.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vs.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ap.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mr.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mg.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sm.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mb.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://eo.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hc.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://db.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gw.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cv.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rn.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xq.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dy.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jp.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lz.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wd.huixiangedu.cn

================================================================================
来源：http://bl.521024.cn

K. JSON 与序列化
来源：http://uq.chemitech.net.cn

================================================================================
来源：http://qv.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://rp.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xu.huixiangedu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ff.521024.cn

JS:   JSON.stringify(obj)
来源：http://oq.asd995.cn

TS:   JSON.stringify(obj)
来源：http://yq.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pz.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://lk.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hj.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ic.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://ct.gzmigu.cn

Py:   json.loads(s)
来源：http://dv.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sg.asd995.cn

JS:   JSON.parse(s)
来源：http://gq.panjiajie.cn

TS:   JSON.parse(s)
来源：http://zd.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ie.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://ms.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://ux.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ac.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://lf.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pg.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yr.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hv.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gj.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fc.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mb.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lu.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dz.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://hv.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yg.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xq.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xj.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pq.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ka.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zu.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://aa.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ar.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://ly.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://qy.lnxyls.cn

PHP:  unserialize(serialize($obj));
来源：http://lc.nicolike.cn

JS:   structuredClone(obj)
来源：http://lb.hahajie.cn

TS:   structuredClone(obj)
来源：http://kf.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tl.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ob.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hh.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://up.huanxung.cn

[K06] 解析 URL 查询串
来源：http://ee.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rh.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hb.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cx.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fs.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yu.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gm.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ki.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://js.bjjhwx.cn

[K07] 进制转换
来源：http://qf.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yj.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vy.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ls.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rp.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sv.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://od.jctech888.com.cn


<!-- 参考信息 -->