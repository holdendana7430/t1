代发 wailian999

H. 异常与错误处理
来源：http://pv.shtwfgs.cn

================================================================================
来源：http://rx.muxihuayi.cn

[H01] try / catch 基础
来源：http://bs.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fg.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jx.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jo.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cj.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ro.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fu.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zx.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ep.huanxung.cn

[H02] finally / ensure 收尾
来源：http://oj.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jr.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uz.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tt.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ff.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wh.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sr.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sd.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ss.yuexingan06.cn

[H03] 主动抛出异常
来源：http://pc.huanxung.cn

Py:   raise ValueError("错误信息")
来源：http://tb.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bc.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://uo.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://wh.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ks.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://au.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://li.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ve.asd995.cn

[H04] 自定义异常类型
来源：http://xw.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://du.shtwfgs.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qv.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://ib.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://oj.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://dq.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dx.521024.cn

Ruby: class MyError < StandardError; end
来源：http://sv.521024.cn

C#:   class MyException : Exception {}
来源：http://yp.shxzukj.cn

[H05] 捕获特定类型
来源：http://ce.nszjky.cn

Py:   except ValueError as e:
来源：http://ka.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pw.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://pi.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://mq.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://us.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://es.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://wi.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vu.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://uv.szsharing.cn

Py:   value = d.get("k") or default
来源：http://vz.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bc.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jt.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dg.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://km.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gc.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://nw.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://yw.jianghongdianzi.cn

[H07] 断言
来源：http://du.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://kx.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://ll.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://kv.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://tz.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://ko.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dl.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wf.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://hp.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://ds.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://yx.chemitech.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wy.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://pk.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nr.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hd.haigaiapp.cn

Go:   err.Error()
来源：http://ar.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://it.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://hw.nszjky.cn

[H09] 带错误码的异常
来源：http://uz.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dq.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://un.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cz.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qx.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zv.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://np.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://go.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://un.colortex.cn

[H10] 资源自动释放
来源：http://is.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ao.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ma.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kd.hnjuh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xh.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pb.9csxet.cn

Go:   defer f.Close()
来源：http://er.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rg.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rq.asd995.cn

================================================================================
来源：http://kv.colortex.cn

I. 正则表达式
来源：http://ty.huixinmuqiang.cn

================================================================================
来源：http://qb.colortex.cn

[I01] 判断是否匹配
来源：http://oh.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ux.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cn.hahajie.cn

JS:   /\d+/.test(s)
来源：http://gn.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://gf.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gz.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ii.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://zo.9csxet.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lx.gzmigu.cn

[I02] 提取所有匹配
来源：http://og.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://nh.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nz.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zd.521024.cn

TS:   s.match(/\d+/g)
来源：http://tr.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jd.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yg.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://ef.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gx.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://ke.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lm.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://po.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rv.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://im.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eo.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fg.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pl.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rm.bookmarksfly.cn

[I04] 正则替换
来源：http://kx.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mt.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vt.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://oy.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zs.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gm.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dd.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://px.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qa.hnjuh.cn

[I05] 按正则拆分
来源：http://xb.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zx.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jw.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://bs.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://dc.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://ye.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wn.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://eh.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ks.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yi.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wa.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bv.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hh.521024.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ty.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wd.hahajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://on.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xc.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ix.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://rh.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tf.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://no.bookmarksfly.cn

TS:   /error/gim
来源：http://rr.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ld.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gg.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://ix.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ir.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://nx.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mx.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rl.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uf.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gc.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gl.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cc.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vn.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gj.nicolike.cn

================================================================================
来源：http://fd.gzmigu.cn

J. 日期与时间
来源：http://rm.huanxung.cn

================================================================================
来源：http://gl.shxzukj.cn

[J01] 获取当前时间
来源：http://do.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ul.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cx.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://yx.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://aa.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zf.muxihuayi.cn

Go:   time.Now()
来源：http://av.gzmigu.cn

Ruby: Time.now
来源：http://ud.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://if.gzmigu.cn

[J02] 格式化输出
来源：http://vk.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pj.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rm.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rd.haigaiapp.cn

TS:   d.toISOString()
来源：http://hl.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eh.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sy.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eg.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yq.colortex.cn

[J03] 字符串解析为日期
来源：http://zk.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://we.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://js.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://ut.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://tc.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xr.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hi.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://gb.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ta.colortex.cn

[J04] 时间戳与日期互转
来源：http://fd.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xh.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ti.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qt.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rv.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ee.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dl.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ct.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ix.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://xn.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://sd.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ho.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oz.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dt.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://si.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ug.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://nt.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ei.gzmigu.cn

[J06] 计算两时间之差
来源：http://zs.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://al.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://jr.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://db.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://my.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://do.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://vc.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://yx.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://go.lnxyls.cn

[J07] 比较两个日期
来源：http://hi.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://us.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xo.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ja.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lf.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ud.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lz.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rx.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://qn.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://wp.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xy.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mu.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ts.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sp.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://of.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ru.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nu.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fd.chemitech.net.cn

[J09] 时区处理
来源：http://cb.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sb.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qr.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fk.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pv.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kf.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pm.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ft.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pp.521024.cn

[J10] 取今天 / 本月第一天
来源：http://ru.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://un.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rs.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gm.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xf.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://im.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iu.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ez.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nc.9csxet.cn

================================================================================
来源：http://nh.colortex.cn

K. JSON 与序列化
来源：http://wv.yuntaijiaju.cn

================================================================================
来源：http://fq.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://xf.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oa.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ky.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://nq.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://zg.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zo.szsharing.cn

Go:   json.Marshal(obj)
来源：http://ay.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://br.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yh.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://tl.bjjhwx.cn

Py:   json.loads(s)
来源：http://we.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ie.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://si.newstarts.cn

TS:   JSON.parse(s)
来源：http://uh.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bi.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://fg.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://en.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gh.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://km.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iz.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vx.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://of.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://td.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ca.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qf.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ln.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tj.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://as.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vz.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wg.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ya.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uc.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ik.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lz.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sz.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wv.shxzukj.cn

[K05] 深拷贝对象
来源：http://uw.9csxet.cn


<!-- 参考信息 -->