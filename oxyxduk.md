代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://hc.yuexingan06.cn

[H04] 自定义异常类型
来源：http://sg.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://ql.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rb.nicolike.cn

JS:   class MyError extends Error {}
来源：http://lr.colortex.cn

TS:   class MyError extends Error {}
来源：http://to.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://cd.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vs.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://lq.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://qk.szsharing.cn

[H05] 捕获特定类型
来源：http://ut.haigaiapp.cn

Py:   except ValueError as e:
来源：http://of.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bo.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://hg.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://hw.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://jp.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hk.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://cy.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gm.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://pn.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://ry.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dt.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gd.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://di.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gp.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ij.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://ar.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://qh.newstarts.cn

[H07] 断言
来源：http://fm.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://lx.asd995.cn

PHP:  assert($x > 0);
来源：http://ip.nszjky.cn

JS:   console.assert(x > 0);
来源：http://vk.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://tk.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://oh.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tr.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jn.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://gy.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://mb.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://ov.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ro.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://wj.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://av.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ys.hnjuh.cn

Go:   err.Error()
来源：http://yc.panjiajie.cn

Ruby: e.message;  e.backtrace
来源：http://nv.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://ae.asd995.cn

[H09] 带错误码的异常
来源：http://lo.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fe.hnjuh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ig.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zh.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qj.szsharing.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fg.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bg.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lv.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oc.nicolike.cn

[H10] 资源自动释放
来源：http://fj.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ab.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wu.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nx.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://my.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yo.nszjky.cn

Go:   defer f.Close()
来源：http://xz.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sw.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qh.yuntaijiaju.cn

================================================================================
来源：http://dj.wgjwhj.cn

I. 正则表达式
来源：http://vf.lnxyls.cn

================================================================================
来源：http://hy.hahajie.cn

[I01] 判断是否匹配
来源：http://av.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ib.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gy.asd995.cn

JS:   /\d+/.test(s)
来源：http://uo.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://vu.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fp.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uh.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://tq.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jt.chemitech.net.cn

[I02] 提取所有匹配
来源：http://ix.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://cf.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qw.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ac.colortex.cn

TS:   s.match(/\d+/g)
来源：http://fn.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nf.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://px.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://fa.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://om.huixiangedu.cn

[I03] 提取捕获分组
来源：http://mc.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zl.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yd.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vi.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ef.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cp.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kr.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ay.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xh.szxytkj.cn

[I04] 正则替换
来源：http://zz.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gy.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iv.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dj.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qz.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mx.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xi.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hc.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://be.panjiajie.cn

[I05] 按正则拆分
来源：http://xo.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pl.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dm.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://ss.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://hq.nicolike.cn

Java: s.split("\\s*,\\s*")
来源：http://zk.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wz.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://to.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zk.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://en.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yk.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rs.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yw.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mz.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gi.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nu.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dy.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fq.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://te.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yk.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uo.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://si.newstarts.cn

TS:   /error/gim
来源：http://rk.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ng.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qs.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://wx.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fn.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://dy.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tg.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tx.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fu.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eo.yuntaijiaju.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ep.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xw.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tv.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vb.521024.cn

================================================================================
来源：http://kn.newstarts.cn

J. 日期与时间
来源：http://lv.huixinmuqiang.cn

================================================================================
来源：http://je.chemitech.net.cn

[J01] 获取当前时间
来源：http://wv.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fa.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vl.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://gn.szsharing.cn

TS:   new Date();  Date.now()
来源：http://df.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://um.nszjky.cn

Go:   time.Now()
来源：http://mt.hnjuh.cn

Ruby: Time.now
来源：http://gh.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gp.gzmigu.cn

[J02] 格式化输出
来源：http://dc.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kc.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ct.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lm.szsharing.cn

TS:   d.toISOString()
来源：http://qg.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mw.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lj.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://az.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bv.panjiajie.cn

[J03] 字符串解析为日期
来源：http://dr.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nv.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ot.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://vy.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://sf.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://al.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ml.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://ps.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rt.colortex.cn

[J04] 时间戳与日期互转
来源：http://jq.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qd.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jr.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://th.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ba.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ti.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ma.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bh.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://au.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://vn.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://xc.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bw.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zk.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fo.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://px.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kk.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://yc.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gg.huixiangedu.cn

[J06] 计算两时间之差
来源：http://xs.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://xe.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://xf.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ax.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mc.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wt.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://td.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://tv.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://ef.hnjuh.cn

[J07] 比较两个日期
来源：http://ed.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://li.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bm.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zv.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yl.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dt.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ji.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ki.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://gf.nszjky.cn

[J08] 提取年月日与星期
来源：http://ge.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bc.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cu.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tv.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gk.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tt.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ap.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yv.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vh.nicolike.cn

[J09] 时区处理
来源：http://sc.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://he.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ji.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fw.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://op.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pz.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ll.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jz.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fv.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://tj.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tj.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sj.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jg.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ax.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://id.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yl.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bf.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lw.nicolike.cn

================================================================================
来源：http://xj.bjjhwx.cn

K. JSON 与序列化
来源：http://jh.wgjwhj.cn

================================================================================
来源：http://pb.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://wm.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qd.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sp.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://oy.colortex.cn

TS:   JSON.stringify(obj)
来源：http://ms.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://up.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://cs.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fj.lnxyls.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ns.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://er.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://ws.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oy.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://am.newstarts.cn

TS:   JSON.parse(s)
来源：http://dt.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iu.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://sn.hahajie.cn

Ruby: JSON.parse(s)
来源：http://ox.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dx.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://dm.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sw.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gk.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ga.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sl.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gs.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tx.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gp.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aa.hahajie.cn

[K04] 读取 JSON 文件
来源：http://dd.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hy.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ob.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oj.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vv.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vu.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eb.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cx.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tg.nszjky.cn

[K05] 深拷贝对象
来源：http://lj.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://zj.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://kj.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://vy.shxzukj.cn

TS:   structuredClone(obj)
来源：http://uh.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ha.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aq.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://id.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ic.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://fa.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dv.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gj.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ff.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qc.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iy.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jq.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uh.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gz.huixiangedu.cn

[K07] 进制转换
来源：http://uv.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dg.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kr.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fx.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nm.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jb.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://na.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jw.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vj.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://as.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://wx.gzmigu.cn


<!-- 参考信息 -->