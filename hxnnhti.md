代发 wailian999

H. 异常与错误处理
来源：http://wc.yuexingan06.cn

================================================================================
来源：http://he.chemitech.net.cn

[H01] try / catch 基础
来源：http://kt.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nd.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://td.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yc.hahajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vy.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://in.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zm.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pt.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cv.szsharing.cn

[H02] finally / ensure 收尾
来源：http://nd.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ng.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qj.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lz.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wo.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ix.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nq.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tz.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fk.hnjuh.cn

[H03] 主动抛出异常
来源：http://yx.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://ik.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lv.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://fz.521024.cn

TS:   throw new Error("错误信息");
来源：http://po.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dv.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cm.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zu.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hn.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://kx.asd995.cn

Py:   class MyError(Exception): pass
来源：http://us.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fy.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://oe.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://na.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://zs.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://py.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://xh.lnxyls.cn

C#:   class MyException : Exception {}
来源：http://ul.gzmigu.cn

[H05] 捕获特定类型
来源：http://ra.huanxung.cn

Py:   except ValueError as e:
来源：http://xy.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lc.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://vp.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://fe.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://ua.nszjky.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://if.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://dz.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sc.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://ev.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://hv.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://eo.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ab.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cx.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fi.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gf.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://pp.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://np.chemitech.net.cn

[H07] 断言
来源：http://gm.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://iv.panjiajie.cn

PHP:  assert($x > 0);
来源：http://pb.521024.cn

JS:   console.assert(x > 0);
来源：http://ur.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://xl.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://pp.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ro.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qg.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://mr.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://kj.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://et.nszjky.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://km.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://um.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xn.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hw.hahajie.cn

Go:   err.Error()
来源：http://ao.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://fd.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://om.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://mq.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yg.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://iz.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://il.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dz.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yd.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vc.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wj.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mp.nicolike.cn

[H10] 资源自动释放
来源：http://hu.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ve.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jt.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fb.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qz.huixiangedu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://re.nicolike.cn

Go:   defer f.Close()
来源：http://vj.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xk.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uc.lnxyls.cn

================================================================================
来源：http://xh.shxzukj.cn

I. 正则表达式
来源：http://ai.jianghongdianzi.cn

================================================================================
来源：http://tt.chemitech.net.cn

[I01] 判断是否匹配
来源：http://yq.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yr.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zt.asd995.cn

JS:   /\d+/.test(s)
来源：http://iz.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://gt.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dy.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://at.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://mo.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zr.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://aq.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://hh.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rr.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tn.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://uc.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ve.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://em.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://xg.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wd.shxzukj.cn

[I03] 提取捕获分组
来源：http://ue.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ue.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bb.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kc.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kq.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vy.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cv.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://su.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ms.bookmarksfly.cn

[I04] 正则替换
来源：http://ld.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ys.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qb.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ww.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://at.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://of.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ys.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tx.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yk.bjjhwx.cn

[I05] 按正则拆分
来源：http://dt.521024.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://io.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oq.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://ml.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://tk.bookmarksfly.cn

Java: s.split("\\s*,\\s*")
来源：http://xv.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ti.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dv.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nf.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zb.asd995.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ur.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aa.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wi.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dw.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tv.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gz.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vb.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nt.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://po.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qd.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://px.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ea.colortex.cn

TS:   /error/gim
来源：http://jc.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dx.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qf.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://ei.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zu.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://qx.521024.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tx.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tx.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uc.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lg.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oj.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ft.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ht.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kv.panjiajie.cn

================================================================================
来源：http://ld.hnjuh.cn

J. 日期与时间
来源：http://by.9csxet.cn

================================================================================
来源：http://fr.bjjhwx.cn

[J01] 获取当前时间
来源：http://yj.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yv.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ej.colortex.cn

JS:   new Date();  Date.now()
来源：http://zl.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://zr.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ph.huanxung.cn

Go:   time.Now()
来源：http://dv.hahajie.cn

Ruby: Time.now
来源：http://ej.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lx.jianghongdianzi.cn

[J02] 格式化输出
来源：http://uf.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ss.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sq.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tc.szsharing.cn

TS:   d.toISOString()
来源：http://yx.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cb.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://um.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zh.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wm.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://qz.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pp.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cb.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://zi.asd995.cn

TS:   new Date("2024-01-02")
来源：http://gs.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tk.newstarts.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zs.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://pb.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zj.huanxung.cn

[J04] 时间戳与日期互转
来源：http://vl.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mh.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ri.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://es.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qp.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ax.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://on.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wd.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qr.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://qx.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://aw.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xj.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tp.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cq.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://fg.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://la.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://vx.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sb.asd995.cn

[J06] 计算两时间之差
来源：http://qj.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://jr.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://kn.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cj.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fh.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lg.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://gp.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://mr.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://ix.nszjky.cn

[J07] 比较两个日期
来源：http://nu.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://ds.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cy.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fu.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nk.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ly.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lw.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qz.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://si.huanxung.cn

[J08] 提取年月日与星期
来源：http://dy.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vu.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cy.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yb.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oh.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cv.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://od.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dx.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ht.gzmigu.cn

[J09] 时区处理
来源：http://av.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wx.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qz.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hj.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sc.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xj.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zj.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zw.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cf.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://by.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uj.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yn.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nm.yuexingan06.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wc.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pa.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://la.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rk.huixinmuqiang.cn

================================================================================
来源：http://av.haigaiapp.cn

K. JSON 与序列化
来源：http://ah.wgjwhj.cn

================================================================================
来源：http://jz.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://cs.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wo.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ek.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://ng.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://cd.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zj.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://xy.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://eb.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cs.521024.cn

[K02] JSON 字符串转对象
来源：http://nn.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://nh.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nr.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://jt.huanxung.cn

TS:   JSON.parse(s)
来源：http://mi.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ra.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://cu.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://eo.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jv.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://qk.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ru.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://em.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://js.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mj.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cs.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dr.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bi.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vh.newstarts.cn

[K04] 读取 JSON 文件
来源：http://nt.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yn.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wm.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ve.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://el.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bg.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rn.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ko.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pr.nszjky.cn

[K05] 深拷贝对象
来源：http://wf.haigaiapp.cn


<!-- 参考信息 -->