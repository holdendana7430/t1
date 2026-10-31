代发 wailian999

JS:   class MyError extends Error {}
来源：http://nv.newstarts.cn

TS:   class MyError extends Error {}
来源：http://op.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://uc.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ms.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://qs.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://lr.huixiangedu.cn

[H05] 捕获特定类型
来源：http://rb.haigaiapp.cn

Py:   except ValueError as e:
来源：http://tj.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vd.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://ja.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://rc.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://wr.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vh.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://cf.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tj.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://sj.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://dv.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dq.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wo.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mi.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bj.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://iw.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://sl.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://te.asd995.cn

[H07] 断言
来源：http://sh.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://ev.panjiajie.cn

PHP:  assert($x > 0);
来源：http://yn.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://lj.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://gj.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://pf.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lo.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yt.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://bd.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://tl.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://mo.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hd.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://tg.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xy.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pe.muxihuayi.cn

Go:   err.Error()
来源：http://mh.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://xx.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://ze.colortex.cn

[H09] 带错误码的异常
来源：http://fg.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://su.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mu.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xo.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ht.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cb.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dy.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wz.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fb.9csxet.cn

[H10] 资源自动释放
来源：http://im.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wn.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hm.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ze.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nh.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kb.szxytkj.cn

Go:   defer f.Close()
来源：http://zk.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ax.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://df.shtwfgs.cn

================================================================================
来源：http://dg.shxzskj.cn

I. 正则表达式
来源：http://pr.chemitech.net.cn

================================================================================
来源：http://ma.chemitech.net.cn

[I01] 判断是否匹配
来源：http://ja.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dl.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dd.shtwfgs.cn

JS:   /\d+/.test(s)
来源：http://gp.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://kx.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lc.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mn.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://bo.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pc.colortex.cn

[I02] 提取所有匹配
来源：http://tl.521024.cn

Py:   re.findall(r"\d+", s)
来源：http://fk.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pq.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oa.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://vy.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://on.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ng.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://ou.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://za.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://qx.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ai.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cg.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lc.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lp.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kc.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mm.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cg.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fw.asd995.cn

[I04] 正则替换
来源：http://ze.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pv.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jp.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wy.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yi.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zm.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jo.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sn.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ze.newstarts.cn

[I05] 按正则拆分
来源：http://cn.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yv.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hq.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://eh.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://bs.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://xa.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ua.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wc.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ec.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kr.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rg.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ai.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dd.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ed.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qp.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vv.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sj.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ud.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://ix.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kd.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pt.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oj.shxzskj.cn

TS:   /error/gim
来源：http://qf.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wj.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ob.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://rm.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ko.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://ig.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ou.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qt.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hf.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gm.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mw.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gn.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qw.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yj.wgjwhj.cn

================================================================================
来源：http://ky.szxytkj.cn

J. 日期与时间
来源：http://hc.colortex.cn

================================================================================
来源：http://qb.newstarts.cn

[J01] 获取当前时间
来源：http://gd.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nr.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xo.nszjky.cn

JS:   new Date();  Date.now()
来源：http://va.9csxet.cn

TS:   new Date();  Date.now()
来源：http://ty.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fw.jianghongdianzi.cn

Go:   time.Now()
来源：http://oz.hahajie.cn

Ruby: Time.now
来源：http://dv.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rc.yuexingan06.cn

[J02] 格式化输出
来源：http://xm.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pc.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fq.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mu.newstarts.cn

TS:   d.toISOString()
来源：http://pd.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jd.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gr.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ju.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ww.newstarts.cn

[J03] 字符串解析为日期
来源：http://lr.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sl.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fk.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://ex.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://he.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tw.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ry.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://ei.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fc.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://sj.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ef.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nr.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yl.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cw.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qg.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zn.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gn.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ji.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://cn.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://ng.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mp.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xg.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ld.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://pw.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sj.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://sc.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kx.shtwfgs.cn

[J06] 计算两时间之差
来源：http://en.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://kb.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://uw.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kk.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bi.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jh.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://bh.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://bk.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://po.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://qn.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://ei.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kg.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rt.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wt.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://va.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ie.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wh.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://qt.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://vw.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rb.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eo.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vg.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ay.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rs.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://en.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fo.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wj.szsharing.cn

[J09] 时区处理
来源：http://jk.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://is.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hs.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xk.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tu.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lb.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://je.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pp.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://au.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://lo.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ke.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lq.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aa.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ud.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ba.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wp.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xm.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ya.wgjwhj.cn

================================================================================
来源：http://sn.gzmigu.cn

K. JSON 与序列化
来源：http://vl.jctech888.com.cn

================================================================================
来源：http://nk.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://oq.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jr.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qy.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://kr.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://ns.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hm.9csxet.cn

Go:   json.Marshal(obj)
来源：http://zh.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sg.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fs.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://og.shxzskj.cn

Py:   json.loads(s)
来源：http://sj.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ty.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://dh.nszjky.cn

TS:   JSON.parse(s)
来源：http://he.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wr.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://yh.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://lw.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yy.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://cc.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ew.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zh.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mo.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cc.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ii.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://up.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wn.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gm.9csxet.cn

[K04] 读取 JSON 文件
来源：http://nn.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iq.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qc.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mn.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pd.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ig.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ht.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mk.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lh.wgjwhj.cn

[K05] 深拷贝对象
来源：http://mv.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://lk.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://qw.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://ed.colortex.cn

TS:   structuredClone(obj)
来源：http://xh.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://is.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oq.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wa.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kf.yuexingan06.cn

[K06] 解析 URL 查询串
来源：http://tj.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oj.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eb.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pi.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ly.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yy.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xc.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cq.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sd.muxihuayi.cn

[K07] 进制转换
来源：http://gw.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ra.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jq.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uz.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kd.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lw.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ga.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kq.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rm.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://tb.asd995.cn

Py:   pickle.dumps(obj)
来源：http://hc.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dq.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://ot.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://pb.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rt.shxzskj.cn


<!-- 参考信息 -->