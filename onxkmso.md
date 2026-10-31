代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://at.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pw.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pt.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wk.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yb.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dp.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vk.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://my.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xz.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kq.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gu.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rc.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fg.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gp.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ui.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nu.szxytkj.cn

[H03] 主动抛出异常
来源：http://qy.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://md.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sz.521024.cn

JS:   throw new Error("错误信息");
来源：http://ws.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://vg.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sa.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ph.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mp.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ta.huanxung.cn

[H04] 自定义异常类型
来源：http://rw.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://er.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://iy.hahajie.cn

JS:   class MyError extends Error {}
来源：http://so.newstarts.cn

TS:   class MyError extends Error {}
来源：http://dr.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://ij.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dj.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://wm.huanxung.cn

C#:   class MyException : Exception {}
来源：http://cv.panjiajie.cn

[H05] 捕获特定类型
来源：http://ib.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://rl.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ky.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://pu.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://hv.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://wk.nszjky.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wa.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://md.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qd.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://el.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://if.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ji.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uw.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://of.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ry.nszjky.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ya.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://rq.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://ay.lnxyls.cn

[H07] 断言
来源：http://ru.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://kq.nicolike.cn

PHP:  assert($x > 0);
来源：http://ys.nszjky.cn

JS:   console.assert(x > 0);
来源：http://la.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://lm.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://xy.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nw.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xi.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://io.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://rh.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://cp.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://le.huanxung.cn

JS:   e.message;  e.stack
来源：http://zn.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wn.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ng.nicolike.cn

Go:   err.Error()
来源：http://xr.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://cf.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://ft.haigaiapp.cn

[H09] 带错误码的异常
来源：http://tc.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://sd.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fv.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ni.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vk.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nb.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qt.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rx.colortex.cn

[H10] 资源自动释放
来源：http://ie.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bp.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oh.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ft.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gb.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ne.hahajie.cn

Go:   defer f.Close()
来源：http://aw.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tg.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://au.szsharing.cn

================================================================================
来源：http://jq.lnxyls.cn

I. 正则表达式
来源：http://mh.shtwfgs.cn

================================================================================
来源：http://np.shtwfgs.cn

[I01] 判断是否匹配
来源：http://zn.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gj.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gq.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://xx.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://sg.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lg.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ux.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://cs.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zt.wgjwhj.cn

[I02] 提取所有匹配
来源：http://ki.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://yy.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jr.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bk.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://nm.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yq.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yf.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://hs.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pm.panjiajie.cn

[I03] 提取捕获分组
来源：http://lx.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gv.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dm.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qx.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zy.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sv.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dv.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yz.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ap.huixinmuqiang.cn

[I04] 正则替换
来源：http://jg.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xb.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yy.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ey.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tc.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ri.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lc.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ek.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://io.nicolike.cn

[I05] 按正则拆分
来源：http://dt.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yk.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hb.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://ee.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://vs.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://qv.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ab.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jt.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mi.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qa.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pi.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://km.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lj.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lp.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mz.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pt.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jm.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dz.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://qp.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hy.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xc.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rt.huanxung.cn

TS:   /error/gim
来源：http://vf.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uh.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://im.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://qh.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uz.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://wo.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ah.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ys.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mn.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lg.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vm.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lk.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://et.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xu.colortex.cn

================================================================================
来源：http://tp.wgjwhj.cn

J. 日期与时间
来源：http://ns.szxytkj.cn

================================================================================
来源：http://qv.haigaiapp.cn

[J01] 获取当前时间
来源：http://vd.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yc.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://to.newstarts.cn

JS:   new Date();  Date.now()
来源：http://or.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://ft.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sd.wgjwhj.cn

Go:   time.Now()
来源：http://ht.huixinmuqiang.cn

Ruby: Time.now
来源：http://ib.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qi.szsharing.cn

[J02] 格式化输出
来源：http://cw.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ew.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hc.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ov.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://av.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gf.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yc.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uu.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ho.shxzskj.cn

[J03] 字符串解析为日期
来源：http://jx.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rh.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cu.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://ow.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://hr.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rj.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://un.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://jl.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cz.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://km.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hl.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fu.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xv.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kx.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bw.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wd.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jm.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mh.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://ov.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://cy.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dp.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hj.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ja.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://fr.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qu.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://ju.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wy.nszjky.cn

[J06] 计算两时间之差
来源：http://bx.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://qr.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://ju.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kb.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ka.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ht.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://vo.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://jp.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://an.gzmigu.cn

[J07] 比较两个日期
来源：http://tf.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://hs.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xp.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nx.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://my.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dp.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cb.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jc.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://kj.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://nr.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tn.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ji.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://df.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oo.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gi.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://re.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cn.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tq.yuntaijiaju.cn

[J09] 时区处理
来源：http://gs.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mn.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rj.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pm.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sq.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kc.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ay.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ll.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nj.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://xp.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xt.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sd.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ac.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vi.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rt.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pi.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tm.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sm.haigaiapp.cn

================================================================================
来源：http://cs.szxytkj.cn

K. JSON 与序列化
来源：http://ie.shxzskj.cn

================================================================================
来源：http://om.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://ld.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xk.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gm.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://zt.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://mc.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sx.9csxet.cn

Go:   json.Marshal(obj)
来源：http://po.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tm.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pj.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://lg.huanxung.cn

Py:   json.loads(s)
来源：http://uw.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jf.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://kr.huanxung.cn

TS:   JSON.parse(s)
来源：http://mv.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cj.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://ma.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://qn.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rd.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://of.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pc.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ab.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vn.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gw.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iw.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pt.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://db.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zb.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://lg.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lw.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qk.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qi.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qx.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pu.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qq.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jx.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kq.szsharing.cn

[K05] 深拷贝对象
来源：http://dd.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://mr.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://yo.9csxet.cn

JS:   structuredClone(obj)
来源：http://cn.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://qy.colortex.cn


<!-- 参考信息 -->