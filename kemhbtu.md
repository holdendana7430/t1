代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://lk.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://bs.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://hr.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://of.huanxung.cn

JS:   class MyError extends Error {}
来源：http://bm.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://wb.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://lg.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fd.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://bp.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://eq.521024.cn

[H05] 捕获特定类型
来源：http://bc.chemitech.net.cn

Py:   except ValueError as e:
来源：http://uj.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jx.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://ey.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://we.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://gr.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nm.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://gp.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://st.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://ha.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://lb.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mm.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sp.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gu.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lh.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fc.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://qs.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://sr.szxytkj.cn

[H07] 断言
来源：http://qv.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://bx.9csxet.cn

PHP:  assert($x > 0);
来源：http://id.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://nw.huanxung.cn

TS:   console.assert(x > 0);
来源：http://zi.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://rb.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rl.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pz.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://vu.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://jy.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://vf.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wf.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://au.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ga.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tg.huixiangedu.cn

Go:   err.Error()
来源：http://gd.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://ur.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://jd.shtwfgs.cn

[H09] 带错误码的异常
来源：http://ph.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://za.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://am.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tq.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jy.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mi.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rq.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tw.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ku.521024.cn

[H10] 资源自动释放
来源：http://ej.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://oi.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tg.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jt.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://du.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://er.hnjuh.cn

Go:   defer f.Close()
来源：http://xg.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nc.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gx.9csxet.cn

================================================================================
来源：http://zq.newstarts.cn

I. 正则表达式
来源：http://bc.shtwfgs.cn

================================================================================
来源：http://oc.colortex.cn

[I01] 判断是否匹配
来源：http://qp.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://or.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qh.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://su.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://qx.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yw.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ui.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://kr.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hc.nszjky.cn

[I02] 提取所有匹配
来源：http://if.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://os.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xn.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://by.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://tm.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ns.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vh.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://jd.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ip.lnxyls.cn

[I03] 提取捕获分组
来源：http://af.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vf.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lf.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mq.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://za.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vj.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hx.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://by.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gm.yuntaijiaju.cn

[I04] 正则替换
来源：http://bj.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lg.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iw.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zw.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sp.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ez.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wo.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://al.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://os.bjjhwx.cn

[I05] 按正则拆分
来源：http://ut.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tn.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mj.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://oa.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://uk.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://nb.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vc.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ww.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kv.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rc.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pv.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ya.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rm.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://co.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lo.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://an.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ql.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pw.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://jh.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wf.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mx.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sw.521024.cn

TS:   /error/gim
来源：http://nv.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://id.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fn.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://tz.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uc.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://ic.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nz.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yl.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sx.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sk.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lx.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lg.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fp.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ow.hahajie.cn

================================================================================
来源：http://jb.haigaiapp.cn

J. 日期与时间
来源：http://bu.chemitech.net.cn

================================================================================
来源：http://nm.panjiajie.cn

[J01] 获取当前时间
来源：http://ee.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gr.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ir.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://ul.newstarts.cn

TS:   new Date();  Date.now()
来源：http://wk.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://en.bookmarksfly.cn

Go:   time.Now()
来源：http://tr.yuexingan06.cn

Ruby: Time.now
来源：http://kl.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qm.asd995.cn

[J02] 格式化输出
来源：http://yt.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nb.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mj.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bi.nicolike.cn

TS:   d.toISOString()
来源：http://ny.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nb.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vh.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jd.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lk.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://vo.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vb.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pd.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://sq.chemitech.net.cn

TS:   new Date("2024-01-02")
来源：http://cn.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uv.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iw.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://rs.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ma.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://iy.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://am.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rs.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bx.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bq.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bu.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gi.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kr.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://pf.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://hi.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ex.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ey.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pe.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://si.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uo.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://kl.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://iw.shxzukj.cn

[J06] 计算两时间之差
来源：http://ba.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://rn.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://xt.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rw.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rs.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gh.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://es.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://ce.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://ns.bjjhwx.cn

[J07] 比较两个日期
来源：http://ba.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://tu.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eg.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fx.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hv.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dz.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ih.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://li.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://nf.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://zd.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rg.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://li.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lk.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://os.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jd.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lc.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ga.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hx.nicolike.cn

[J09] 时区处理
来源：http://oj.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://it.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dr.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ui.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qo.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xt.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://an.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jl.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xc.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://if.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wt.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://po.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qt.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fd.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cd.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qz.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://in.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qu.521024.cn

================================================================================
来源：http://fa.newstarts.cn

K. JSON 与序列化
来源：http://wc.9csxet.cn

================================================================================
来源：http://hw.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://lp.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rw.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ns.521024.cn

JS:   JSON.stringify(obj)
来源：http://ad.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://vr.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dn.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://dw.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ar.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gv.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://bo.szxytkj.cn

Py:   json.loads(s)
来源：http://pd.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sy.shxzukj.cn

JS:   JSON.parse(s)
来源：http://hm.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://uh.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fb.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://la.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://kh.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wz.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://xe.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://py.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hr.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sd.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cg.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eo.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wf.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fw.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ly.nszjky.cn

[K04] 读取 JSON 文件
来源：http://kd.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jm.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hk.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vl.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sw.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hm.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bc.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ea.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kt.521024.cn

[K05] 深拷贝对象
来源：http://mo.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://mt.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://bv.521024.cn

JS:   structuredClone(obj)
来源：http://og.9csxet.cn

TS:   structuredClone(obj)
来源：http://mv.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://el.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yg.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vl.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fs.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://lu.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://se.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vr.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cv.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uc.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gh.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sn.huixiangedu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dp.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ec.hahajie.cn

[K07] 进制转换
来源：http://tv.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gf.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zt.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jo.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vb.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ac.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eb.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://so.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://to.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://nf.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://fw.hahajie.cn


<!-- 参考信息 -->