代发 wailian999

H. 异常与错误处理
来源：http://ir.hnjuh.cn

================================================================================
来源：http://sq.yuexingan06.cn

[H01] try / catch 基础
来源：http://kh.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vs.colortex.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ab.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fd.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://un.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yg.haigaiapp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nf.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ys.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bv.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://ka.colortex.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xp.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://es.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://te.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://az.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://im.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mf.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vr.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bz.asd995.cn

[H03] 主动抛出异常
来源：http://kp.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://yk.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pi.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://be.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://hw.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hi.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sn.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zn.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yu.521024.cn

[H04] 自定义异常类型
来源：http://nk.asd995.cn

Py:   class MyError(Exception): pass
来源：http://yv.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://es.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://zl.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://vl.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://mz.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lr.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://ob.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://iv.muxihuayi.cn

[H05] 捕获特定类型
来源：http://wu.colortex.cn

Py:   except ValueError as e:
来源：http://ki.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mh.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://yq.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://tg.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://ki.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wc.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://id.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qf.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://so.huanxung.cn

Py:   value = d.get("k") or default
来源：http://yf.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cx.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qd.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ge.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xf.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uz.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://yn.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://mg.newstarts.cn

[H07] 断言
来源：http://dd.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://cg.panjiajie.cn

PHP:  assert($x > 0);
来源：http://rv.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://ch.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://se.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://kf.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zf.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://is.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://vz.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://yp.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://mz.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oc.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://tq.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yz.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ol.newstarts.cn

Go:   err.Error()
来源：http://ki.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://ac.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://fk.shxzukj.cn

[H09] 带错误码的异常
来源：http://bs.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ht.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ff.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oc.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lr.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gq.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ll.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dg.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jf.panjiajie.cn

[H10] 资源自动释放
来源：http://vv.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ha.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ev.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wm.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://su.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wl.wgjwhj.cn

Go:   defer f.Close()
来源：http://le.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oj.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ei.9csxet.cn

================================================================================
来源：http://zz.huixiangedu.cn

I. 正则表达式
来源：http://tc.yuntaijiaju.cn

================================================================================
来源：http://db.521024.cn

[I01] 判断是否匹配
来源：http://uv.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xa.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hs.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://sm.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://yy.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fc.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bu.shtwfgs.cn

Ruby: s.match?(/\d+/)
来源：http://gl.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rm.shxzukj.cn

[I02] 提取所有匹配
来源：http://es.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://ue.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xb.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bq.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://jr.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vr.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gv.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://tw.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qw.colortex.cn

[I03] 提取捕获分组
来源：http://vs.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ac.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qk.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ll.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jl.yuexingan06.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wi.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nz.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pp.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ib.muxihuayi.cn

[I04] 正则替换
来源：http://sq.gzmigu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cw.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://in.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fe.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cw.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yd.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://im.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yh.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ct.wgjwhj.cn

[I05] 按正则拆分
来源：http://wv.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fe.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uf.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://bt.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://tj.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://ro.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zn.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://me.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wc.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oo.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cc.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://df.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://db.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yz.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://av.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wq.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yy.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://df.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://ij.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qw.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bl.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jr.szsharing.cn

TS:   /error/gim
来源：http://bc.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cx.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ay.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://an.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ob.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://qf.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xw.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ck.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bg.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mg.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wl.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://id.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ox.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://no.szsharing.cn

================================================================================
来源：http://du.yuntaijiaju.cn

J. 日期与时间
来源：http://tq.shxzskj.cn

================================================================================
来源：http://es.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://vy.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wn.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qu.hahajie.cn

JS:   new Date();  Date.now()
来源：http://vj.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://mc.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qn.gzmigu.cn

Go:   time.Now()
来源：http://xz.chemitech.net.cn

Ruby: Time.now
来源：http://kh.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yu.panjiajie.cn

[J02] 格式化输出
来源：http://bz.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vy.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fj.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qf.wgjwhj.cn

TS:   d.toISOString()
来源：http://yf.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pt.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yi.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hq.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vv.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://jn.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nh.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kp.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://lf.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://xq.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://em.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://di.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://cp.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rp.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://vq.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ov.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gr.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gi.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://iy.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://if.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bn.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oh.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rv.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://ez.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://bl.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cr.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dj.bookmarksfly.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lj.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://kb.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ef.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://tc.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qg.szxytkj.cn

[J06] 计算两时间之差
来源：http://bu.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://wm.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://mc.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vf.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ei.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ff.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://gj.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://uz.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://yg.nszjky.cn

[J07] 比较两个日期
来源：http://cl.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://tj.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kd.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://os.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mn.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kq.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zt.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uw.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://dv.lnxyls.cn

[J08] 提取年月日与星期
来源：http://cx.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hq.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rq.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://za.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rd.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://te.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ko.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wd.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tp.gzmigu.cn

[J09] 时区处理
来源：http://au.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oi.nicolike.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bj.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fb.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pz.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cc.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vn.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ls.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://af.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://xp.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fa.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://me.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://js.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zo.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qq.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zz.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hd.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ka.lnxyls.cn

================================================================================
来源：http://ud.shtwfgs.cn

K. JSON 与序列化
来源：http://ec.asd995.cn

================================================================================
来源：http://hk.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://al.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xq.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jf.colortex.cn

JS:   JSON.stringify(obj)
来源：http://tk.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://iz.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ua.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://ej.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bx.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://td.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://ul.9csxet.cn

Py:   json.loads(s)
来源：http://gp.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hb.shxzskj.cn

JS:   JSON.parse(s)
来源：http://mg.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://qx.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://du.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://ar.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://jh.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dx.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://cv.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pg.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ng.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lv.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fe.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gd.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ev.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sw.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xh.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://uc.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ju.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://en.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wx.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bu.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sw.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xz.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sc.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hx.newstarts.cn

[K05] 深拷贝对象
来源：http://kc.szxytkj.cn


<!-- 参考信息 -->