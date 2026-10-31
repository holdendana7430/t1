代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uh.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sg.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://su.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jp.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://va.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rt.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ev.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://vg.hahajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jw.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kq.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mu.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hb.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xs.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yz.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ny.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gm.szsharing.cn

[H03] 主动抛出异常
来源：http://xr.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://ai.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mb.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://rd.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://ti.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ph.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ft.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yb.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ki.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://pz.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://nz.szsharing.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zs.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://re.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://fj.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://sn.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://om.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://ba.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://wt.hahajie.cn

[H05] 捕获特定类型
来源：http://ok.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://bz.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dq.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://hv.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://ne.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://ng.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ud.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://qf.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uv.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://fi.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://gg.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://go.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hx.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://st.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nd.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xj.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://mx.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://tf.huixiangedu.cn

[H07] 断言
来源：http://ey.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://uu.szxytkj.cn

PHP:  assert($x > 0);
来源：http://ui.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://fq.nszjky.cn

TS:   console.assert(x > 0);
来源：http://jr.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://ia.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dw.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lu.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://km.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://eo.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://yk.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yk.asd995.cn

JS:   e.message;  e.stack
来源：http://co.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mu.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qo.chemitech.net.cn

Go:   err.Error()
来源：http://mr.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://gh.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://qs.szxytkj.cn

[H09] 带错误码的异常
来源：http://mt.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fr.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://re.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yw.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vu.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ii.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nn.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gw.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pz.chemitech.net.cn

[H10] 资源自动释放
来源：http://nd.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://et.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zs.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hw.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fp.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wk.shxzskj.cn

Go:   defer f.Close()
来源：http://rl.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kj.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zx.jctech888.com.cn

================================================================================
来源：http://uv.9csxet.cn

I. 正则表达式
来源：http://yf.szsharing.cn

================================================================================
来源：http://qv.szsharing.cn

[I01] 判断是否匹配
来源：http://ww.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zq.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vy.huanxung.cn

JS:   /\d+/.test(s)
来源：http://tk.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://ab.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cd.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://us.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://zf.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sg.shxzukj.cn

[I02] 提取所有匹配
来源：http://zg.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://zg.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sp.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fq.colortex.cn

TS:   s.match(/\d+/g)
来源：http://jd.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ee.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://df.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://tz.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tn.huixiangedu.cn

[I03] 提取捕获分组
来源：http://mw.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qc.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dt.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xu.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wu.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gf.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iz.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ip.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ih.muxihuayi.cn

[I04] 正则替换
来源：http://go.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://px.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hh.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mi.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mk.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fx.huanxung.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ny.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wj.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://it.hnjuh.cn

[I05] 按正则拆分
来源：http://sx.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gg.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fx.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://pz.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://eu.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://bi.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bf.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://by.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mi.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dc.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://px.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://le.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ay.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xf.huanxung.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sp.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://td.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gu.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bm.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://on.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ow.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gw.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jy.asd995.cn

TS:   /error/gim
来源：http://wn.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oi.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hp.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://px.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ni.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://wz.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qw.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yz.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://li.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mn.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pv.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dj.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://if.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ha.szxytkj.cn

================================================================================
来源：http://ij.gzmigu.cn

J. 日期与时间
来源：http://sc.yuexingan06.cn

================================================================================
来源：http://zn.panjiajie.cn

[J01] 获取当前时间
来源：http://zs.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lr.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sa.9csxet.cn

JS:   new Date();  Date.now()
来源：http://ja.521024.cn

TS:   new Date();  Date.now()
来源：http://fg.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://oj.wgjwhj.cn

Go:   time.Now()
来源：http://tz.wgjwhj.cn

Ruby: Time.now
来源：http://zq.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zp.521024.cn

[J02] 格式化输出
来源：http://ze.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fr.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sr.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sy.yuexingan06.cn

TS:   d.toISOString()
来源：http://eu.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://el.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gr.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ls.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qk.521024.cn

[J03] 字符串解析为日期
来源：http://eb.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oc.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gn.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://zs.colortex.cn

TS:   new Date("2024-01-02")
来源：http://md.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pw.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xk.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://zl.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ib.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://kj.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ww.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zz.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sw.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://on.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pu.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://an.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kn.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kg.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://fy.wgjwhj.cn

Py:   now + timedelta(days=7)
来源：http://zt.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tm.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://px.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qi.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://op.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jx.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://ix.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cx.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://ef.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://hb.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://ji.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ne.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kb.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qj.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://eh.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://fa.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://bn.shxzukj.cn

[J07] 比较两个日期
来源：http://pr.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://mk.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cn.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ve.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ik.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rn.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bj.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jx.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://xk.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://ij.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fl.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xu.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gr.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hg.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cl.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sv.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fb.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yk.panjiajie.cn

[J09] 时区处理
来源：http://fs.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ii.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ly.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mt.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pr.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wg.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yg.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pz.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ne.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://ak.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rh.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xc.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nh.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ik.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://je.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fg.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dw.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sm.szsharing.cn

================================================================================
来源：http://jd.yuntaijiaju.cn

K. JSON 与序列化
来源：http://ci.521024.cn

================================================================================
来源：http://yz.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://xo.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yf.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kh.colortex.cn

JS:   JSON.stringify(obj)
来源：http://ie.colortex.cn

TS:   JSON.stringify(obj)
来源：http://hz.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qq.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://sa.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://eo.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xc.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://vx.szsharing.cn

Py:   json.loads(s)
来源：http://aw.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sc.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://mk.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://ku.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ad.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://be.521024.cn

Ruby: JSON.parse(s)
来源：http://di.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gh.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://bn.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://if.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ov.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vl.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://do.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qw.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ed.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nl.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ng.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://db.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ro.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ec.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vp.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://js.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://im.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xm.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ue.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://px.521024.cn

[K05] 深拷贝对象
来源：http://qp.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://ri.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://ac.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://do.lnxyls.cn

TS:   structuredClone(obj)
来源：http://un.yuntaijiaju.cn


<!-- 参考信息 -->