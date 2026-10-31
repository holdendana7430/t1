代发 wailian999

[H03] 主动抛出异常
来源：http://tz.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://uq.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cg.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://nk.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://yy.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://za.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uh.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zo.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://do.colortex.cn

[H04] 自定义异常类型
来源：http://mx.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://yf.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cd.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://go.521024.cn

TS:   class MyError extends Error {}
来源：http://dk.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://bo.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hh.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://ch.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://ox.jctech888.com.cn

[H05] 捕获特定类型
来源：http://up.newstarts.cn

Py:   except ValueError as e:
来源：http://et.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pz.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://cm.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ko.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://ge.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uw.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://zu.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qp.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://tf.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://mo.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wz.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cd.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uv.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mz.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pg.hahajie.cn

Ruby: d&.dig(:a, :b)
来源：http://dm.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://tq.521024.cn

[H07] 断言
来源：http://er.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://jz.nszjky.cn

PHP:  assert($x > 0);
来源：http://mt.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://sv.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://lq.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://ks.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://et.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rd.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://xt.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://ny.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://bp.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xw.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://hj.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rm.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qt.shtwfgs.cn

Go:   err.Error()
来源：http://ia.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://di.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://pn.szxytkj.cn

[H09] 带错误码的异常
来源：http://je.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cm.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://eh.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://be.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bs.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fq.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jp.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hk.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://td.huixinmuqiang.cn

[H10] 资源自动释放
来源：http://hv.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ii.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wd.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nb.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kr.muxihuayi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qt.gzmigu.cn

Go:   defer f.Close()
来源：http://kp.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lo.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bq.huanxung.cn

================================================================================
来源：http://jx.haigaiapp.cn

I. 正则表达式
来源：http://lw.gzmigu.cn

================================================================================
来源：http://rf.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://rn.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kp.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xh.szsharing.cn

JS:   /\d+/.test(s)
来源：http://xe.newstarts.cn

TS:   /\d+/.test(s)
来源：http://gh.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lh.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qr.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://yd.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ts.newstarts.cn

[I02] 提取所有匹配
来源：http://st.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://jq.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sf.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://go.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://rc.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ae.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lp.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://ja.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://es.szxytkj.cn

[I03] 提取捕获分组
来源：http://yu.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aq.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yv.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lq.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://on.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zq.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vx.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rg.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xs.shxzukj.cn

[I04] 正则替换
来源：http://ob.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ng.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://on.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wi.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ia.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://co.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yw.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hq.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sr.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://ni.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rf.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fd.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://zg.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://rb.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://ki.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kc.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jd.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dx.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qk.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nr.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hm.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yd.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xt.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uh.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sl.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oe.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://im.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://zs.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xe.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dw.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vp.colortex.cn

TS:   /error/gim
来源：http://tt.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://je.colortex.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fg.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://ez.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jx.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://xd.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rj.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ux.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jj.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xm.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dq.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rc.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zd.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://np.asd995.cn

================================================================================
来源：http://ol.jianghongdianzi.cn

J. 日期与时间
来源：http://cf.huanxung.cn

================================================================================
来源：http://we.panjiajie.cn

[J01] 获取当前时间
来源：http://kk.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qc.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ha.9csxet.cn

JS:   new Date();  Date.now()
来源：http://ne.9csxet.cn

TS:   new Date();  Date.now()
来源：http://dw.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pe.jctech888.com.cn

Go:   time.Now()
来源：http://sh.shxzskj.cn

Ruby: Time.now
来源：http://gk.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kv.chemitech.net.cn

[J02] 格式化输出
来源：http://wb.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pg.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ul.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jm.huanxung.cn

TS:   d.toISOString()
来源：http://vc.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kh.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sb.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sh.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oq.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://sr.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://br.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vq.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://pd.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://oi.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kq.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ih.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://nj.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bg.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://wq.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pe.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lq.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gy.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://si.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://du.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uq.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uw.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ez.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://er.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://qm.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pb.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cg.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qx.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://my.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lo.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://rl.szsharing.cn

C#:   DateTime.Now.AddDays(7)
来源：http://om.gzmigu.cn

[J06] 计算两时间之差
来源：http://fb.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://qg.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://vy.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yx.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mz.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nc.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://gj.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://re.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://do.9csxet.cn

[J07] 比较两个日期
来源：http://da.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://yf.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mf.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hv.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sx.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yp.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gd.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yt.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://zw.hahajie.cn

[J08] 提取年月日与星期
来源：http://oi.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cs.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lu.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://do.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jf.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wc.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hd.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qv.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oh.newstarts.cn

[J09] 时区处理
来源：http://sd.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://od.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://to.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ze.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xk.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qf.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tn.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://im.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sa.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://gv.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zn.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yv.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xc.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rn.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wf.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://he.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qg.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dq.shtwfgs.cn

================================================================================
来源：http://dd.nicolike.cn

K. JSON 与序列化
来源：http://nm.chemitech.net.cn

================================================================================
来源：http://hp.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://jf.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bl.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kt.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://vr.colortex.cn

TS:   JSON.stringify(obj)
来源：http://uo.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gi.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://jd.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gj.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xn.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://nt.colortex.cn

Py:   json.loads(s)
来源：http://dt.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pf.521024.cn

JS:   JSON.parse(s)
来源：http://rf.szxytkj.cn

TS:   JSON.parse(s)
来源：http://gh.gzmigu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pv.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://dw.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://cd.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mh.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://as.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sx.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dq.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hh.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://np.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vx.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ht.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ly.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gw.9csxet.cn

[K04] 读取 JSON 文件
来源：http://qf.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bb.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://te.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wh.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ug.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://df.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://by.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mw.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zd.jctech888.com.cn

[K05] 深拷贝对象
来源：http://zy.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://ob.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://jp.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://on.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://ki.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lq.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uq.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xa.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mg.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://qj.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bn.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jj.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://br.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sy.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iv.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ya.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qb.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mj.asd995.cn

[K07] 进制转换
来源：http://xo.panjiajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lp.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sj.bjjhwx.cn


<!-- 参考信息 -->