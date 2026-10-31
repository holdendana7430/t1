代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rn.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rp.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xt.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://jz.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ro.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qd.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://an.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://in.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ya.muxihuayi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fc.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://as.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://he.muxihuayi.cn

[H03] 主动抛出异常
来源：http://ko.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://or.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://er.newstarts.cn

JS:   throw new Error("错误信息");
来源：http://er.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://do.yuexingan06.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bz.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xs.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dd.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pd.521024.cn

[H04] 自定义异常类型
来源：http://eh.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://ca.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jo.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://fh.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://pz.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://yi.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rk.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://yy.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://gh.newstarts.cn

[H05] 捕获特定类型
来源：http://dh.yuexingan06.cn

Py:   except ValueError as e:
来源：http://oc.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://es.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://ud.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://vh.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://ew.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ig.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://dh.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ue.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://om.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://lh.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jt.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yv.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mw.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jj.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qj.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://sc.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://qo.yuexingan06.cn

[H07] 断言
来源：http://fs.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://qx.panjiajie.cn

PHP:  assert($x > 0);
来源：http://hb.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://ir.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://wz.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://qj.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wp.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yy.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://yr.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://ee.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://vn.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eu.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://na.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vg.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oj.newstarts.cn

Go:   err.Error()
来源：http://ht.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://az.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://ye.panjiajie.cn

[H09] 带错误码的异常
来源：http://cd.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rl.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://py.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jz.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hx.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gd.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nq.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://aq.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hg.shtwfgs.cn

[H10] 资源自动释放
来源：http://xz.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lr.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ov.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yr.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tl.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ix.colortex.cn

Go:   defer f.Close()
来源：http://nl.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kc.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hd.panjiajie.cn

================================================================================
来源：http://da.shtwfgs.cn

I. 正则表达式
来源：http://ye.gzmigu.cn

================================================================================
来源：http://ox.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://um.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dq.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pw.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://tv.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://jz.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gd.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iz.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://po.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sv.hahajie.cn

[I02] 提取所有匹配
来源：http://vo.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://us.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bm.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mf.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://yn.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bk.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ie.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://yc.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kc.hahajie.cn

[I03] 提取捕获分组
来源：http://ad.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xh.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://au.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ml.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kl.yuexingan06.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sh.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kb.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qu.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://la.jctech888.com.cn

[I04] 正则替换
来源：http://sj.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xi.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hh.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yv.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rw.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yj.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kr.nicolike.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hc.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tb.panjiajie.cn

[I05] 按正则拆分
来源：http://jy.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tg.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ww.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://fz.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://py.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://is.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mu.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ew.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ez.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gh.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vr.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yq.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wo.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vx.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ad.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rd.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fh.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tf.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://gx.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wa.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fa.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sv.hahajie.cn

TS:   /error/gim
来源：http://fo.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rz.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://el.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://yk.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pv.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://nr.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rq.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ix.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fn.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kx.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://of.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ej.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cc.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xv.hahajie.cn

================================================================================
来源：http://on.szxytkj.cn

J. 日期与时间
来源：http://ow.shxzukj.cn

================================================================================
来源：http://kv.haigaiapp.cn

[J01] 获取当前时间
来源：http://it.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zk.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nx.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://ce.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://bl.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cg.shxzskj.cn

Go:   time.Now()
来源：http://kw.lnxyls.cn

Ruby: Time.now
来源：http://di.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ri.yuntaijiaju.cn

[J02] 格式化输出
来源：http://ih.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cx.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qw.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vp.nicolike.cn

TS:   d.toISOString()
来源：http://ia.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dj.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gz.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tt.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yw.panjiajie.cn

[J03] 字符串解析为日期
来源：http://qg.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bt.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rd.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://ki.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://ig.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wk.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cy.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://hh.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tg.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://np.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wi.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rg.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zw.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ey.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uj.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lr.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://po.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rb.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://ai.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://nc.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xw.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ab.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kg.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://zf.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ib.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://fz.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nr.newstarts.cn

[J06] 计算两时间之差
来源：http://dw.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://rx.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://bw.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tt.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gn.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ku.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://mi.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://zx.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://nk.bjjhwx.cn

[J07] 比较两个日期
来源：http://xa.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://dg.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cs.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jb.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://av.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hj.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zq.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kh.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://tb.szxytkj.cn

[J08] 提取年月日与星期
来源：http://ub.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qx.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xj.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wf.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qv.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hu.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ha.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tt.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ix.yuntaijiaju.cn

[J09] 时区处理
来源：http://gy.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cf.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nf.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gk.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bq.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sz.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://as.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yk.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dg.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://zo.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vk.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oz.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pj.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qe.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yl.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://go.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zn.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hm.lnxyls.cn

================================================================================
来源：http://ve.jianghongdianzi.cn

K. JSON 与序列化
来源：http://lp.szxytkj.cn

================================================================================
来源：http://no.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://wy.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ve.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fh.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://bx.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://nq.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ii.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://pk.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gx.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ja.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://nc.szsharing.cn

Py:   json.loads(s)
来源：http://it.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bz.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://tv.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://tj.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nn.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://rc.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://hr.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xf.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://hg.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://li.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ns.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ea.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://re.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hk.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qk.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rh.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rn.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://tu.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sz.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://st.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dh.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mj.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qb.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jd.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yc.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://az.nicolike.cn

[K05] 深拷贝对象
来源：http://mm.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://ro.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://ko.nicolike.cn

JS:   structuredClone(obj)
来源：http://ch.521024.cn

TS:   structuredClone(obj)
来源：http://sw.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ao.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mg.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mu.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cw.nszjky.cn


<!-- 参考信息 -->