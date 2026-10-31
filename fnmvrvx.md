代发 wailian999

JS:   class MyError extends Error {}
来源：http://pa.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://cy.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://bu.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xd.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://ad.nszjky.cn

C#:   class MyException : Exception {}
来源：http://rh.szxytkj.cn

[H05] 捕获特定类型
来源：http://hr.newstarts.cn

Py:   except ValueError as e:
来源：http://dl.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dp.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://ed.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://xf.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://bs.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bx.9csxet.cn

Ruby: rescue ArgumentError => e
来源：http://ir.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fj.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://zp.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://co.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sz.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dh.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bw.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wx.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kx.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://ko.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://xp.shxzukj.cn

[H07] 断言
来源：http://th.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://dv.asd995.cn

PHP:  assert($x > 0);
来源：http://nb.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://gd.colortex.cn

TS:   console.assert(x > 0);
来源：http://ag.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://wk.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bf.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ux.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://vz.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://aj.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://jm.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vj.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://nf.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ex.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wu.shtwfgs.cn

Go:   err.Error()
来源：http://mb.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://wj.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://xl.nicolike.cn

[H09] 带错误码的异常
来源：http://as.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ko.yuexingan06.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gq.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iz.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lk.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yk.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cl.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gx.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gg.bjjhwx.cn

[H10] 资源自动释放
来源：http://oj.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kn.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fw.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dm.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qk.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ar.shxzskj.cn

Go:   defer f.Close()
来源：http://iy.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ub.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zx.newstarts.cn

================================================================================
来源：http://sq.gzmigu.cn

I. 正则表达式
来源：http://kq.gzmigu.cn

================================================================================
来源：http://na.bjjhwx.cn

[I01] 判断是否匹配
来源：http://ec.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ts.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ue.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://nr.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://ae.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ms.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://te.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://pf.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sk.panjiajie.cn

[I02] 提取所有匹配
来源：http://cp.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://jg.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vq.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ks.521024.cn

TS:   s.match(/\d+/g)
来源：http://be.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qn.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ft.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://bt.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://no.hahajie.cn

[I03] 提取捕获分组
来源：http://si.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ep.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hd.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ha.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wa.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jx.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://me.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rq.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://is.muxihuayi.cn

[I04] 正则替换
来源：http://yn.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://km.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hf.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ia.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ss.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cv.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rb.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pp.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://us.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://js.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dv.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vo.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://fk.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://nw.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://ok.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gs.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://il.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sv.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lm.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qg.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cj.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rb.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ws.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tv.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xh.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ar.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lg.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://cv.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://km.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cd.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://za.panjiajie.cn

TS:   /error/gim
来源：http://cg.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pq.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fl.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://ga.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://aa.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://ju.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yd.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cl.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sf.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ii.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kx.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yu.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sb.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xx.jctech888.com.cn

================================================================================
来源：http://lr.9csxet.cn

J. 日期与时间
来源：http://xa.szxytkj.cn

================================================================================
来源：http://gs.jctech888.com.cn

[J01] 获取当前时间
来源：http://rz.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ht.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vu.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://dn.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://iu.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mv.yuexingan06.cn

Go:   time.Now()
来源：http://rf.gzmigu.cn

Ruby: Time.now
来源：http://qk.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ua.shxzukj.cn

[J02] 格式化输出
来源：http://rq.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://se.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ww.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://er.lnxyls.cn

TS:   d.toISOString()
来源：http://pv.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jl.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gx.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ac.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lq.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://an.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vk.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jk.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://hf.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://rz.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ro.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dl.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://fk.521024.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://my.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://gf.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://br.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://di.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pc.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kk.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nm.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sw.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dy.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aq.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://ns.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://ot.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ik.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nm.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zz.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://un.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ei.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://rd.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jo.hahajie.cn

[J06] 计算两时间之差
来源：http://ce.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://co.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://sk.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kg.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ek.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jd.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://dv.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://wv.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://sj.jctech888.com.cn

[J07] 比较两个日期
来源：http://nq.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://mg.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fc.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pi.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xo.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gk.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jj.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zw.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://pl.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://vj.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nc.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ah.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://je.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tl.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ls.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qx.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gq.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ma.nicolike.cn

[J09] 时区处理
来源：http://hy.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bs.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qf.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cq.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uk.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ov.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oo.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dk.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kd.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://ja.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fm.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tq.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://up.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vn.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cc.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rs.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://up.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ii.nszjky.cn

================================================================================
来源：http://mh.szsharing.cn

K. JSON 与序列化
来源：http://jn.szxytkj.cn

================================================================================
来源：http://bt.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://xp.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pk.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://in.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://mp.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://ka.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ho.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://ix.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pi.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ae.colortex.cn

[K02] JSON 字符串转对象
来源：http://rt.muxihuayi.cn

Py:   json.loads(s)
来源：http://sj.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://du.hahajie.cn

JS:   JSON.parse(s)
来源：http://nv.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://bk.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wy.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://zy.szsharing.cn

Ruby: JSON.parse(s)
来源：http://je.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fc.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://ti.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xm.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://io.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rv.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rt.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qf.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cm.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://da.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dh.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://qd.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://td.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ak.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uc.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nk.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://il.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zh.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tg.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bo.newstarts.cn

[K05] 深拷贝对象
来源：http://hk.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://mn.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://ub.hnjuh.cn

JS:   structuredClone(obj)
来源：http://cz.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://fp.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zs.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qm.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cq.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lb.colortex.cn

[K06] 解析 URL 查询串
来源：http://xp.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lb.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jk.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vu.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://da.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ek.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hw.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ur.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bn.panjiajie.cn

[K07] 进制转换
来源：http://il.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ly.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oh.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nn.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gp.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yy.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ns.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ya.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mq.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://yn.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://ch.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vn.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://ie.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://vn.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kk.chemitech.net.cn


<!-- 参考信息 -->