代发 wailian999

TS:   throw new Error("错误信息");
来源：http://ai.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://av.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jv.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zu.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ie.gzmigu.cn

[H04] 自定义异常类型
来源：http://xs.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://tp.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uw.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://xt.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://gx.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://xe.shtwfgs.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fk.shxzskj.cn

Ruby: class MyError < StandardError; end
来源：http://rf.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://xt.panjiajie.cn

[H05] 捕获特定类型
来源：http://jj.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://dw.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ly.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://ay.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://sn.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://zk.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tt.9csxet.cn

Ruby: rescue ArgumentError => e
来源：http://dn.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xk.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://dg.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://qk.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pc.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hd.9csxet.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jf.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://as.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tl.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://gl.521024.cn

C#:   obj?.A?.B ?? default
来源：http://qn.nicolike.cn

[H07] 断言
来源：http://nx.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://aw.huanxung.cn

PHP:  assert($x > 0);
来源：http://un.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://gz.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://qm.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://pt.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ag.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://js.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://hg.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://ua.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://pu.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gy.huanxung.cn

JS:   e.message;  e.stack
来源：http://jy.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://os.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fk.wgjwhj.cn

Go:   err.Error()
来源：http://ey.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://vr.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://hd.huanxung.cn

[H09] 带错误码的异常
来源：http://cl.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pn.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uc.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mu.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oh.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uk.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fj.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bp.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jb.jctech888.com.cn

[H10] 资源自动释放
来源：http://cq.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wr.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ll.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qq.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uw.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cw.wgjwhj.cn

Go:   defer f.Close()
来源：http://oc.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dk.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://na.9csxet.cn

================================================================================
来源：http://sp.jianghongdianzi.cn

I. 正则表达式
来源：http://xc.shxzukj.cn

================================================================================
来源：http://cy.9csxet.cn

[I01] 判断是否匹配
来源：http://yh.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://en.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ix.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://of.521024.cn

TS:   /\d+/.test(s)
来源：http://ux.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sp.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bn.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://pp.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wd.chemitech.net.cn

[I02] 提取所有匹配
来源：http://eg.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://xf.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aw.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fw.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://oy.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vm.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bn.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://on.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iv.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://yd.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://un.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ef.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ik.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kf.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tm.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xz.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bt.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rt.panjiajie.cn

[I04] 正则替换
来源：http://dt.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tm.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pt.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xt.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bs.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://oc.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ek.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ts.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kx.huixiangedu.cn

[I05] 按正则拆分
来源：http://si.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dq.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sv.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://wq.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://km.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://nl.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qn.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ii.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ci.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pi.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dz.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ar.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bj.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oo.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sp.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qk.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iv.bjjhwx.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wv.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://oh.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yq.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ve.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nx.szsharing.cn

TS:   /error/gim
来源：http://gn.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://of.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hu.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://hz.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://no.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://ty.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vh.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://at.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ln.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nm.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yc.muxihuayi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ek.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qf.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ie.muxihuayi.cn

================================================================================
来源：http://wx.szxytkj.cn

J. 日期与时间
来源：http://tf.szxytkj.cn

================================================================================
来源：http://gk.chemitech.net.cn

[J01] 获取当前时间
来源：http://ca.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ag.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hu.colortex.cn

JS:   new Date();  Date.now()
来源：http://wz.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://wg.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://oq.shtwfgs.cn

Go:   time.Now()
来源：http://sv.yuexingan06.cn

Ruby: Time.now
来源：http://de.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kt.huixiangedu.cn

[J02] 格式化输出
来源：http://dn.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yp.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hr.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jx.yuexingan06.cn

TS:   d.toISOString()
来源：http://dk.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rk.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xz.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rr.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hx.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://ml.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ev.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tu.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://gn.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://ci.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ip.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tg.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://di.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eg.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://zq.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gw.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gh.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uo.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cc.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gr.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zt.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ny.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tf.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://jn.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://cj.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lg.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://se.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ul.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://iw.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uw.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://zl.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hz.muxihuayi.cn

[J06] 计算两时间之差
来源：http://jl.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://bl.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://za.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wb.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vp.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ep.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://yu.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://yv.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://ic.gzmigu.cn

[J07] 比较两个日期
来源：http://us.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://fy.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ws.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jg.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://it.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nh.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sc.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pm.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://jo.panjiajie.cn

[J08] 提取年月日与星期
来源：http://ew.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mi.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kh.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ex.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://by.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sb.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wr.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://il.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://en.yuntaijiaju.cn

[J09] 时区处理
来源：http://bi.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bt.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mr.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://at.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cg.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hs.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://un.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ww.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yj.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://cj.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dn.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mc.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fv.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pu.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vi.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ag.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dc.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wo.yuntaijiaju.cn

================================================================================
来源：http://fq.colortex.cn

K. JSON 与序列化
来源：http://cw.bjjhwx.cn

================================================================================
来源：http://oq.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://er.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mi.gzmigu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yb.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://zr.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://rh.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nk.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://br.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fu.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pc.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://av.szsharing.cn

Py:   json.loads(s)
来源：http://gm.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hq.hahajie.cn

JS:   JSON.parse(s)
来源：http://hu.szxytkj.cn

TS:   JSON.parse(s)
来源：http://br.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wi.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://bj.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://wc.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gn.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://pt.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://br.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fg.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pt.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lz.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uo.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wl.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vq.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dj.nicolike.cn

[K04] 读取 JSON 文件
来源：http://tu.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ly.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oz.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zw.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vp.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jw.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cb.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jd.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kr.huixiangedu.cn

[K05] 深拷贝对象
来源：http://oi.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://aa.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://xn.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://xx.shxzskj.cn

TS:   structuredClone(obj)
来源：http://lr.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wt.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lt.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oc.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jv.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://jt.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xd.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mf.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kj.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vc.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ly.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ya.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jr.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nl.bookmarksfly.cn

[K07] 进制转换
来源：http://ml.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://il.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fj.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vm.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bf.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fi.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sx.gzmigu.cn


<!-- 参考信息 -->