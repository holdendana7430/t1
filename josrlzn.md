代发 wailian999

TS:   throw new Error("错误信息");
来源：http://ab.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nr.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dw.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ev.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jl.huixiangedu.cn

[H04] 自定义异常类型
来源：http://ou.asd995.cn

Py:   class MyError(Exception): pass
来源：http://mt.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tb.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://qb.huanxung.cn

TS:   class MyError extends Error {}
来源：http://df.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://fw.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://me.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://ws.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://mt.chemitech.net.cn

[H05] 捕获特定类型
来源：http://wn.asd995.cn

Py:   except ValueError as e:
来源：http://hg.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bb.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://lf.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://gt.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://vd.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nn.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://xu.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jc.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://ps.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://gu.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pf.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qy.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jp.lnxyls.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uy.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jo.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://um.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://tq.lnxyls.cn

[H07] 断言
来源：http://hc.hahajie.cn

Py:   assert x > 0, "必须为正"
来源：http://ki.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://sc.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://yl.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://jl.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://ms.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vh.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rd.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://yy.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://jl.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://pj.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yg.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://hl.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ax.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uw.lnxyls.cn

Go:   err.Error()
来源：http://et.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://zt.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://uw.lnxyls.cn

[H09] 带错误码的异常
来源：http://rm.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eu.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rt.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ov.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bj.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kd.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qe.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yx.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://aq.newstarts.cn

[H10] 资源自动释放
来源：http://bj.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xq.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cs.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qm.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uc.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hs.nicolike.cn

Go:   defer f.Close()
来源：http://fu.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fj.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uu.lnxyls.cn

================================================================================
来源：http://ig.szsharing.cn

I. 正则表达式
来源：http://oc.9csxet.cn

================================================================================
来源：http://wf.chemitech.net.cn

[I01] 判断是否匹配
来源：http://xq.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dh.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wk.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://wr.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://ks.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lh.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wq.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://ag.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ou.nszjky.cn

[I02] 提取所有匹配
来源：http://hf.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://jh.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zh.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bn.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://va.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ta.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pf.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://me.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fb.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://xd.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://if.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ft.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kq.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ri.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ak.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ru.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iy.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ht.colortex.cn

[I04] 正则替换
来源：http://xh.gzmigu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gr.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tx.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://on.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rw.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jq.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fd.nicolike.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://aw.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yw.muxihuayi.cn

[I05] 按正则拆分
来源：http://vq.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dw.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vx.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://zz.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://nv.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://fm.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bk.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://se.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pk.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ry.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lg.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oj.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mm.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ki.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ea.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uc.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://px.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gt.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://kd.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xg.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qc.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ji.shxzukj.cn

TS:   /error/gim
来源：http://po.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sj.gzmigu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gt.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://ye.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vj.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://bn.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sq.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ww.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yv.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hc.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xp.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qw.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iz.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ml.huixinmuqiang.cn

================================================================================
来源：http://pt.colortex.cn

J. 日期与时间
来源：http://ct.panjiajie.cn

================================================================================
来源：http://ws.panjiajie.cn

[J01] 获取当前时间
来源：http://xf.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ll.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ph.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://vz.newstarts.cn

TS:   new Date();  Date.now()
来源：http://sv.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ca.huixiangedu.cn

Go:   time.Now()
来源：http://re.huanxung.cn

Ruby: Time.now
来源：http://jq.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vz.jianghongdianzi.cn

[J02] 格式化输出
来源：http://lc.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://st.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pz.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ye.newstarts.cn

TS:   d.toISOString()
来源：http://aq.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vf.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dr.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mw.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://by.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://kh.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bc.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yg.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://ns.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://ax.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fa.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sa.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://rx.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ln.9csxet.cn

[J04] 时间戳与日期互转
来源：http://zm.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qg.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ij.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xw.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ww.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gu.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://np.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nv.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sd.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://on.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://pk.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://oh.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xd.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kl.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://wn.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mm.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://ip.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mh.nicolike.cn

[J06] 计算两时间之差
来源：http://il.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://ih.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://ka.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dq.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hf.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://le.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://mi.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://jw.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://kd.521024.cn

[J07] 比较两个日期
来源：http://xw.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://ba.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lc.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ei.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mr.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://os.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zc.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://iz.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://wq.shxzskj.cn

[J08] 提取年月日与星期
来源：http://ul.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nv.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zy.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nf.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fh.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fm.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pd.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aj.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hq.szxytkj.cn

[J09] 时区处理
来源：http://uk.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fb.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sd.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dh.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zq.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lr.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bx.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sy.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://py.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://jp.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xe.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://of.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://el.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kg.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zn.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ew.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pv.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vp.huixinmuqiang.cn

================================================================================
来源：http://bu.colortex.cn

K. JSON 与序列化
来源：http://gz.wgjwhj.cn

================================================================================
来源：http://cc.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://xo.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hh.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sj.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://bo.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://wh.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ma.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://ac.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qk.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://er.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://xd.szxytkj.cn

Py:   json.loads(s)
来源：http://lt.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ue.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://ug.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://ye.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ze.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://dk.newstarts.cn

Ruby: JSON.parse(s)
来源：http://sw.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rf.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://aq.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rf.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jr.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mf.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ta.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gb.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jg.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ff.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zn.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://yv.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yx.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ku.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hc.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qe.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aw.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qv.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yy.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dp.huixiangedu.cn

[K05] 深拷贝对象
来源：http://xh.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://en.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://rr.nszjky.cn

JS:   structuredClone(obj)
来源：http://og.huanxung.cn

TS:   structuredClone(obj)
来源：http://la.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ge.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ep.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fw.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pm.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://pg.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hf.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mj.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jo.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bx.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wm.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qx.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ne.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rt.gzmigu.cn

[K07] 进制转换
来源：http://jt.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lg.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vv.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aw.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ue.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ms.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ue.nszjky.cn


<!-- 参考信息 -->