代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lw.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ii.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nl.huanxung.cn

[H02] finally / ensure 收尾
来源：http://ld.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sn.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pn.shxzskj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sd.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://th.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kb.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ak.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kw.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cb.gzmigu.cn

[H03] 主动抛出异常
来源：http://hk.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://ww.huixinmuqiang.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rl.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://gw.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://jm.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://da.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vk.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wh.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qi.hahajie.cn

[H04] 自定义异常类型
来源：http://vc.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://sg.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cn.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://cd.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://cy.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://sw.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ur.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://en.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://ho.colortex.cn

[H05] 捕获特定类型
来源：http://ot.gzmigu.cn

Py:   except ValueError as e:
来源：http://bt.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dy.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://xj.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://kd.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://qb.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xi.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://oq.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kx.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://lt.szsharing.cn

Py:   value = d.get("k") or default
来源：http://nx.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ii.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xn.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ga.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fs.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ps.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://hr.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://vi.nicolike.cn

[H07] 断言
来源：http://dl.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://ia.newstarts.cn

PHP:  assert($x > 0);
来源：http://rg.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://fg.szsharing.cn

TS:   console.assert(x > 0);
来源：http://ir.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://pi.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://df.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://so.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://zi.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://xv.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://om.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://un.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://lt.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qo.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rb.huixiangedu.cn

Go:   err.Error()
来源：http://yc.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://ys.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://zr.nicolike.cn

[H09] 带错误码的异常
来源：http://zd.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wk.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://me.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vn.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qe.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vz.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tj.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ek.lnxyls.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rz.shtwfgs.cn

[H10] 资源自动释放
来源：http://yc.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fl.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ut.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vw.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zt.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qe.newstarts.cn

Go:   defer f.Close()
来源：http://zx.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lf.shxzukj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ns.shtwfgs.cn

================================================================================
来源：http://kv.shxzukj.cn

I. 正则表达式
来源：http://fc.jianghongdianzi.cn

================================================================================
来源：http://zg.huanxung.cn

[I01] 判断是否匹配
来源：http://vs.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ri.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uk.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://eg.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://ks.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nk.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qi.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://od.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qz.521024.cn

[I02] 提取所有匹配
来源：http://tk.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://mj.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zj.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sq.bjjhwx.cn

TS:   s.match(/\d+/g)
来源：http://dk.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oz.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://no.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://je.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zz.9csxet.cn

[I03] 提取捕获分组
来源：http://ir.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ch.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://po.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ax.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://am.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zi.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uy.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xc.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lk.huixinmuqiang.cn

[I04] 正则替换
来源：http://gr.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ki.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gw.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fb.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qy.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ib.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yh.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pb.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hr.colortex.cn

[I05] 按正则拆分
来源：http://qt.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ad.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eo.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://dc.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://tv.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://ru.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vu.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vi.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rw.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ak.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zr.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://au.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mz.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fb.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hn.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xf.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zk.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fr.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://ax.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://df.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ry.bjjhwx.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wb.9csxet.cn

TS:   /error/gim
来源：http://gw.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jn.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nt.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://vv.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zu.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://ks.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fs.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://we.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ol.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://em.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gz.muxihuayi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tc.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://op.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ko.jctech888.com.cn

================================================================================
来源：http://bw.panjiajie.cn

J. 日期与时间
来源：http://cr.shxzukj.cn

================================================================================
来源：http://sm.bookmarksfly.cn

[J01] 获取当前时间
来源：http://rs.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vi.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uw.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://wn.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://hm.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zr.wgjwhj.cn

Go:   time.Now()
来源：http://dn.wgjwhj.cn

Ruby: Time.now
来源：http://we.newstarts.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://no.jianghongdianzi.cn

[J02] 格式化输出
来源：http://fg.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cz.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gx.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nn.chemitech.net.cn

TS:   d.toISOString()
来源：http://ms.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uy.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xf.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nu.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rc.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://az.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xn.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gg.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://mq.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://zz.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hd.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yo.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://sa.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ms.newstarts.cn

[J04] 时间戳与日期互转
来源：http://sl.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rs.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fe.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xl.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hd.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fj.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xc.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wu.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tl.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://ak.wgjwhj.cn

Py:   now + timedelta(days=7)
来源：http://dg.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://aw.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ru.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fk.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://lo.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sr.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://eb.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gy.chemitech.net.cn

[J06] 计算两时间之差
来源：http://iy.asd995.cn

Py:   (end - start).total_seconds()
来源：http://nx.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://yl.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vo.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://na.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uk.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://ct.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://pf.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://vl.colortex.cn

[J07] 比较两个日期
来源：http://ll.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://jn.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lt.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lk.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://to.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zb.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dx.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://na.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://rh.colortex.cn

[J08] 提取年月日与星期
来源：http://jn.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tg.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aq.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sf.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oj.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ap.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hg.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mg.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rg.chemitech.net.cn

[J09] 时区处理
来源：http://ae.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hg.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ju.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ol.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kv.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gf.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ns.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cr.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nb.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://mm.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hf.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wy.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iw.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mn.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://in.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gr.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tw.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qe.szsharing.cn

================================================================================
来源：http://we.bjjhwx.cn

K. JSON 与序列化
来源：http://pq.shxzukj.cn

================================================================================
来源：http://mo.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://ft.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ba.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pp.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://hv.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://lf.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qo.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://vj.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ec.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pw.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://lx.shxzskj.cn

Py:   json.loads(s)
来源：http://bg.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ib.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://gz.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://sz.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sh.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://vo.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://id.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ot.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://sf.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tz.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tq.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xy.szxytkj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jp.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ky.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://as.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xm.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mm.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://ci.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ds.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jr.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ey.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tj.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hx.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fg.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://un.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zx.haigaiapp.cn

[K05] 深拷贝对象
来源：http://zp.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://xa.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://de.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://jm.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://bv.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nx.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sh.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vw.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mp.hahajie.cn


<!-- 参考信息 -->