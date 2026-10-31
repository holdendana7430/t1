代发 wailian999

TS:   throw new Error("错误信息");
来源：http://yx.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gd.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dd.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ni.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://je.hnjuh.cn

[H04] 自定义异常类型
来源：http://lb.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://lc.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ms.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://mk.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://yc.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://rw.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lc.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://bx.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://cx.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://rt.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://df.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xp.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://nk.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://sk.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://nb.nszjky.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ir.9csxet.cn

Ruby: rescue ArgumentError => e
来源：http://jg.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gn.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://hi.szsharing.cn

Py:   value = d.get("k") or default
来源：http://bd.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nx.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ye.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lz.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nk.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://by.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://cq.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://dl.haigaiapp.cn

[H07] 断言
来源：http://dw.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://sg.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://jv.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://oo.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://vq.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://rp.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sm.nicolike.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wz.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://fk.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://ze.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://rb.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hq.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://rz.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ol.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xo.jianghongdianzi.cn

Go:   err.Error()
来源：http://ed.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://is.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://cj.muxihuayi.cn

[H09] 带错误码的异常
来源：http://qu.nszjky.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ub.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ps.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ng.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ro.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wc.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cv.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ph.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zd.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://oy.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ti.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kr.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dw.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dk.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fi.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://wv.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pq.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dh.newstarts.cn

================================================================================
来源：http://ay.newstarts.cn

I. 正则表达式
来源：http://uz.haigaiapp.cn

================================================================================
来源：http://qy.haigaiapp.cn

[I01] 判断是否匹配
来源：http://jo.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dy.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vn.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://gm.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://wy.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qo.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vh.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://br.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fo.lnxyls.cn

[I02] 提取所有匹配
来源：http://kj.szsharing.cn

Py:   re.findall(r"\d+", s)
来源：http://ye.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qg.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uu.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://gw.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rt.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kl.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://ca.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lc.hahajie.cn

[I03] 提取捕获分组
来源：http://wm.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ls.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eb.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nr.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fv.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ci.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gb.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://er.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ur.huanxung.cn

[I04] 正则替换
来源：http://dp.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tc.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gn.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wk.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nx.haigaiapp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eg.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nc.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kq.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wn.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://gu.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pa.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bs.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://ap.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://et.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://oq.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://by.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://in.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ly.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cg.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yi.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pp.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ia.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qb.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ie.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mu.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ga.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ob.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://qt.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kv.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ux.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oy.shtwfgs.cn

TS:   /error/gim
来源：http://rk.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mt.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mh.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://na.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oi.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://rt.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cz.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sp.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gy.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hc.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tr.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xt.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sa.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eh.haigaiapp.cn

================================================================================
来源：http://ma.szxytkj.cn

J. 日期与时间
来源：http://ml.9csxet.cn

================================================================================
来源：http://ki.huixiangedu.cn

[J01] 获取当前时间
来源：http://pg.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nh.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sk.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://oj.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://fk.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hg.panjiajie.cn

Go:   time.Now()
来源：http://za.yuexingan06.cn

Ruby: Time.now
来源：http://px.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iv.wgjwhj.cn

[J02] 格式化输出
来源：http://fd.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tt.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ps.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zw.hnjuh.cn

TS:   d.toISOString()
来源：http://zm.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dk.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dg.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ow.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aj.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://yz.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qq.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gx.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://cs.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://dk.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tc.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pz.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://os.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xa.9csxet.cn

[J04] 时间戳与日期互转
来源：http://jk.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kx.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ez.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yb.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zi.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aa.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://at.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xb.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xc.521024.cn

[J05] 时间加减（加 7 天）
来源：http://tw.wgjwhj.cn

Py:   now + timedelta(days=7)
来源：http://ag.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ac.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fm.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fa.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://wr.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ng.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://al.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bz.shtwfgs.cn

[J06] 计算两时间之差
来源：http://ro.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://jm.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://gf.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sy.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bw.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bo.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://uw.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://sc.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://ci.szxytkj.cn

[J07] 比较两个日期
来源：http://jz.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://ha.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zx.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qn.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://us.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gr.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zw.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zm.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://mx.gzmigu.cn

[J08] 提取年月日与星期
来源：http://iz.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qy.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nl.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://od.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ni.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mg.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rj.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kr.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pr.nicolike.cn

[J09] 时区处理
来源：http://nz.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yu.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pv.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yq.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fs.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sq.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zv.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pv.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://at.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://eq.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aj.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sf.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dv.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zi.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nb.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pp.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ge.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gb.haigaiapp.cn

================================================================================
来源：http://xw.jctech888.com.cn

K. JSON 与序列化
来源：http://uw.jctech888.com.cn

================================================================================
来源：http://uk.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://gc.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://im.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yz.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://ja.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://dc.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vy.nszjky.cn

Go:   json.Marshal(obj)
来源：http://ze.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gx.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zr.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://su.9csxet.cn

Py:   json.loads(s)
来源：http://qs.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rc.asd995.cn

JS:   JSON.parse(s)
来源：http://qu.lnxyls.cn

TS:   JSON.parse(s)
来源：http://gq.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hl.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://sv.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://pa.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kc.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://ux.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nc.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rz.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zm.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://no.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nl.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ki.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jw.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dc.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://hl.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ou.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://li.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tj.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mk.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qz.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sl.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tr.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eb.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://ja.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://gw.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://df.gzmigu.cn

JS:   structuredClone(obj)
来源：http://yh.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://zd.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xe.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fh.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rq.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ww.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://po.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hy.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rp.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://km.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://by.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nj.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wc.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://za.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ia.huixiangedu.cn

[K07] 进制转换
来源：http://rz.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wt.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gy.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rx.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kl.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://og.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zg.nicolike.cn


<!-- 参考信息 -->