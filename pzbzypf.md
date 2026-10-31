代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bj.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xf.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://me.huanxung.cn

[H02] finally / ensure 收尾
来源：http://zk.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qc.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bw.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jx.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lq.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xj.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ev.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hv.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pv.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://nt.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://om.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tw.newstarts.cn

JS:   throw new Error("错误信息");
来源：http://gu.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://kg.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yr.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ar.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gl.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hs.colortex.cn

[H04] 自定义异常类型
来源：http://av.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://vo.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mg.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://gc.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://nm.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://nn.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://um.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://ve.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://kq.521024.cn

[H05] 捕获特定类型
来源：http://ca.9csxet.cn

Py:   except ValueError as e:
来源：http://lu.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ix.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://ux.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://gd.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://gh.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qw.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://bv.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qa.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://au.jianghongdianzi.cn

Py:   value = d.get("k") or default
来源：http://qv.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://eo.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rn.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hn.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kn.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uw.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://ni.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://iq.colortex.cn

[H07] 断言
来源：http://jm.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://rl.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://fs.hahajie.cn

JS:   console.assert(x > 0);
来源：http://nr.9csxet.cn

TS:   console.assert(x > 0);
来源：http://my.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://gh.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ld.hahajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yb.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://mf.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://zf.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://fd.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nq.shxzukj.cn

JS:   e.message;  e.stack
来源：http://ju.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mu.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zg.gzmigu.cn

Go:   err.Error()
来源：http://qk.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://up.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://kk.shtwfgs.cn

[H09] 带错误码的异常
来源：http://hi.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kc.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ne.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ug.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://st.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tu.asd995.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://el.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://si.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nk.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://ii.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hq.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jp.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://he.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nv.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aw.muxihuayi.cn

Go:   defer f.Close()
来源：http://sm.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mb.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ww.nszjky.cn

================================================================================
来源：http://uz.bookmarksfly.cn

I. 正则表达式
来源：http://bf.bookmarksfly.cn

================================================================================
来源：http://is.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://ag.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dy.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hw.9csxet.cn

JS:   /\d+/.test(s)
来源：http://td.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://gs.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kr.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ba.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://am.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://as.haigaiapp.cn

[I02] 提取所有匹配
来源：http://uh.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://cw.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cb.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dc.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://el.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ih.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uz.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://jv.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://do.nszjky.cn

[I03] 提取捕获分组
来源：http://zb.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kn.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lk.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ed.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eo.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gb.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nq.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rt.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jz.newstarts.cn

[I04] 正则替换
来源：http://up.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yj.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zk.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mw.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yb.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jg.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nz.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jv.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zx.bjjhwx.cn

[I05] 按正则拆分
来源：http://dj.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ma.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://km.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://ud.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://hd.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://dq.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wa.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ap.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kb.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hh.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pg.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bd.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qf.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sk.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://el.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pj.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aa.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dp.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://vk.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qx.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vc.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ct.szsharing.cn

TS:   /error/gim
来源：http://la.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hx.colortex.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nb.colortex.cn

Ruby: s.scan(/error/i)
来源：http://vs.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sg.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://nv.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://av.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pc.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xo.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oh.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ov.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ls.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vf.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ld.jianghongdianzi.cn

================================================================================
来源：http://yc.panjiajie.cn

J. 日期与时间
来源：http://ut.panjiajie.cn

================================================================================
来源：http://yc.nicolike.cn

[J01] 获取当前时间
来源：http://yc.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hk.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fg.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://qe.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://dl.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ri.9csxet.cn

Go:   time.Now()
来源：http://vl.szsharing.cn

Ruby: Time.now
来源：http://xt.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hl.muxihuayi.cn

[J02] 格式化输出
来源：http://ej.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gg.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bc.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://td.muxihuayi.cn

TS:   d.toISOString()
来源：http://pq.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://th.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ix.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vf.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cj.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://pt.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nk.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://in.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://zo.asd995.cn

TS:   new Date("2024-01-02")
来源：http://nm.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jp.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vu.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://am.521024.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qt.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://rf.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jv.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ok.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xc.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wp.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qu.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mv.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ua.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qy.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://la.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://rh.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nl.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ku.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bg.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://bf.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cm.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://qb.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://je.szsharing.cn

[J06] 计算两时间之差
来源：http://va.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://tk.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://cl.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://my.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nx.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vy.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://jj.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://vm.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://xp.bjjhwx.cn

[J07] 比较两个日期
来源：http://em.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://gu.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wt.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tx.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dp.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ps.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lg.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pp.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://bx.nszjky.cn

[J08] 提取年月日与星期
来源：http://py.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xh.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kv.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pl.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://at.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kd.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xx.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vj.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kf.panjiajie.cn

[J09] 时区处理
来源：http://ys.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://je.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gz.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vk.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wj.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ut.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cs.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ds.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ph.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://vb.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ti.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yf.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fl.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qd.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qr.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pr.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hj.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fr.shxzukj.cn

================================================================================
来源：http://fp.huanxung.cn

K. JSON 与序列化
来源：http://ne.jianghongdianzi.cn

================================================================================
来源：http://xl.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://lx.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xa.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hc.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://vj.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://dy.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ku.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://xa.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sk.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://me.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://bb.521024.cn

Py:   json.loads(s)
来源：http://xn.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mg.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://gi.shxzukj.cn

TS:   JSON.parse(s)
来源：http://pl.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gp.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://yz.szsharing.cn

Ruby: JSON.parse(s)
来源：http://wz.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ld.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://pj.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yc.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://id.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qe.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mv.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ns.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hi.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://re.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ry.9csxet.cn

[K04] 读取 JSON 文件
来源：http://sq.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ay.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uo.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kc.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hw.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wv.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qm.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ss.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tg.9csxet.cn

[K05] 深拷贝对象
来源：http://gq.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://mq.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://xj.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://el.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://ri.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ss.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ty.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tl.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yz.huixiangedu.cn


<!-- 参考信息 -->