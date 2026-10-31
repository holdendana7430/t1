代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://zz.521024.cn

[H04] 自定义异常类型
来源：http://ti.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://wo.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://os.newstarts.cn

JS:   class MyError extends Error {}
来源：http://ms.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://sj.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://dg.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wo.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://gv.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://in.newstarts.cn

[H05] 捕获特定类型
来源：http://da.shxzskj.cn

Py:   except ValueError as e:
来源：http://yq.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jn.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://zo.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://uc.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://fr.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kg.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://bf.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fy.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://yf.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://zs.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bn.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vs.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sz.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gu.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hx.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://cx.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://so.muxihuayi.cn

[H07] 断言
来源：http://jp.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://up.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://nt.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://kr.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://uc.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://fs.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sp.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pd.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://lt.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://nw.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://bz.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iz.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://lm.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cr.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ek.newstarts.cn

Go:   err.Error()
来源：http://sv.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://jl.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://yu.lnxyls.cn

[H09] 带错误码的异常
来源：http://xh.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ff.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://is.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sz.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cs.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qd.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lf.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mr.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qa.521024.cn

[H10] 资源自动释放
来源：http://sc.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://of.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tq.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ok.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zp.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rm.haigaiapp.cn

Go:   defer f.Close()
来源：http://an.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fc.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kv.panjiajie.cn

================================================================================
来源：http://sc.muxihuayi.cn

I. 正则表达式
来源：http://ya.asd995.cn

================================================================================
来源：http://cx.hahajie.cn

[I01] 判断是否匹配
来源：http://if.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://au.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ko.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://rq.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://nm.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xk.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ak.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://px.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xm.yuexingan06.cn

[I02] 提取所有匹配
来源：http://mx.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://pb.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qq.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fg.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://pp.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bm.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mq.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://jk.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://os.muxihuayi.cn

[I03] 提取捕获分组
来源：http://tg.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ft.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wk.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qz.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bo.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jg.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aq.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vw.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mo.huixinmuqiang.cn

[I04] 正则替换
来源：http://oy.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qe.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zf.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gy.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zk.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zd.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ca.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ct.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://af.chemitech.net.cn

[I05] 按正则拆分
来源：http://uu.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cj.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zm.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://lo.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://zh.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://be.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ck.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rs.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sd.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zo.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ge.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yn.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://av.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xx.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eq.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zy.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://me.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://if.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://wl.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ep.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xg.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ex.szsharing.cn

TS:   /error/gim
来源：http://lc.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ey.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uq.shxzskj.cn

Ruby: s.scan(/error/i)
来源：http://ou.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jw.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://ju.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://od.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mj.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nl.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tp.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ws.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zb.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ey.chemitech.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://do.shtwfgs.cn

================================================================================
来源：http://ae.521024.cn

J. 日期与时间
来源：http://yr.huanxung.cn

================================================================================
来源：http://vt.bjjhwx.cn

[J01] 获取当前时间
来源：http://xj.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bp.jctech888.com.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mu.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://by.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://bp.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kz.jctech888.com.cn

Go:   time.Now()
来源：http://nt.521024.cn

Ruby: Time.now
来源：http://wt.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vt.gzmigu.cn

[J02] 格式化输出
来源：http://fu.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gk.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ol.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pz.lnxyls.cn

TS:   d.toISOString()
来源：http://il.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://au.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qh.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ce.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cs.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://uq.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fu.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://su.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://jt.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://yf.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bf.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pw.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://aj.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bz.asd995.cn

[J04] 时间戳与日期互转
来源：http://rn.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ds.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xf.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gt.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pf.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lp.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ma.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cy.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ww.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://qo.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://dn.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ym.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xv.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yo.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://oy.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://of.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://ub.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://re.chemitech.net.cn

[J06] 计算两时间之差
来源：http://wp.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://ly.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://ze.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ph.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cz.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fd.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://sg.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://ik.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://qc.newstarts.cn

[J07] 比较两个日期
来源：http://gy.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://pm.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ge.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://os.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://du.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://km.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://se.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hr.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://ag.hahajie.cn

[J08] 提取年月日与星期
来源：http://fz.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ux.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mi.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ln.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://va.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vg.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vf.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zv.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://my.huixiangedu.cn

[J09] 时区处理
来源：http://an.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qq.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dm.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fa.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://na.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://po.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ri.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://re.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://og.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://ye.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ie.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qq.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qc.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rz.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rh.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mg.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sb.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lr.huixinmuqiang.cn

================================================================================
来源：http://pa.panjiajie.cn

K. JSON 与序列化
来源：http://nb.szsharing.cn

================================================================================
来源：http://wu.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://gm.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kg.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ui.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://mh.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://sg.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jr.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://ud.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nc.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://om.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://ya.nszjky.cn

Py:   json.loads(s)
来源：http://bv.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bh.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://ap.colortex.cn

TS:   JSON.parse(s)
来源：http://ru.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zc.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://ev.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://ji.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rp.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://zj.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oo.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qm.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://we.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dg.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cy.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zy.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qi.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ar.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://at.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://za.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rw.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gf.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tp.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tm.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://co.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nm.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hs.gzmigu.cn

[K05] 深拷贝对象
来源：http://pk.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://ha.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://oi.lnxyls.cn

JS:   structuredClone(obj)
来源：http://fg.szsharing.cn

TS:   structuredClone(obj)
来源：http://wh.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pl.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ua.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zn.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xv.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://dx.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qm.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nb.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ly.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wu.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qv.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vp.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ol.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tx.jianghongdianzi.cn

[K07] 进制转换
来源：http://ug.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://io.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nz.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xd.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wt.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sm.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gi.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zx.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bl.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://ua.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://ed.bookmarksfly.cn


<!-- 参考信息 -->