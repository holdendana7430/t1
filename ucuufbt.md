代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uc.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wj.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rm.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://at.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eg.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ho.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fo.hahajie.cn

[H02] finally / ensure 收尾
来源：http://aj.colortex.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ze.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sh.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jf.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://po.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ap.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xe.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://th.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gi.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://fg.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://dq.hahajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tp.521024.cn

JS:   throw new Error("错误信息");
来源：http://dm.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://ae.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://js.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nh.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mv.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://om.yuexingan06.cn

[H04] 自定义异常类型
来源：http://rx.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://hb.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qq.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://aq.newstarts.cn

TS:   class MyError extends Error {}
来源：http://mp.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://si.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cp.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://dc.asd995.cn

C#:   class MyException : Exception {}
来源：http://zv.yuexingan06.cn

[H05] 捕获特定类型
来源：http://li.haigaiapp.cn

Py:   except ValueError as e:
来源：http://ld.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eu.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://hw.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://iy.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://jo.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ty.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://ex.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pt.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://sv.9csxet.cn

Py:   value = d.get("k") or default
来源：http://sk.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://in.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fs.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yf.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wl.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jb.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://lg.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://la.jianghongdianzi.cn

[H07] 断言
来源：http://ka.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://jv.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://rg.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://oz.huanxung.cn

TS:   console.assert(x > 0);
来源：http://rq.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://vs.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://js.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rv.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://mt.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://is.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://ul.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oy.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://vg.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ck.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gz.muxihuayi.cn

Go:   err.Error()
来源：http://wj.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://kk.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://tj.wgjwhj.cn

[H09] 带错误码的异常
来源：http://ub.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yz.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ae.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ys.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hd.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kg.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oy.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nb.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hl.nszjky.cn

[H10] 资源自动释放
来源：http://ph.bjjhwx.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kv.shxzskj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tr.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gu.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ty.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ub.szxytkj.cn

Go:   defer f.Close()
来源：http://qg.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ev.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zz.jctech888.com.cn

================================================================================
来源：http://ce.521024.cn

I. 正则表达式
来源：http://qi.colortex.cn

================================================================================
来源：http://dj.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://ad.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yq.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://du.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://pn.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://ky.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ks.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vf.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://lb.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://at.521024.cn

[I02] 提取所有匹配
来源：http://ht.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://eq.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ig.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bo.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://fq.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eq.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ak.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://kc.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ub.jctech888.com.cn

[I03] 提取捕获分组
来源：http://nz.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ea.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rp.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lw.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://te.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dk.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qt.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bj.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ty.chemitech.net.cn

[I04] 正则替换
来源：http://kp.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mm.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zi.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ad.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zj.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yf.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pf.chemitech.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://po.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hk.gzmigu.cn

[I05] 按正则拆分
来源：http://fd.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tq.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ql.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://lc.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://jb.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://it.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hu.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://us.muxihuayi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qx.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dz.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yh.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bg.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tf.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sn.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ou.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tm.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vq.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tl.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://us.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wh.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lf.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sk.bookmarksfly.cn

TS:   /error/gim
来源：http://oh.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ap.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qm.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://fn.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gf.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://gg.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jt.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ju.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gx.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xo.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sk.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iw.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xr.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eg.bjjhwx.cn

================================================================================
来源：http://bd.colortex.cn

J. 日期与时间
来源：http://sx.lnxyls.cn

================================================================================
来源：http://bn.newstarts.cn

[J01] 获取当前时间
来源：http://tr.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hk.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eg.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://vg.szsharing.cn

TS:   new Date();  Date.now()
来源：http://fh.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jv.newstarts.cn

Go:   time.Now()
来源：http://hi.huanxung.cn

Ruby: Time.now
来源：http://xo.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hy.jctech888.com.cn

[J02] 格式化输出
来源：http://ho.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ga.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bc.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sf.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://jb.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lq.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ft.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dp.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dd.nicolike.cn

[J03] 字符串解析为日期
来源：http://yh.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jn.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://me.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://xc.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://gm.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cv.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tf.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://ty.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iw.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://fr.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://it.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dw.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ge.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dm.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ow.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ea.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ib.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fo.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://hc.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://ft.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ca.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vh.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pp.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://co.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ap.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://vl.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vn.wgjwhj.cn

[J06] 计算两时间之差
来源：http://qj.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://rx.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://tg.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bi.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ms.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dv.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://qb.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://xz.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://rz.nszjky.cn

[J07] 比较两个日期
来源：http://mg.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://sd.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zo.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nz.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nw.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vj.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iz.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bg.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://bo.9csxet.cn

[J08] 提取年月日与星期
来源：http://rp.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tt.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cm.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ri.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vh.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yu.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jw.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ve.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xz.bjjhwx.cn

[J09] 时区处理
来源：http://nb.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jp.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zz.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gz.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://do.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nt.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zf.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yh.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mk.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://uo.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sj.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bg.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yu.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cc.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ne.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lo.shxzukj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zl.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yc.chemitech.net.cn

================================================================================
来源：http://if.huixinmuqiang.cn

K. JSON 与序列化
来源：http://ih.hnjuh.cn

================================================================================
来源：http://fq.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://ei.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ok.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cc.asd995.cn

JS:   JSON.stringify(obj)
来源：http://sz.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://ro.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rc.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://yi.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xz.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gr.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://gr.panjiajie.cn

Py:   json.loads(s)
来源：http://vg.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yb.szsharing.cn

JS:   JSON.parse(s)
来源：http://ef.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://mk.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lg.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://hd.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://dj.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ki.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://lo.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gp.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zf.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lv.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qf.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nx.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mq.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kd.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lz.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://eg.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hd.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://av.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tv.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zk.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yh.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uo.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vb.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hw.gzmigu.cn

[K05] 深拷贝对象
来源：http://cb.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://br.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://nk.shxzukj.cn

JS:   structuredClone(obj)
来源：http://mn.colortex.cn

TS:   structuredClone(obj)
来源：http://nf.bookmarksfly.cn


<!-- 参考信息 -->