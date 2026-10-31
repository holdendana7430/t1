代发 wailian999

[H03] 主动抛出异常
来源：http://rn.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://gw.nszjky.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nb.521024.cn

JS:   throw new Error("错误信息");
来源：http://ti.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://dk.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vo.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zg.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cc.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ov.nszjky.cn

[H04] 自定义异常类型
来源：http://tw.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://zm.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bq.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://id.szsharing.cn

TS:   class MyError extends Error {}
来源：http://sj.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://jh.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zj.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://ig.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://qu.huanxung.cn

[H05] 捕获特定类型
来源：http://iq.wgjwhj.cn

Py:   except ValueError as e:
来源：http://gk.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cs.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://sz.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://fm.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://tu.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jg.yuexingan06.cn

Ruby: rescue ArgumentError => e
来源：http://go.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gm.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://ct.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://ql.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ld.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ve.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dd.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ny.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ib.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://ze.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://br.jctech888.com.cn

[H07] 断言
来源：http://fu.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://jf.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://es.hahajie.cn

JS:   console.assert(x > 0);
来源：http://en.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://bx.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://ls.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://as.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sq.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://rf.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://yg.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://ni.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vz.szsharing.cn

JS:   e.message;  e.stack
来源：http://rl.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qr.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ex.shxzskj.cn

Go:   err.Error()
来源：http://ui.nicolike.cn

Ruby: e.message;  e.backtrace
来源：http://yl.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://uf.nszjky.cn

[H09] 带错误码的异常
来源：http://hd.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fd.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rx.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://js.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ho.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://up.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hs.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wn.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xd.hahajie.cn

[H10] 资源自动释放
来源：http://qr.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xi.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oi.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kp.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cn.shxzskj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yi.shtwfgs.cn

Go:   defer f.Close()
来源：http://lo.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ml.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ke.panjiajie.cn

================================================================================
来源：http://dp.muxihuayi.cn

I. 正则表达式
来源：http://ol.huixiangedu.cn

================================================================================
来源：http://ap.521024.cn

[I01] 判断是否匹配
来源：http://gf.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bj.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mv.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://dy.colortex.cn

TS:   /\d+/.test(s)
来源：http://mj.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wk.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rs.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://ky.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ss.szxytkj.cn

[I02] 提取所有匹配
来源：http://pe.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://jb.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rb.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uq.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://ix.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ft.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cc.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://bd.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ig.szsharing.cn

[I03] 提取捕获分组
来源：http://gc.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lp.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ax.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lb.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xr.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zm.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rv.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sk.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kf.shxzskj.cn

[I04] 正则替换
来源：http://pf.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dk.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sw.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hw.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nr.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://co.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rg.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dw.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ws.muxihuayi.cn

[I05] 按正则拆分
来源：http://tv.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jw.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://no.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://lx.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://tl.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://aa.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yt.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cy.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oc.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fw.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iz.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vr.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cc.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oa.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dw.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dz.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ba.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cm.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://lw.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lm.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dl.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gy.9csxet.cn

TS:   /error/gim
来源：http://ag.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pv.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://da.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://ty.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rh.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://ij.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cq.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://so.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mc.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fh.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://go.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hq.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://od.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mc.asd995.cn

================================================================================
来源：http://gl.panjiajie.cn

J. 日期与时间
来源：http://fn.yuntaijiaju.cn

================================================================================
来源：http://ar.szxytkj.cn

[J01] 获取当前时间
来源：http://tw.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vb.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ds.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://qp.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://gt.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tf.shtwfgs.cn

Go:   time.Now()
来源：http://pe.asd995.cn

Ruby: Time.now
来源：http://ip.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://re.huixinmuqiang.cn

[J02] 格式化输出
来源：http://au.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tg.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hp.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pz.newstarts.cn

TS:   d.toISOString()
来源：http://fa.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iu.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://so.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aq.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://se.9csxet.cn

[J03] 字符串解析为日期
来源：http://hb.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zq.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hv.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://uy.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://ck.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://oz.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eh.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://er.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dc.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://zt.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gy.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ao.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wr.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zb.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ov.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ao.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fc.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fu.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://nx.asd995.cn

Py:   now + timedelta(days=7)
来源：http://yx.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pj.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xq.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xk.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ly.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gq.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://rp.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mm.yuexingan06.cn

[J06] 计算两时间之差
来源：http://pi.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://ix.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://mf.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yb.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qs.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iu.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://ff.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://nx.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://sr.szsharing.cn

[J07] 比较两个日期
来源：http://nn.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://xx.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yz.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://as.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gl.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qf.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fh.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://ni.huanxung.cn

[J08] 提取年月日与星期
来源：http://jc.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qw.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mg.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ld.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tp.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mq.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ce.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gu.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cs.jctech888.com.cn

[J09] 时区处理
来源：http://hs.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ne.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lo.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ep.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pr.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rr.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ev.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zq.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://np.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://sm.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fl.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bd.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ha.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hp.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sw.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uv.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sb.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ru.asd995.cn

================================================================================
来源：http://fw.bookmarksfly.cn

K. JSON 与序列化
来源：http://xv.jctech888.com.cn

================================================================================
来源：http://xi.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://pa.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jw.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pw.colortex.cn

JS:   JSON.stringify(obj)
来源：http://yv.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://ln.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cp.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://pw.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://li.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://og.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://pc.gzmigu.cn

Py:   json.loads(s)
来源：http://fc.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://if.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://hg.gzmigu.cn

TS:   JSON.parse(s)
来源：http://ar.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://as.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://oe.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://ug.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xx.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://ih.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ar.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bv.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jt.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qq.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rl.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ae.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://eb.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tm.newstarts.cn

[K04] 读取 JSON 文件
来源：http://av.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hk.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yv.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eo.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ne.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hb.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qj.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gw.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xb.lnxyls.cn

[K05] 深拷贝对象
来源：http://ha.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://mw.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://fz.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://pq.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://wq.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mm.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rf.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ea.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://we.colortex.cn

[K06] 解析 URL 查询串
来源：http://xs.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dz.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vj.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ax.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://my.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://am.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://uc.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yi.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ib.szsharing.cn

[K07] 进制转换
来源：http://nh.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jm.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dh.jianghongdianzi.cn


<!-- 参考信息 -->