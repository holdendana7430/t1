代发 wailian999

H. 异常与错误处理
来源：http://fl.nszjky.cn

================================================================================
来源：http://kz.hnjuh.cn

[H01] try / catch 基础
来源：http://qo.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wd.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pv.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://at.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rg.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ze.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ty.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://af.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ia.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://bx.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ic.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lc.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vf.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nx.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://es.bookmarksfly.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fh.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ld.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://if.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://gv.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://id.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nd.haigaiapp.cn

JS:   throw new Error("错误信息");
来源：http://lh.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://br.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jx.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://km.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bp.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ko.newstarts.cn

[H04] 自定义异常类型
来源：http://vd.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://ub.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bt.szsharing.cn

JS:   class MyError extends Error {}
来源：http://vi.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://ad.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://hc.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://so.shxzskj.cn

Ruby: class MyError < StandardError; end
来源：http://hw.newstarts.cn

C#:   class MyException : Exception {}
来源：http://dc.szxytkj.cn

[H05] 捕获特定类型
来源：http://in.newstarts.cn

Py:   except ValueError as e:
来源：http://zv.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mh.9csxet.cn

JS:   if (e instanceof TypeError) {}
来源：http://pd.jctech888.com.cn

TS:   if (e instanceof TypeError) {}
来源：http://rf.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://pv.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xz.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://ee.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sn.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://ud.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://pf.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://if.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bl.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xh.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yw.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cd.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://tq.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://zj.szxytkj.cn

[H07] 断言
来源：http://vy.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://ju.lnxyls.cn

PHP:  assert($x > 0);
来源：http://al.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://lo.szsharing.cn

TS:   console.assert(x > 0);
来源：http://ux.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://le.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://id.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uz.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://ci.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://ab.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://pk.shxzskj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pd.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://gn.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vu.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://no.shtwfgs.cn

Go:   err.Error()
来源：http://tr.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://nd.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://bx.szsharing.cn

[H09] 带错误码的异常
来源：http://kk.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aw.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xd.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gt.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qq.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://li.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lf.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://de.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hi.nszjky.cn

[H10] 资源自动释放
来源：http://hu.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tn.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hn.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qf.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://np.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lm.hahajie.cn

Go:   defer f.Close()
来源：http://ai.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ey.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rl.huixinmuqiang.cn

================================================================================
来源：http://wd.shxzukj.cn

I. 正则表达式
来源：http://go.521024.cn

================================================================================
来源：http://xu.asd995.cn

[I01] 判断是否匹配
来源：http://ru.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qs.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rt.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://sk.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://tm.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xp.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xa.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://ua.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://so.hahajie.cn

[I02] 提取所有匹配
来源：http://jm.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://ip.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rm.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hq.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://rd.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bz.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ia.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://ex.bjjhwx.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ea.wgjwhj.cn

[I03] 提取捕获分组
来源：http://ts.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nb.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ch.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pr.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dh.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lm.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vf.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://so.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ck.huixiangedu.cn

[I04] 正则替换
来源：http://nl.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nd.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://co.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mn.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oi.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://db.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hg.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yu.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fi.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://as.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rb.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://io.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://li.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://vl.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://pn.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ua.nicolike.cn

Ruby: s.split(/\s*,\s*/)
来源：http://he.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gj.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fa.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lr.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tr.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wq.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jd.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sr.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ao.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fh.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dm.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://ij.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dp.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cs.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kr.colortex.cn

TS:   /error/gim
来源：http://sy.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lr.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lz.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://jn.szsharing.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lg.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://to.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fs.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kk.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sc.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qg.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sj.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kz.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gp.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dx.nicolike.cn

================================================================================
来源：http://ns.haigaiapp.cn

J. 日期与时间
来源：http://eu.haigaiapp.cn

================================================================================
来源：http://qq.shxzukj.cn

[J01] 获取当前时间
来源：http://yr.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tg.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://of.521024.cn

JS:   new Date();  Date.now()
来源：http://ra.9csxet.cn

TS:   new Date();  Date.now()
来源：http://df.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pb.gzmigu.cn

Go:   time.Now()
来源：http://qs.lnxyls.cn

Ruby: Time.now
来源：http://pu.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bk.lnxyls.cn

[J02] 格式化输出
来源：http://qj.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ao.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yv.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qn.hahajie.cn

TS:   d.toISOString()
来源：http://ke.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://te.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fi.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dt.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://el.nicolike.cn

[J03] 字符串解析为日期
来源：http://gd.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gz.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ta.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://ep.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://fw.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rm.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oe.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ed.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tm.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://tj.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hc.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ib.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://me.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xi.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wa.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kg.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mn.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://np.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://gc.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://vv.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rv.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uh.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cx.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://qa.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ek.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://tm.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mt.panjiajie.cn

[J06] 计算两时间之差
来源：http://qg.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://yl.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://uv.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xj.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ad.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pk.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://gx.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://vu.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://pv.shxzskj.cn

[J07] 比较两个日期
来源：http://np.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://fm.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://my.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lh.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tr.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yx.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cb.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://of.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://zx.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://hf.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nh.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nu.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vc.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qw.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hc.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ay.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://as.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iu.lnxyls.cn

[J09] 时区处理
来源：http://ws.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pm.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sx.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pb.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kv.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qu.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wa.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gh.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xz.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://ye.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dn.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gq.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jt.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ud.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zh.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dl.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pb.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fs.nicolike.cn

================================================================================
来源：http://re.szsharing.cn

K. JSON 与序列化
来源：http://yi.jianghongdianzi.cn

================================================================================
来源：http://ex.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://df.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kq.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vb.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://xz.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://om.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vf.colortex.cn

Go:   json.Marshal(obj)
来源：http://nk.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zn.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uf.9csxet.cn

[K02] JSON 字符串转对象
来源：http://ov.wgjwhj.cn

Py:   json.loads(s)
来源：http://oi.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pt.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://hg.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://wq.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://de.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://ue.szsharing.cn

Ruby: JSON.parse(s)
来源：http://vz.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zy.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://dc.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://te.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ot.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://aw.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://km.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ua.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nl.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://da.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vg.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://un.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qw.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mh.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kb.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hd.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://le.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mc.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ra.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mr.yuexingan06.cn

[K05] 深拷贝对象
来源：http://vd.bjjhwx.cn


<!-- 参考信息 -->