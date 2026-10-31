代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://yi.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://rr.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://zl.yuntaijiaju.cn

================================================================================
来源：http://kv.szsharing.cn

H. 异常与错误处理
来源：http://jy.nicolike.cn

================================================================================
来源：http://ew.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://mt.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sm.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ni.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nr.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tr.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mh.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iw.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://am.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gt.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://yh.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nz.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nk.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uz.9csxet.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qx.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hz.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pa.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://js.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ax.newstarts.cn

[H03] 主动抛出异常
来源：http://oy.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://yl.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ox.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://br.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://wz.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bb.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oc.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://up.gzmigu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gf.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://dv.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://nz.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://up.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://dp.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://nq.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://je.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kx.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://ee.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://rc.bjjhwx.cn

[H05] 捕获特定类型
来源：http://ls.szsharing.cn

Py:   except ValueError as e:
来源：http://tk.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cw.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://fx.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://ok.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://np.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ul.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://ss.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gl.szxytkj.cn

[H06] 可选值 / 空值安全访问
来源：http://bk.huanxung.cn

Py:   value = d.get("k") or default
来源：http://su.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vc.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xi.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://re.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ln.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hm.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://xw.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://nm.huixiangedu.cn

[H07] 断言
来源：http://eo.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://bc.panjiajie.cn

PHP:  assert($x > 0);
来源：http://mc.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://qk.colortex.cn

TS:   console.assert(x > 0);
来源：http://ok.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://lc.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ln.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://br.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://hx.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://by.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://ov.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iy.huanxung.cn

JS:   e.message;  e.stack
来源：http://vh.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xq.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sk.yuntaijiaju.cn

Go:   err.Error()
来源：http://wz.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://bd.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://zm.9csxet.cn

[H09] 带错误码的异常
来源：http://qy.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lg.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lz.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hi.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://in.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tq.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cm.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ge.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mf.huixiangedu.cn

[H10] 资源自动释放
来源：http://sh.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jv.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://la.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kp.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rs.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dt.szsharing.cn

Go:   defer f.Close()
来源：http://vi.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ph.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xo.bjjhwx.cn

================================================================================
来源：http://pv.huixinmuqiang.cn

I. 正则表达式
来源：http://vc.9csxet.cn

================================================================================
来源：http://wf.shxzukj.cn

[I01] 判断是否匹配
来源：http://mj.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rk.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fc.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://fb.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://lz.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eq.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yv.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://wy.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sz.shtwfgs.cn

[I02] 提取所有匹配
来源：http://pc.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://mi.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://en.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://py.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://vi.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zn.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zg.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://wa.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zn.yuexingan06.cn

[I03] 提取捕获分组
来源：http://re.jianghongdianzi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eu.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hq.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ss.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eg.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pu.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eg.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tt.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vx.nicolike.cn

[I04] 正则替换
来源：http://dg.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qy.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aj.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cj.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://iu.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zx.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://og.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uq.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cu.colortex.cn

[I05] 按正则拆分
来源：http://vb.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xt.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dx.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ym.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://my.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://wg.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jk.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rx.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qh.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lw.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zu.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hu.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ae.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kx.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wn.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rc.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eb.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sq.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://yr.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pw.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ya.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://du.yuntaijiaju.cn

TS:   /error/gim
来源：http://gl.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hu.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pf.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://uz.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dp.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://ew.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sd.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eo.shxzukj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://me.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fg.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fz.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aq.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kh.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://td.panjiajie.cn

================================================================================
来源：http://li.521024.cn

J. 日期与时间
来源：http://zj.jianghongdianzi.cn

================================================================================
来源：http://fl.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://zz.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yj.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wn.nszjky.cn

JS:   new Date();  Date.now()
来源：http://pi.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://zw.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sp.panjiajie.cn

Go:   time.Now()
来源：http://et.muxihuayi.cn

Ruby: Time.now
来源：http://ve.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://up.shxzukj.cn

[J02] 格式化输出
来源：http://ir.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vp.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vd.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uu.panjiajie.cn

TS:   d.toISOString()
来源：http://qk.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tk.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hy.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oh.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vs.521024.cn

[J03] 字符串解析为日期
来源：http://wq.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dx.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vd.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://ta.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://yb.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mj.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wl.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://yj.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ah.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://lu.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://it.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tn.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sq.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wm.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ib.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ju.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sp.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oh.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://nr.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://fg.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tk.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yt.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hw.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://an.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hu.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://js.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jd.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://mv.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://mw.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://zy.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vp.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fr.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://aq.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://ro.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://vt.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://cj.nszjky.cn

[J07] 比较两个日期
来源：http://jd.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://dn.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xz.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yu.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hm.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zr.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yv.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://es.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://sn.newstarts.cn

[J08] 提取年月日与星期
来源：http://im.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dq.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lg.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hh.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hx.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xt.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xw.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uu.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vg.szxytkj.cn

[J09] 时区处理
来源：http://sp.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ko.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://if.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lf.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zb.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://je.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gf.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://aq.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ir.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://tb.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ou.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dx.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jk.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://to.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oq.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tb.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cx.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oj.muxihuayi.cn

================================================================================
来源：http://wx.shtwfgs.cn

K. JSON 与序列化
来源：http://qb.shtwfgs.cn

================================================================================
来源：http://kq.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://ea.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zb.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kp.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://zo.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://ud.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hw.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://nz.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://id.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://js.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://md.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://hw.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ho.9csxet.cn

JS:   JSON.parse(s)
来源：http://dh.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://tt.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jk.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://ey.colortex.cn

Ruby: JSON.parse(s)
来源：http://kt.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pw.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://dt.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aa.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xm.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wn.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xi.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ha.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bt.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ya.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pl.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://gt.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fh.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://le.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fn.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bu.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jo.lnxyls.cn


<!-- 参考信息 -->