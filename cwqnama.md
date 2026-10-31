代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yw.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ep.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qn.newstarts.cn

[H02] finally / ensure 收尾
来源：http://gy.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xy.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fc.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jt.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ft.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ba.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zu.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zs.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mx.panjiajie.cn

[H03] 主动抛出异常
来源：http://pl.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://hn.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xo.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://dg.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://uv.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zc.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ic.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ys.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sp.hnjuh.cn

[H04] 自定义异常类型
来源：http://rc.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://dz.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rd.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://rq.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://ig.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://ue.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oe.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://ay.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://hn.shxzskj.cn

[H05] 捕获特定类型
来源：http://tx.521024.cn

Py:   except ValueError as e:
来源：http://bb.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gd.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://xe.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://eb.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://yc.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pv.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://pd.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ue.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://id.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://kd.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qp.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oa.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://so.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ku.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://le.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://tv.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://og.chemitech.net.cn

[H07] 断言
来源：http://nf.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://qt.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://sx.szsharing.cn

JS:   console.assert(x > 0);
来源：http://ev.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://zg.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://an.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ha.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ao.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://yk.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://uq.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://ba.nszjky.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xy.szsharing.cn

JS:   e.message;  e.stack
来源：http://it.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ke.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nl.shtwfgs.cn

Go:   err.Error()
来源：http://ng.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://bb.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://hf.wgjwhj.cn

[H09] 带错误码的异常
来源：http://cq.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vp.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dg.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kg.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://at.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iv.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uo.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ku.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ib.521024.cn

[H10] 资源自动释放
来源：http://wh.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xm.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kl.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://on.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fc.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cz.shxzskj.cn

Go:   defer f.Close()
来源：http://jc.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lm.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kd.bjjhwx.cn

================================================================================
来源：http://tf.hahajie.cn

I. 正则表达式
来源：http://vm.jianghongdianzi.cn

================================================================================
来源：http://ss.hahajie.cn

[I01] 判断是否匹配
来源：http://br.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fm.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xu.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://yw.huanxung.cn

TS:   /\d+/.test(s)
来源：http://so.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://is.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zv.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://vl.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jk.wgjwhj.cn

[I02] 提取所有匹配
来源：http://io.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://eh.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mg.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mc.asd995.cn

TS:   s.match(/\d+/g)
来源：http://ak.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://na.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bv.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://xx.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hv.hahajie.cn

[I03] 提取捕获分组
来源：http://qh.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lp.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mj.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qc.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ur.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ia.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pm.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rf.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lx.shxzskj.cn

[I04] 正则替换
来源：http://ui.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cw.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gc.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rd.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vt.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dp.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ul.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qk.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vo.bookmarksfly.cn

[I05] 按正则拆分
来源：http://ce.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hv.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vk.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://ln.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://fm.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://qu.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://it.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zf.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zc.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://od.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qa.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ew.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qj.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vq.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uz.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pd.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qb.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qf.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://za.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ws.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lx.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kh.szxytkj.cn

TS:   /error/gim
来源：http://ur.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bt.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sj.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://gc.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bh.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://mt.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fv.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xh.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sa.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dw.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oz.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ux.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nk.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kl.bookmarksfly.cn

================================================================================
来源：http://vm.yuexingan06.cn

J. 日期与时间
来源：http://wi.yuexingan06.cn

================================================================================
来源：http://ey.gzmigu.cn

[J01] 获取当前时间
来源：http://ua.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ko.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qs.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://vw.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://pp.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mj.shxzukj.cn

Go:   time.Now()
来源：http://uh.nicolike.cn

Ruby: Time.now
来源：http://qk.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vn.huixiangedu.cn

[J02] 格式化输出
来源：http://fv.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vy.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://po.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qm.lnxyls.cn

TS:   d.toISOString()
来源：http://nk.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lq.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tf.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kp.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yu.shxzskj.cn

[J03] 字符串解析为日期
来源：http://zd.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://to.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ot.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://kj.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://gy.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rs.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qh.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://on.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cg.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://ks.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xz.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mo.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ny.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gz.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nd.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yq.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rq.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ya.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://nf.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://bc.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lc.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cv.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fn.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://zi.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://od.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://ds.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yg.bjjhwx.cn

[J06] 计算两时间之差
来源：http://rl.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://ny.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://ic.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dg.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ee.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://js.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://xm.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://cj.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://ym.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://um.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://bc.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gj.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lr.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ih.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oy.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jp.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xf.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://vj.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://qc.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://om.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rc.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jy.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yc.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sh.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wy.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kr.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://je.bookmarksfly.cn

[J09] 时区处理
来源：http://kh.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wy.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fp.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gb.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zh.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ux.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fp.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://st.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ro.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://fg.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wk.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yd.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kp.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ee.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gi.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cv.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tc.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ir.gzmigu.cn

================================================================================
来源：http://xn.nszjky.cn

K. JSON 与序列化
来源：http://bv.asd995.cn

================================================================================
来源：http://jb.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://rm.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ln.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ua.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://rv.asd995.cn

TS:   JSON.stringify(obj)
来源：http://ir.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yh.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://xm.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nz.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cn.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://bv.chemitech.net.cn

Py:   json.loads(s)
来源：http://fg.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://he.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://li.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://ol.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xh.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://ut.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://iy.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yg.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://vy.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jr.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hj.jianghongdianzi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ma.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tp.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sg.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wb.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cu.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ng.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://ne.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sp.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ai.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uw.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zm.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gq.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ij.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xr.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gl.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://kb.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://jk.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://bx.hahajie.cn

JS:   structuredClone(obj)
来源：http://vs.colortex.cn

TS:   structuredClone(obj)
来源：http://mb.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qr.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tb.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nj.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kj.bookmarksfly.cn


<!-- 参考信息 -->