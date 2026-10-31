代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://zd.colortex.cn

[H04] 自定义异常类型
来源：http://oj.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://ji.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ro.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://ff.huanxung.cn

TS:   class MyError extends Error {}
来源：http://hh.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://xk.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yw.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://ob.asd995.cn

C#:   class MyException : Exception {}
来源：http://sx.shxzukj.cn

[H05] 捕获特定类型
来源：http://lp.shxzukj.cn

Py:   except ValueError as e:
来源：http://kl.asd995.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xp.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://zi.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://uj.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://qm.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ms.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://sp.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iz.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://az.hahajie.cn

Py:   value = d.get("k") or default
来源：http://hv.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tj.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cl.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://iy.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ar.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bs.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://kb.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://pe.shxzukj.cn

[H07] 断言
来源：http://pc.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://rm.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://ze.szsharing.cn

JS:   console.assert(x > 0);
来源：http://md.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://zq.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://rn.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xr.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bj.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://wi.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://vb.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://iu.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zq.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://gu.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nk.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://is.huanxung.cn

Go:   err.Error()
来源：http://bp.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://ss.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://ls.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://kb.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dl.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dh.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sr.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kh.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dt.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://os.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yh.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pg.jctech888.com.cn

[H10] 资源自动释放
来源：http://dr.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ap.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kh.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wu.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zw.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ie.jctech888.com.cn

Go:   defer f.Close()
来源：http://hq.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://di.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bw.colortex.cn

================================================================================
来源：http://mi.jctech888.com.cn

I. 正则表达式
来源：http://mt.szxytkj.cn

================================================================================
来源：http://it.asd995.cn

[I01] 判断是否匹配
来源：http://mb.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tl.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sg.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://yx.nszjky.cn

TS:   /\d+/.test(s)
来源：http://zz.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bz.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lx.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://lp.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wy.haigaiapp.cn

[I02] 提取所有匹配
来源：http://ea.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://fg.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rw.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uz.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://dx.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ac.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ct.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://ra.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dz.gzmigu.cn

[I03] 提取捕获分组
来源：http://bz.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vi.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pe.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ti.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qv.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cd.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cu.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dw.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qo.huixiangedu.cn

[I04] 正则替换
来源：http://dh.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jn.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uq.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hd.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wc.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ya.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ql.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jh.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kc.hnjuh.cn

[I05] 按正则拆分
来源：http://ht.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wx.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pl.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://mm.chemitech.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://jc.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://ha.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xi.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lw.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lx.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jz.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lc.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ko.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wy.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ih.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qd.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yq.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rv.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uy.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://hl.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eb.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kh.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ng.bjjhwx.cn

TS:   /error/gim
来源：http://xs.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qs.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aa.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://jf.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hd.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://nz.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zn.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yz.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xn.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gk.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ff.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qg.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fk.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tw.chemitech.net.cn

================================================================================
来源：http://hb.huixinmuqiang.cn

J. 日期与时间
来源：http://ex.nicolike.cn

================================================================================
来源：http://ij.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://ht.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dm.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dm.nszjky.cn

JS:   new Date();  Date.now()
来源：http://br.szsharing.cn

TS:   new Date();  Date.now()
来源：http://en.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nj.hahajie.cn

Go:   time.Now()
来源：http://ds.yuexingan06.cn

Ruby: Time.now
来源：http://dx.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kj.szsharing.cn

[J02] 格式化输出
来源：http://yx.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gt.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pa.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sz.muxihuayi.cn

TS:   d.toISOString()
来源：http://du.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bn.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sl.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xo.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kh.newstarts.cn

[J03] 字符串解析为日期
来源：http://qe.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://av.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wf.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://wh.asd995.cn

TS:   new Date("2024-01-02")
来源：http://li.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gb.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://st.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://et.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dz.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://th.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xp.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://se.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hk.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://av.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sr.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kq.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uf.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dz.521024.cn

[J05] 时间加减（加 7 天）
来源：http://bv.wgjwhj.cn

Py:   now + timedelta(days=7)
来源：http://lf.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://oj.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jw.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zj.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://sn.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jw.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://om.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qz.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://zn.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://wf.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://kc.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vc.hnjuh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vu.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nc.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://rr.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://qx.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://xf.gzmigu.cn

[J07] 比较两个日期
来源：http://cj.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://ry.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xq.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hc.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vr.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nz.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iu.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ra.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://gz.hnjuh.cn

[J08] 提取年月日与星期
来源：http://ju.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fj.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xk.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jf.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ii.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yj.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jt.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ml.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wo.haigaiapp.cn

[J09] 时区处理
来源：http://un.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ax.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nb.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://we.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://li.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vb.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ve.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yp.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hm.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://jz.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xl.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ev.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jw.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://do.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fh.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tx.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zn.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ha.nszjky.cn

================================================================================
来源：http://jp.szxytkj.cn

K. JSON 与序列化
来源：http://bz.szsharing.cn

================================================================================
来源：http://ms.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://pa.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://od.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vw.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://iz.colortex.cn

TS:   JSON.stringify(obj)
来源：http://qu.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ii.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://lw.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vr.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oc.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://lz.colortex.cn

Py:   json.loads(s)
来源：http://jx.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oq.szsharing.cn

JS:   JSON.parse(s)
来源：http://gu.gzmigu.cn

TS:   JSON.parse(s)
来源：http://sa.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nj.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://eq.9csxet.cn

Ruby: JSON.parse(s)
来源：http://ai.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nb.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://cq.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wo.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yf.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ix.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xq.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ps.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xd.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://va.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uq.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://ax.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ur.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nw.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fv.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bs.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vh.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ie.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ky.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rk.jctech888.com.cn

[K05] 深拷贝对象
来源：http://yt.521024.cn

Py:   copy.deepcopy(obj)
来源：http://hi.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://ti.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://zb.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://ng.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rv.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tu.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://it.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yt.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://yd.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://di.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://az.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fm.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pm.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vk.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rx.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yw.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ql.hnjuh.cn

[K07] 进制转换
来源：http://qh.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fj.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pd.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ic.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vd.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://de.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sy.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pn.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bu.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://zh.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://it.shxzukj.cn


<!-- 参考信息 -->