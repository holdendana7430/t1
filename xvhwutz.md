代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://di.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cb.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wa.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jd.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ui.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gr.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ai.colortex.cn

[H02] finally / ensure 收尾
来源：http://jn.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://df.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jb.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sw.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://we.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fx.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oq.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uc.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oa.9csxet.cn

[H03] 主动抛出异常
来源：http://ys.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://dp.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ro.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://ct.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://ia.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tp.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jp.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dm.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://eh.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://nv.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://zv.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://id.hahajie.cn

JS:   class MyError extends Error {}
来源：http://qy.521024.cn

TS:   class MyError extends Error {}
来源：http://ja.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://uw.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mi.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://rj.nszjky.cn

C#:   class MyException : Exception {}
来源：http://mq.nicolike.cn

[H05] 捕获特定类型
来源：http://oz.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://sx.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pf.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://bn.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://jb.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://ek.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ue.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://xr.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mp.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://se.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://pj.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lu.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jf.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qa.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hb.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yw.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://vu.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://je.haigaiapp.cn

[H07] 断言
来源：http://av.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://sm.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://xj.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://ni.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://ri.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://os.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://en.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://va.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://fa.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://kj.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://tr.gzmigu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ky.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://im.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fd.yuexingan06.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ck.nszjky.cn

Go:   err.Error()
来源：http://tz.hahajie.cn

Ruby: e.message;  e.backtrace
来源：http://ww.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://gh.yuexingan06.cn

[H09] 带错误码的异常
来源：http://fu.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mz.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ek.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://en.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ju.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wk.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ib.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gl.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qm.nicolike.cn

[H10] 资源自动释放
来源：http://vs.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vc.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rl.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bt.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yv.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lp.lnxyls.cn

Go:   defer f.Close()
来源：http://di.521024.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ad.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sb.nszjky.cn

================================================================================
来源：http://pb.9csxet.cn

I. 正则表达式
来源：http://la.huixinmuqiang.cn

================================================================================
来源：http://hr.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://ne.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ae.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zu.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://wm.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://yf.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cm.colortex.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://by.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://fg.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sj.muxihuayi.cn

[I02] 提取所有匹配
来源：http://sw.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://qr.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://df.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rr.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://lq.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mo.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cz.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://iu.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bl.muxihuayi.cn

[I03] 提取捕获分组
来源：http://wx.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tg.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ne.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gt.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xn.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aa.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lo.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xc.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qf.9csxet.cn

[I04] 正则替换
来源：http://dp.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sq.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hn.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mq.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xs.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fd.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hk.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gx.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qk.wgjwhj.cn

[I05] 按正则拆分
来源：http://zh.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kv.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jr.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://ms.lnxyls.cn

TS:   s.split(/\s*,\s*/)
来源：http://oi.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://kz.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nr.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zy.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ax.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lv.hnjuh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ga.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mo.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lp.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dg.huanxung.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zf.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sy.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fs.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xb.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://iy.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rs.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sk.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://so.asd995.cn

TS:   /error/gim
来源：http://uq.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iq.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gn.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://my.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xa.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://ub.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tq.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sd.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lq.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ky.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gf.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rc.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gb.shxzukj.cn

================================================================================
来源：http://ai.jianghongdianzi.cn

J. 日期与时间
来源：http://ox.shxzskj.cn

================================================================================
来源：http://xi.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://ke.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wy.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dt.hahajie.cn

JS:   new Date();  Date.now()
来源：http://vd.nszjky.cn

TS:   new Date();  Date.now()
来源：http://ni.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wd.shxzskj.cn

Go:   time.Now()
来源：http://np.newstarts.cn

Ruby: Time.now
来源：http://hm.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://af.colortex.cn

[J02] 格式化输出
来源：http://aw.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ie.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nj.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dc.bookmarksfly.cn

TS:   d.toISOString()
来源：http://jv.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oy.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jq.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ld.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://go.gzmigu.cn

[J03] 字符串解析为日期
来源：http://po.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ad.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ch.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://ss.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://hc.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fc.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oe.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://mx.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gd.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://gn.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cl.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hk.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ds.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xk.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wz.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fp.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ic.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jb.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://sx.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://fc.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tm.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vu.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dz.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://jb.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://re.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://kd.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wv.521024.cn

[J06] 计算两时间之差
来源：http://oq.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://av.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://dr.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://id.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://om.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rr.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://qd.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://tx.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://td.hnjuh.cn

[J07] 比较两个日期
来源：http://pj.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://ki.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://th.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ne.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yv.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fv.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ot.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cc.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ff.nicolike.cn

[J08] 提取年月日与星期
来源：http://jt.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dg.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://px.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fa.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fm.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nw.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qj.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dr.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zy.bjjhwx.cn

[J09] 时区处理
来源：http://ex.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rs.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nm.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jz.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ci.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yv.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fk.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hc.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mp.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://em.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://td.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qn.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rg.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ww.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bw.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ny.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bh.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xh.nszjky.cn

================================================================================
来源：http://do.wgjwhj.cn

K. JSON 与序列化
来源：http://wf.newstarts.cn

================================================================================
来源：http://wu.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://nt.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ib.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fk.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://ep.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://gt.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jp.nicolike.cn

Go:   json.Marshal(obj)
来源：http://vf.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sb.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xt.hahajie.cn

[K02] JSON 字符串转对象
来源：http://cl.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://bd.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eq.shxzskj.cn

JS:   JSON.parse(s)
来源：http://ig.nicolike.cn

TS:   JSON.parse(s)
来源：http://gs.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jp.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://gs.szsharing.cn

Ruby: JSON.parse(s)
来源：http://nv.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qd.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://jn.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://do.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xq.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qo.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bm.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://re.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wm.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fp.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yd.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://fi.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wh.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aa.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sp.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oh.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ew.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vq.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qm.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iz.szxytkj.cn

[K05] 深拷贝对象
来源：http://zu.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://ht.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://xu.nicolike.cn

JS:   structuredClone(obj)
来源：http://zh.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://xi.colortex.cn


<!-- 参考信息 -->