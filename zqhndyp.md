代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ic.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://up.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://us.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hw.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tx.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://up.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jy.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://cx.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ft.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cn.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rl.9csxet.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ts.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qh.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ki.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hm.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yr.asd995.cn

[H03] 主动抛出异常
来源：http://nm.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://zz.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tf.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://pr.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://jr.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gi.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ck.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cv.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yn.gzmigu.cn

[H04] 自定义异常类型
来源：http://hr.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://ix.szsharing.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pr.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://lo.newstarts.cn

TS:   class MyError extends Error {}
来源：http://kv.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://wn.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mb.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://us.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://xz.jctech888.com.cn

[H05] 捕获特定类型
来源：http://lv.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://mo.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mt.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://tm.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://zx.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://vn.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ln.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://cd.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pm.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://rx.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://pd.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xe.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vg.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gq.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sc.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kt.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://sr.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://rb.colortex.cn

[H07] 断言
来源：http://hr.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://tw.hahajie.cn

PHP:  assert($x > 0);
来源：http://os.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://el.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://ld.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://kw.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jl.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nu.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://dc.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://hz.yuexingan06.cn

Py:   str(e);  traceback.format_exc()
来源：http://rk.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lh.panjiajie.cn

JS:   e.message;  e.stack
来源：http://do.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ca.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://av.shtwfgs.cn

Go:   err.Error()
来源：http://ht.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://bu.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://ld.9csxet.cn

[H09] 带错误码的异常
来源：http://de.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pt.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kn.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bb.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ua.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ao.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ry.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fl.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lm.bookmarksfly.cn

[H10] 资源自动释放
来源：http://jr.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wm.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wv.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qu.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tf.gzmigu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gw.chemitech.net.cn

Go:   defer f.Close()
来源：http://kb.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dm.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ms.jctech888.com.cn

================================================================================
来源：http://ib.shtwfgs.cn

I. 正则表达式
来源：http://no.huanxung.cn

================================================================================
来源：http://km.szxytkj.cn

[I01] 判断是否匹配
来源：http://dv.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mu.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jz.nicolike.cn

JS:   /\d+/.test(s)
来源：http://wr.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://zh.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eu.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qa.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://hp.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sg.haigaiapp.cn

[I02] 提取所有匹配
来源：http://pm.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://tv.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sa.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yz.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://df.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mq.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ae.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://iy.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iq.colortex.cn

[I03] 提取捕获分组
来源：http://kh.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xs.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fc.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cc.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ce.yuexingan06.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gz.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nx.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bh.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dt.szsharing.cn

[I04] 正则替换
来源：http://zo.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dh.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xm.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nd.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fb.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pk.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://os.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zo.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ma.asd995.cn

[I05] 按正则拆分
来源：http://on.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ck.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://az.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://hg.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://yy.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://mi.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://az.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nd.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xx.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oc.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jy.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oa.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gk.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jk.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oa.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ye.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vm.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://ew.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qz.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ym.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://em.shxzukj.cn

TS:   /error/gim
来源：http://kh.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ob.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nw.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://ug.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ht.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://tm.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dq.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fd.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dv.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ok.yuntaijiaju.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xs.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hu.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://th.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xu.asd995.cn

================================================================================
来源：http://lb.9csxet.cn

J. 日期与时间
来源：http://fz.asd995.cn

================================================================================
来源：http://cv.lnxyls.cn

[J01] 获取当前时间
来源：http://qz.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wj.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://di.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://jy.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://np.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tq.yuexingan06.cn

Go:   time.Now()
来源：http://sv.huanxung.cn

Ruby: Time.now
来源：http://tv.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ic.szsharing.cn

[J02] 格式化输出
来源：http://gq.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jh.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ta.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aq.yuexingan06.cn

TS:   d.toISOString()
来源：http://aa.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hd.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oa.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hr.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://me.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://nk.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ir.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nf.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://og.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://fq.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fj.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uo.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://jg.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xu.521024.cn

[J04] 时间戳与日期互转
来源：http://mj.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sr.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sj.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bw.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jf.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iy.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://su.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eb.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lu.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://qd.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://mo.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uo.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uq.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://su.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://hb.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fs.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://un.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://do.shtwfgs.cn

[J06] 计算两时间之差
来源：http://or.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://xp.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://vc.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kq.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qt.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yx.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://xt.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://qg.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://qn.521024.cn

[J07] 比较两个日期
来源：http://cv.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://nl.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ry.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://md.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gq.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ha.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ix.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qe.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://iy.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://ir.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qd.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ij.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://px.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://th.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ho.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zp.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fl.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sk.huixiangedu.cn

[J09] 时区处理
来源：http://ml.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tm.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tu.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ct.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ny.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gz.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uq.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://br.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hf.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://sr.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sa.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jg.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sq.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nx.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eq.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sp.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ky.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zf.panjiajie.cn

================================================================================
来源：http://ko.haigaiapp.cn

K. JSON 与序列化
来源：http://dw.bookmarksfly.cn

================================================================================
来源：http://vg.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://vx.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sj.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ib.asd995.cn

JS:   JSON.stringify(obj)
来源：http://tc.asd995.cn

TS:   JSON.stringify(obj)
来源：http://iu.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jg.szsharing.cn

Go:   json.Marshal(obj)
来源：http://zp.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ep.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gi.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://yv.szsharing.cn

Py:   json.loads(s)
来源：http://mk.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hq.hnjuh.cn

JS:   JSON.parse(s)
来源：http://cm.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://yp.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jv.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://cn.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://if.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zw.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://iv.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gy.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pn.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zs.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ey.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zf.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tm.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xx.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ld.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://nt.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mg.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ja.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zh.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lo.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kh.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gl.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qp.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kq.shxzukj.cn

[K05] 深拷贝对象
来源：http://kv.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://aj.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://xt.9csxet.cn

JS:   structuredClone(obj)
来源：http://nf.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://av.shxzukj.cn


<!-- 参考信息 -->