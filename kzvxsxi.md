代发 wailian999

H. 异常与错误处理
来源：http://dn.szsharing.cn

================================================================================
来源：http://kv.chemitech.net.cn

[H01] try / catch 基础
来源：http://pk.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jv.yuexingan06.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kw.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://os.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rz.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wa.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sj.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bs.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uj.szxytkj.cn

[H02] finally / ensure 收尾
来源：http://ti.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zh.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xn.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://os.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lh.bookmarksfly.cn

Java: try { f(); } finally { cleanup(); }
来源：http://op.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qr.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ju.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vp.jctech888.com.cn

[H03] 主动抛出异常
来源：http://bi.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://un.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hk.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://sk.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://sk.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ig.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gd.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://au.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://iu.huixinmuqiang.cn

[H04] 自定义异常类型
来源：http://ng.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://dd.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kh.huanxung.cn

JS:   class MyError extends Error {}
来源：http://mk.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://rp.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://fm.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://se.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://bi.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://bx.szsharing.cn

[H05] 捕获特定类型
来源：http://hj.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://kw.shxzskj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nr.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://og.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://uk.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://cl.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://aq.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://vg.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qz.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://ms.colortex.cn

Py:   value = d.get("k") or default
来源：http://dt.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://so.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kp.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://na.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ab.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yt.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://wd.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://cv.yuntaijiaju.cn

[H07] 断言
来源：http://bz.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://qz.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://ch.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://vf.newstarts.cn

TS:   console.assert(x > 0);
来源：http://oh.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://cw.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://py.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lv.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://vn.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://wc.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://ho.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ad.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://ga.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uo.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://db.shtwfgs.cn

Go:   err.Error()
来源：http://mq.521024.cn

Ruby: e.message;  e.backtrace
来源：http://px.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://vu.yuexingan06.cn

[H09] 带错误码的异常
来源：http://ui.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ms.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jk.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tj.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kk.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tk.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://km.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hj.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cx.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://jb.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://eb.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ko.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yz.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kq.muxihuayi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vm.jctech888.com.cn

Go:   defer f.Close()
来源：http://wj.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eq.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sg.nicolike.cn

================================================================================
来源：http://xg.lnxyls.cn

I. 正则表达式
来源：http://ql.jctech888.com.cn

================================================================================
来源：http://zs.newstarts.cn

[I01] 判断是否匹配
来源：http://vm.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://in.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cm.newstarts.cn

JS:   /\d+/.test(s)
来源：http://hf.nicolike.cn

TS:   /\d+/.test(s)
来源：http://cp.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://la.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wi.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://zi.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ge.bjjhwx.cn

[I02] 提取所有匹配
来源：http://dt.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://li.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cw.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mb.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://hx.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ko.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://km.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://hf.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nm.panjiajie.cn

[I03] 提取捕获分组
来源：http://ka.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uh.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uu.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vp.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ti.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fy.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yt.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://be.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fx.bookmarksfly.cn

[I04] 正则替换
来源：http://jy.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vp.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uw.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bz.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cl.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lx.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dy.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ch.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iu.hnjuh.cn

[I05] 按正则拆分
来源：http://lm.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ib.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xh.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://ut.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://mt.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://fi.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vf.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nj.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gn.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vz.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sw.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jx.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ge.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lg.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vo.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oo.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yw.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xn.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://pe.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ro.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dt.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kv.szsharing.cn

TS:   /error/gim
来源：http://tp.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xl.colortex.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vb.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://aw.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ph.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://ip.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qx.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ww.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nk.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zo.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iu.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tm.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hb.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wv.asd995.cn

================================================================================
来源：http://yf.hnjuh.cn

J. 日期与时间
来源：http://dr.huixinmuqiang.cn

================================================================================
来源：http://yf.szxytkj.cn

[J01] 获取当前时间
来源：http://nh.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cn.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cn.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://rl.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://xp.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lr.shtwfgs.cn

Go:   time.Now()
来源：http://ye.szsharing.cn

Ruby: Time.now
来源：http://ym.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tr.szsharing.cn

[J02] 格式化输出
来源：http://ih.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mp.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mq.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://er.haigaiapp.cn

TS:   d.toISOString()
来源：http://zd.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hp.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jn.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nn.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pc.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://yb.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qs.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dk.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://xq.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://ou.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bk.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ji.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://xx.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ge.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://nf.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pa.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tc.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nz.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mk.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vi.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hx.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rn.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zt.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://qn.wgjwhj.cn

Py:   now + timedelta(days=7)
来源：http://ax.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cl.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gv.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wu.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://iy.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dd.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://yi.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rj.panjiajie.cn

[J06] 计算两时间之差
来源：http://oo.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://vj.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://qd.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ao.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pk.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ih.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://go.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://aj.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://ub.huixiangedu.cn

[J07] 比较两个日期
来源：http://kx.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://sz.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wv.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ci.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jy.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wq.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fh.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ht.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://mt.szsharing.cn

[J08] 提取年月日与星期
来源：http://bo.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yf.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ok.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qc.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ln.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tr.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tw.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://br.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ja.shtwfgs.cn

[J09] 时区处理
来源：http://dg.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cf.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rm.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rl.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fh.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://og.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cu.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rm.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tx.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://bo.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bc.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qb.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rd.yuexingan06.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zr.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ip.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fc.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ze.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zb.haigaiapp.cn

================================================================================
来源：http://ib.hahajie.cn

K. JSON 与序列化
来源：http://hr.gzmigu.cn

================================================================================
来源：http://be.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://rv.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yz.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://av.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://ju.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://ni.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nc.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://ef.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dk.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bj.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://wr.newstarts.cn

Py:   json.loads(s)
来源：http://dq.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ou.colortex.cn

JS:   JSON.parse(s)
来源：http://ca.shxzukj.cn

TS:   JSON.parse(s)
来源：http://or.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mj.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://bp.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://yw.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ez.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://pu.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://de.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dm.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xd.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zo.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qk.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hc.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yh.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ms.newstarts.cn

[K04] 读取 JSON 文件
来源：http://nx.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nd.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gf.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gu.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rc.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ze.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eo.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ll.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://as.panjiajie.cn

[K05] 深拷贝对象
来源：http://ok.colortex.cn


<!-- 参考信息 -->