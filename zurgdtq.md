代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://od.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fj.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vn.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://df.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qp.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yp.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qy.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://lk.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cl.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ra.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://em.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zj.szsharing.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gj.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jj.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ea.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rb.huanxung.cn

[H03] 主动抛出异常
来源：http://bl.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://cg.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ru.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://za.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://ap.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qi.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jj.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zt.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hr.colortex.cn

[H04] 自定义异常类型
来源：http://mm.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://bq.nszjky.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wr.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://gq.panjiajie.cn

TS:   class MyError extends Error {}
来源：http://tt.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://is.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fm.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://dp.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://vs.shtwfgs.cn

[H05] 捕获特定类型
来源：http://lz.jctech888.com.cn

Py:   except ValueError as e:
来源：http://jg.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hc.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://wq.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://bl.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://mm.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sj.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://lk.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yr.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://jm.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://rr.haigaiapp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zf.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mo.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sa.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uw.521024.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lb.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://vl.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://mi.szsharing.cn

[H07] 断言
来源：http://we.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://hs.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://mp.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://zt.nszjky.cn

TS:   console.assert(x > 0);
来源：http://sz.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://px.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mw.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mu.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://cy.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://lc.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://jw.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jo.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://ys.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dh.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ew.shtwfgs.cn

Go:   err.Error()
来源：http://br.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://gh.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://gb.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://wa.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bu.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qb.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bu.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bc.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ox.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fu.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mo.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hk.colortex.cn

[H10] 资源自动释放
来源：http://bo.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ld.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lg.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sc.hnjuh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nj.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://js.colortex.cn

Go:   defer f.Close()
来源：http://dj.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tj.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://px.hahajie.cn

================================================================================
来源：http://af.shtwfgs.cn

I. 正则表达式
来源：http://sr.yuntaijiaju.cn

================================================================================
来源：http://ns.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://yd.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wx.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hr.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://gy.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://yz.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qy.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hv.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://jq.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xa.nicolike.cn

[I02] 提取所有匹配
来源：http://gb.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://gv.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gk.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rx.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://zt.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hw.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zv.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://iv.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ep.szsharing.cn

[I03] 提取捕获分组
来源：http://jm.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://re.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://om.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dq.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ty.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wd.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://so.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nd.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gb.jianghongdianzi.cn

[I04] 正则替换
来源：http://ms.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ip.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yo.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fq.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ww.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://oc.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xc.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cf.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gl.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://wp.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jh.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cx.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://st.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://rm.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://fd.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zh.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yh.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://da.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dp.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vk.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tz.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dh.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ax.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vm.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fp.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kw.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zd.521024.cn

[I07] 忽略大小写与多行模式
来源：http://zi.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ke.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ee.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ze.wgjwhj.cn

TS:   /error/gim
来源：http://fn.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yq.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zn.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://hu.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tp.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ww.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://py.yuntaijiaju.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://we.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mi.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zd.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sy.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rj.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://km.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ff.nicolike.cn

================================================================================
来源：http://py.hahajie.cn

J. 日期与时间
来源：http://dg.bookmarksfly.cn

================================================================================
来源：http://va.shxzskj.cn

[J01] 获取当前时间
来源：http://tg.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rk.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://as.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://jz.colortex.cn

TS:   new Date();  Date.now()
来源：http://xy.chemitech.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pa.huixinmuqiang.cn

Go:   time.Now()
来源：http://mh.wgjwhj.cn

Ruby: Time.now
来源：http://ol.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://og.gzmigu.cn

[J02] 格式化输出
来源：http://yp.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sf.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qc.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zu.nszjky.cn

TS:   d.toISOString()
来源：http://yo.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sz.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pg.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mw.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://id.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://ry.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mv.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fl.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://jt.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://fj.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ii.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ij.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://qw.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zp.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://iw.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ch.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sl.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pp.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fs.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nt.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ux.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dh.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ro.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://ja.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://ma.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zp.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ix.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xc.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://jn.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ks.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://uf.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lh.9csxet.cn

[J06] 计算两时间之差
来源：http://ru.521024.cn

Py:   (end - start).total_seconds()
来源：http://ko.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://be.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jb.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mv.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dx.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://mm.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://du.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://hx.muxihuayi.cn

[J07] 比较两个日期
来源：http://pa.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://uw.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vk.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yu.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cq.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wx.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uo.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dx.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://fl.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://oi.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ax.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tv.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://av.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wy.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://se.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yo.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fl.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wc.521024.cn

[J09] 时区处理
来源：http://ox.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bc.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qd.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ys.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pm.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kq.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hp.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xz.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hy.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://nd.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://in.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xh.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://da.yuexingan06.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ds.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ne.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hb.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nf.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://im.shtwfgs.cn

================================================================================
来源：http://jg.shxzukj.cn

K. JSON 与序列化
来源：http://uz.bjjhwx.cn

================================================================================
来源：http://le.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://gc.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wh.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zq.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://vc.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://as.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sa.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://jl.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vz.lnxyls.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://br.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://vr.hnjuh.cn

Py:   json.loads(s)
来源：http://km.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fm.hahajie.cn

JS:   JSON.parse(s)
来源：http://lq.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://qg.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xn.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://eh.asd995.cn

Ruby: JSON.parse(s)
来源：http://jw.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qk.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://po.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kt.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eh.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://am.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fi.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qy.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pa.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rg.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tv.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://ou.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cc.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zf.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vz.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tc.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vh.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yi.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ka.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pj.bjjhwx.cn

[K05] 深拷贝对象
来源：http://jb.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://io.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://ma.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://ga.newstarts.cn

TS:   structuredClone(obj)
来源：http://dh.szsharing.cn


<!-- 参考信息 -->