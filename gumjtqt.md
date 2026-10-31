代发 wailian999

TS:   throw new Error("错误信息");
来源：http://ao.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ed.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://le.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uq.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tl.bjjhwx.cn

[H04] 自定义异常类型
来源：http://rb.bjjhwx.cn

Py:   class MyError(Exception): pass
来源：http://vz.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://da.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://lq.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://ou.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://gi.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mx.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://bq.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://ax.hnjuh.cn

[H05] 捕获特定类型
来源：http://ma.newstarts.cn

Py:   except ValueError as e:
来源：http://dc.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zv.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://bh.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://ig.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://hc.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zt.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://hd.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ol.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://am.nicolike.cn

Py:   value = d.get("k") or default
来源：http://hd.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dg.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qw.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wq.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ik.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ui.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://ju.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://me.newstarts.cn

[H07] 断言
来源：http://no.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://vi.gzmigu.cn

PHP:  assert($x > 0);
来源：http://pt.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://ab.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://tx.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://bi.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ir.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pw.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://hx.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://at.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://gg.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zu.newstarts.cn

JS:   e.message;  e.stack
来源：http://rl.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bh.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bx.haigaiapp.cn

Go:   err.Error()
来源：http://tk.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://mr.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://cm.bjjhwx.cn

[H09] 带错误码的异常
来源：http://ms.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ny.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://km.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zd.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tz.szsharing.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eg.asd995.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fa.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ez.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zo.gzmigu.cn

[H10] 资源自动释放
来源：http://zq.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ci.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wk.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zr.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sy.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ha.bjjhwx.cn

Go:   defer f.Close()
来源：http://vc.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ve.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://di.shtwfgs.cn

================================================================================
来源：http://dw.hnjuh.cn

I. 正则表达式
来源：http://ho.shxzukj.cn

================================================================================
来源：http://rs.newstarts.cn

[I01] 判断是否匹配
来源：http://qw.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mt.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wx.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://gd.nicolike.cn

TS:   /\d+/.test(s)
来源：http://hk.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dh.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pg.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://lr.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bx.newstarts.cn

[I02] 提取所有匹配
来源：http://yo.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://pc.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://om.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://we.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://zi.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mz.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ns.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://jr.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wz.chemitech.net.cn

[I03] 提取捕获分组
来源：http://wt.hnjuh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ux.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qn.nszjky.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gp.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ca.wgjwhj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ln.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://et.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ow.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ky.jctech888.com.cn

[I04] 正则替换
来源：http://oq.szxytkj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kl.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ww.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hk.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ym.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ux.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vg.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yo.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qw.panjiajie.cn

[I05] 按正则拆分
来源：http://qi.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sm.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qj.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://ih.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ub.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://dj.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qg.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dr.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jg.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eq.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zn.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wf.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dm.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://my.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ni.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wo.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xh.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nh.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://ra.szxytkj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://st.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pk.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lh.huixiangedu.cn

TS:   /error/gim
来源：http://gc.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vy.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gz.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://vd.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oa.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://gz.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sj.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ui.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gx.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ea.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mt.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hb.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gx.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bl.jianghongdianzi.cn

================================================================================
来源：http://dd.shxzskj.cn

J. 日期与时间
来源：http://dq.bjjhwx.cn

================================================================================
来源：http://wd.nicolike.cn

[J01] 获取当前时间
来源：http://qx.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bz.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wv.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://gi.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://ck.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qm.hnjuh.cn

Go:   time.Now()
来源：http://iv.muxihuayi.cn

Ruby: Time.now
来源：http://jh.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pa.hnjuh.cn

[J02] 格式化输出
来源：http://fq.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lc.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ab.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dg.9csxet.cn

TS:   d.toISOString()
来源：http://kp.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vn.newstarts.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://we.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qg.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ui.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://ij.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qn.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zw.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://kf.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://rt.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wc.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hw.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://tf.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ho.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://dl.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fr.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kt.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mx.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cc.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ky.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ft.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sa.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xo.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://dj.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://pe.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ii.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pk.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pz.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://la.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qy.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://am.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://iv.shxzskj.cn

[J06] 计算两时间之差
来源：http://bt.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://vd.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://bt.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ws.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ym.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://um.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://ma.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://ok.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://xl.asd995.cn

[J07] 比较两个日期
来源：http://md.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://gf.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ud.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gp.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nb.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zs.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gm.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://op.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://kh.huixiangedu.cn

[J08] 提取年月日与星期
来源：http://oc.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sm.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nf.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ox.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ts.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nb.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ph.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cc.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ll.gzmigu.cn

[J09] 时区处理
来源：http://hl.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mb.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xi.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wf.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cs.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jy.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wd.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rh.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vu.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://pj.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gh.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qy.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cn.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zf.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rk.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qh.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pn.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nt.bjjhwx.cn

================================================================================
来源：http://hn.gzmigu.cn

K. JSON 与序列化
来源：http://of.wgjwhj.cn

================================================================================
来源：http://kr.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://ka.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hu.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uo.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://rs.521024.cn

TS:   JSON.stringify(obj)
来源：http://hs.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sx.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://eg.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fk.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kx.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://mh.hnjuh.cn

Py:   json.loads(s)
来源：http://ol.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ta.newstarts.cn

JS:   JSON.parse(s)
来源：http://en.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://pn.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oa.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://bo.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://zs.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ak.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://jq.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zm.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kf.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uh.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://va.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cy.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nl.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bg.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://de.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://hl.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uo.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tb.szxytkj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sp.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bk.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://si.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ha.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uq.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dd.huixiangedu.cn

[K05] 深拷贝对象
来源：http://hh.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://hm.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://wu.hnjuh.cn

JS:   structuredClone(obj)
来源：http://em.szsharing.cn

TS:   structuredClone(obj)
来源：http://nv.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ss.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lc.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xa.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pg.newstarts.cn

[K06] 解析 URL 查询串
来源：http://ch.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ky.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ub.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bo.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hw.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://my.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fs.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gm.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ww.shtwfgs.cn

[K07] 进制转换
来源：http://qx.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qr.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://co.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yv.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wo.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oz.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hh.szsharing.cn


<!-- 参考信息 -->