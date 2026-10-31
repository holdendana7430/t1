代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://qh.shxzukj.cn

Ruby: obj.instance_variables
来源：http://ns.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://mb.shxzskj.cn

================================================================================
来源：http://ve.yuexingan06.cn

H. 异常与错误处理
来源：http://pz.muxihuayi.cn

================================================================================
来源：http://ij.haigaiapp.cn

[H01] try / catch 基础
来源：http://cw.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ii.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bi.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ou.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uh.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wl.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ms.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xt.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ja.nszjky.cn

[H02] finally / ensure 收尾
来源：http://sm.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vn.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://db.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://un.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jc.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mc.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tr.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ko.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wf.lnxyls.cn

[H03] 主动抛出异常
来源：http://pn.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://dc.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eo.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://kp.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://oe.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ve.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lj.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ym.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ru.panjiajie.cn

[H04] 自定义异常类型
来源：http://fa.haigaiapp.cn

Py:   class MyError(Exception): pass
来源：http://ku.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nf.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://db.9csxet.cn

TS:   class MyError extends Error {}
来源：http://hy.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://iu.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mt.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://iz.hahajie.cn

C#:   class MyException : Exception {}
来源：http://rw.hnjuh.cn

[H05] 捕获特定类型
来源：http://qb.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://tf.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sk.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://hw.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://lt.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://wn.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hx.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://oq.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://in.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://qr.nszjky.cn

Py:   value = d.get("k") or default
来源：http://vu.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hc.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://me.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gl.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ak.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yv.hahajie.cn

Ruby: d&.dig(:a, :b)
来源：http://xe.szxytkj.cn

C#:   obj?.A?.B ?? default
来源：http://ax.gzmigu.cn

[H07] 断言
来源：http://cu.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://qx.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://tq.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://dn.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://we.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://ua.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ea.wgjwhj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ni.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://ao.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://nj.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://tv.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dn.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://dw.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mb.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jh.nszjky.cn

Go:   err.Error()
来源：http://nk.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://zb.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://dd.jianghongdianzi.cn

[H09] 带错误码的异常
来源：http://fc.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://op.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wm.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rl.newstarts.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rw.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vw.szsharing.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uz.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cr.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zl.huanxung.cn

[H10] 资源自动释放
来源：http://zz.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rg.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pc.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ew.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xy.huixiangedu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://li.colortex.cn

Go:   defer f.Close()
来源：http://dc.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://su.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mp.haigaiapp.cn

================================================================================
来源：http://kv.521024.cn

I. 正则表达式
来源：http://by.521024.cn

================================================================================
来源：http://ou.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://vr.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zx.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vk.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://mz.newstarts.cn

TS:   /\d+/.test(s)
来源：http://no.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lb.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yh.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://ma.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sk.szxytkj.cn

[I02] 提取所有匹配
来源：http://lx.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://ge.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dl.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ck.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://zc.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nd.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zm.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://gv.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gc.asd995.cn

[I03] 提取捕获分组
来源：http://do.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fb.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uw.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://at.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xs.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iq.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://we.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xt.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gt.9csxet.cn

[I04] 正则替换
来源：http://ka.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bf.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kx.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ze.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kw.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tf.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pt.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gt.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sp.muxihuayi.cn

[I05] 按正则拆分
来源：http://no.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vb.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vl.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://cf.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://in.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://zx.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xg.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zd.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gs.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bc.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yz.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ba.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zw.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fn.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://za.bookmarksfly.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wb.jianghongdianzi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://th.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wx.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://sl.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cd.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rf.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zw.newstarts.cn

TS:   /error/gim
来源：http://gp.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oa.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kx.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://sx.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ja.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://wx.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qr.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gf.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://is.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ll.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hv.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ap.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wr.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oy.shxzskj.cn

================================================================================
来源：http://wf.9csxet.cn

J. 日期与时间
来源：http://lh.nicolike.cn

================================================================================
来源：http://tc.nszjky.cn

[J01] 获取当前时间
来源：http://ug.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yi.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fm.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://ox.newstarts.cn

TS:   new Date();  Date.now()
来源：http://lb.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zn.lnxyls.cn

Go:   time.Now()
来源：http://ul.colortex.cn

Ruby: Time.now
来源：http://es.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pb.asd995.cn

[J02] 格式化输出
来源：http://qf.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yp.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vn.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ca.huixiangedu.cn

TS:   d.toISOString()
来源：http://cp.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fy.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ls.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lm.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wu.hahajie.cn

[J03] 字符串解析为日期
来源：http://wk.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nv.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://en.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://hu.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://tv.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xn.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bc.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://xh.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://au.huanxung.cn

[J04] 时间戳与日期互转
来源：http://bm.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://to.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ue.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ve.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tk.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zj.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qd.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nz.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sz.huanxung.cn

[J05] 时间加减（加 7 天）
来源：http://ib.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://wn.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mt.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://of.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cf.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://vo.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hf.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://kz.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://oj.shtwfgs.cn

[J06] 计算两时间之差
来源：http://sm.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://az.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://sn.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gt.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wz.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://om.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://ip.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://xr.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://mp.bjjhwx.cn

[J07] 比较两个日期
来源：http://za.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://fo.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ki.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://on.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rq.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ei.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ak.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ld.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://xb.panjiajie.cn

[J08] 提取年月日与星期
来源：http://fk.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rs.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sa.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wr.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wf.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gb.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dy.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ll.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qh.yuntaijiaju.cn

[J09] 时区处理
来源：http://lu.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sx.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pv.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://al.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nm.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pw.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://du.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://eu.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mb.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://ok.gzmigu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nu.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nd.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zp.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mg.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rs.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://um.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wo.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kx.huixinmuqiang.cn

================================================================================
来源：http://ph.shxzskj.cn

K. JSON 与序列化
来源：http://pn.yuntaijiaju.cn

================================================================================
来源：http://uj.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://mo.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ys.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bj.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://it.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://hm.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ji.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://jf.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ot.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mt.szsharing.cn

[K02] JSON 字符串转对象
来源：http://zq.shxzukj.cn

Py:   json.loads(s)
来源：http://mm.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dm.gzmigu.cn

JS:   JSON.parse(s)
来源：http://kd.huanxung.cn

TS:   JSON.parse(s)
来源：http://xv.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hd.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://zy.521024.cn

Ruby: JSON.parse(s)
来源：http://pw.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gs.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://od.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dx.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bl.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ag.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://si.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fr.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rl.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vx.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ez.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://kv.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jz.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://np.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tk.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wp.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wj.newstarts.cn


<!-- 参考信息 -->