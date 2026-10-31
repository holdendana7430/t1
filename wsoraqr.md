代发 wailian999

[H03] 主动抛出异常
来源：http://yr.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://rx.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yk.haigaiapp.cn

JS:   throw new Error("错误信息");
来源：http://ou.colortex.cn

TS:   throw new Error("错误信息");
来源：http://up.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://iz.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ma.yuexingan06.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gb.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ns.szsharing.cn

[H04] 自定义异常类型
来源：http://jc.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://uk.521024.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yu.wgjwhj.cn

JS:   class MyError extends Error {}
来源：http://zq.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://ip.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://ge.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://de.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://zw.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://bt.nszjky.cn

[H05] 捕获特定类型
来源：http://ay.nszjky.cn

Py:   except ValueError as e:
来源：http://xp.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ed.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://sc.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://vh.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://nr.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zq.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://ue.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://je.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://ad.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://qh.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gj.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wj.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zs.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oc.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://in.huanxung.cn

Ruby: d&.dig(:a, :b)
来源：http://wy.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://od.bookmarksfly.cn

[H07] 断言
来源：http://tw.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://yk.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://yh.newstarts.cn

JS:   console.assert(x > 0);
来源：http://lh.asd995.cn

TS:   console.assert(x > 0);
来源：http://fj.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://qv.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://at.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://iy.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://yt.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://yx.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://qb.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pv.hnjuh.cn

JS:   e.message;  e.stack
来源：http://gm.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://za.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ae.chemitech.net.cn

Go:   err.Error()
来源：http://tr.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://ws.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://su.szsharing.cn

[H09] 带错误码的异常
来源：http://en.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mi.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vz.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bt.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gg.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tf.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hi.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://om.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lu.bookmarksfly.cn

[H10] 资源自动释放
来源：http://if.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vk.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jz.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nh.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cx.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mq.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://rm.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oi.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vr.bookmarksfly.cn

================================================================================
来源：http://jl.521024.cn

I. 正则表达式
来源：http://tt.shxzukj.cn

================================================================================
来源：http://xe.wgjwhj.cn

[I01] 判断是否匹配
来源：http://gb.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hx.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nv.newstarts.cn

JS:   /\d+/.test(s)
来源：http://dy.521024.cn

TS:   /\d+/.test(s)
来源：http://sd.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gk.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yx.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://ga.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ni.jctech888.com.cn

[I02] 提取所有匹配
来源：http://xr.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://lk.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wf.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xb.jianghongdianzi.cn

TS:   s.match(/\d+/g)
来源：http://pa.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tr.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kq.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://hl.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qa.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://hy.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://js.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jf.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fq.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xr.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fl.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://it.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qc.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mu.haigaiapp.cn

[I04] 正则替换
来源：http://if.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ws.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nx.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ki.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sv.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ue.yuntaijiaju.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ie.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rs.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cj.huixiangedu.cn

[I05] 按正则拆分
来源：http://yc.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gs.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sq.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://nj.chemitech.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://jy.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://gb.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xn.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zw.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ms.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mp.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ej.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dx.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cs.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zn.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uu.yuntaijiaju.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uw.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vc.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bu.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://fo.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wc.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tt.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hf.haigaiapp.cn

TS:   /error/gim
来源：http://hs.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mr.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lg.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://sh.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yq.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://gd.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dl.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nj.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wl.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zw.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://br.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gx.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://et.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rj.bookmarksfly.cn

================================================================================
来源：http://af.hahajie.cn

J. 日期与时间
来源：http://bq.521024.cn

================================================================================
来源：http://ay.bookmarksfly.cn

[J01] 获取当前时间
来源：http://jt.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sr.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jz.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://ws.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://vd.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jc.jianghongdianzi.cn

Go:   time.Now()
来源：http://tp.huixinmuqiang.cn

Ruby: Time.now
来源：http://bt.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yl.jianghongdianzi.cn

[J02] 格式化输出
来源：http://md.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://td.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rv.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xp.hnjuh.cn

TS:   d.toISOString()
来源：http://ha.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ib.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sb.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lq.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ek.lnxyls.cn

[J03] 字符串解析为日期
来源：http://ws.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rm.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bs.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://rr.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://kd.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://aj.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cz.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://ty.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lz.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://de.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://na.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jl.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zs.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://am.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vc.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nq.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rn.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sm.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://pi.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://wv.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kc.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vf.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zj.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://uv.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mj.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://tq.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ep.bjjhwx.cn

[J06] 计算两时间之差
来源：http://qk.asd995.cn

Py:   (end - start).total_seconds()
来源：http://js.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://xf.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zd.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://do.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nd.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://mv.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://tk.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://va.asd995.cn

[J07] 比较两个日期
来源：http://hg.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://xp.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bi.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zu.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bf.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hf.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://es.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ei.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://jo.huanxung.cn

[J08] 提取年月日与星期
来源：http://me.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wg.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kh.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ik.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ql.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hw.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rj.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nl.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ko.asd995.cn

[J09] 时区处理
来源：http://ue.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://al.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cp.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://va.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mw.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kt.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://md.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cb.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dq.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://rf.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://is.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bl.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zi.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iz.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tn.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xd.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ts.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fj.newstarts.cn

================================================================================
来源：http://am.jctech888.com.cn

K. JSON 与序列化
来源：http://fp.muxihuayi.cn

================================================================================
来源：http://jz.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://ws.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nd.gzmigu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hy.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://lb.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://cy.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ui.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://pt.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zr.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iq.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://ht.yuexingan06.cn

Py:   json.loads(s)
来源：http://bh.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eg.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://et.nicolike.cn

TS:   JSON.parse(s)
来源：http://qe.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://da.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://lx.asd995.cn

Ruby: JSON.parse(s)
来源：http://yk.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hm.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://kj.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nv.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hx.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hh.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xf.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fp.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sm.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bx.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kz.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://ti.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iy.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ps.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mi.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ee.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pc.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fz.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ui.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ww.shxzskj.cn

[K05] 深拷贝对象
来源：http://hj.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://zj.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://sa.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://bm.asd995.cn

TS:   structuredClone(obj)
来源：http://xb.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mu.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://un.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ym.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gn.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://hn.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fa.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ez.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tu.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ig.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ea.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dd.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hv.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ur.gzmigu.cn

[K07] 进制转换
来源：http://xi.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kv.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aj.hnjuh.cn


<!-- 参考信息 -->