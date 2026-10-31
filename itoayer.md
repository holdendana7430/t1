代发 wailian999

TS:   throw new Error("错误信息");
来源：http://nx.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gp.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jt.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dp.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vl.szsharing.cn

[H04] 自定义异常类型
来源：http://hl.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://ke.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dj.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://tn.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://rp.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://ho.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xm.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://oe.nszjky.cn

C#:   class MyException : Exception {}
来源：http://tf.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://sy.lnxyls.cn

Py:   except ValueError as e:
来源：http://lj.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ed.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://zx.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://jl.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://se.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dd.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://zr.szxytkj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://df.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://ui.521024.cn

Py:   value = d.get("k") or default
来源：http://nj.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ua.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://aw.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xu.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ay.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://er.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://ai.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://ld.bookmarksfly.cn

[H07] 断言
来源：http://jz.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://gh.szsharing.cn

PHP:  assert($x > 0);
来源：http://ty.chemitech.net.cn

JS:   console.assert(x > 0);
来源：http://yy.9csxet.cn

TS:   console.assert(x > 0);
来源：http://dx.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://vf.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://op.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ez.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://oh.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://nl.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://bc.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://js.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://zt.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yg.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rw.shtwfgs.cn

Go:   err.Error()
来源：http://uh.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://ab.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://xh.gzmigu.cn

[H09] 带错误码的异常
来源：http://cs.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fb.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ao.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ao.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wy.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gq.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kg.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qx.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kr.gzmigu.cn

[H10] 资源自动释放
来源：http://nc.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zk.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gc.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fc.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yu.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ri.shtwfgs.cn

Go:   defer f.Close()
来源：http://vs.gzmigu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cx.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://au.lnxyls.cn

================================================================================
来源：http://cm.szxytkj.cn

I. 正则表达式
来源：http://ez.hahajie.cn

================================================================================
来源：http://cy.nszjky.cn

[I01] 判断是否匹配
来源：http://iw.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pi.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://as.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://da.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://le.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tf.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bb.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://wa.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xb.huixiangedu.cn

[I02] 提取所有匹配
来源：http://ns.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://py.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jn.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ij.521024.cn

TS:   s.match(/\d+/g)
来源：http://er.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://df.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fd.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://oo.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cs.huanxung.cn

[I03] 提取捕获分组
来源：http://mn.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nu.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qk.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://od.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gn.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vf.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jc.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jf.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iz.panjiajie.cn

[I04] 正则替换
来源：http://qs.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xs.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pd.lnxyls.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yl.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ef.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wq.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ga.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gl.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://li.panjiajie.cn

[I05] 按正则拆分
来源：http://jx.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hy.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ac.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://di.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ws.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://ux.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hx.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ft.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uy.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gd.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tr.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cr.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://im.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bk.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ts.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fo.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ue.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yz.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://ft.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dj.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ex.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://my.colortex.cn

TS:   /error/gim
来源：http://ns.yuexingan06.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gg.521024.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cd.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://rs.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ai.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://nl.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kv.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cw.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nv.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ki.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pw.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ur.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ps.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sm.9csxet.cn

================================================================================
来源：http://ev.shxzukj.cn

J. 日期与时间
来源：http://ah.shxzskj.cn

================================================================================
来源：http://km.muxihuayi.cn

[J01] 获取当前时间
来源：http://qc.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hh.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ze.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://hw.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://ry.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wy.bookmarksfly.cn

Go:   time.Now()
来源：http://la.521024.cn

Ruby: Time.now
来源：http://km.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ls.huanxung.cn

[J02] 格式化输出
来源：http://ei.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ak.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zr.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xj.521024.cn

TS:   d.toISOString()
来源：http://ra.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ao.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rl.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gc.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gh.colortex.cn

[J03] 字符串解析为日期
来源：http://ap.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ey.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://an.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://ms.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://es.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://eo.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gz.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://zy.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://en.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://qt.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://if.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oz.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ah.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://np.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xq.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oy.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ps.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iq.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://sq.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://yv.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ij.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rg.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ta.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://ug.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qp.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://ls.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fo.jctech888.com.cn

[J06] 计算两时间之差
来源：http://xu.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://rt.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://df.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ab.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cn.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xx.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://zs.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://al.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://hc.panjiajie.cn

[J07] 比较两个日期
来源：http://yk.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://kb.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yr.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://eq.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kk.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eo.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vh.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lz.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://cp.panjiajie.cn

[J08] 提取年月日与星期
来源：http://ad.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rc.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pj.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fs.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ye.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iy.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://in.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://og.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pq.hnjuh.cn

[J09] 时区处理
来源：http://tw.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://si.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://et.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://de.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xm.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://me.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vp.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dn.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zw.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://gu.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nh.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cz.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cb.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wv.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qj.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vk.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xu.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ht.shxzukj.cn

================================================================================
来源：http://tr.asd995.cn

K. JSON 与序列化
来源：http://vt.huixiangedu.cn

================================================================================
来源：http://fb.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://lq.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rl.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ki.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://ul.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://ye.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pq.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://wl.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://di.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xm.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://br.lnxyls.cn

Py:   json.loads(s)
来源：http://ly.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wa.szxytkj.cn

JS:   JSON.parse(s)
来源：http://tw.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://ux.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mf.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ij.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://oo.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hd.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://gj.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vc.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vr.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yz.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wm.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hq.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://et.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ff.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xq.9csxet.cn

[K04] 读取 JSON 文件
来源：http://xx.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bk.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jp.szxytkj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ta.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bt.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mx.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uw.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://am.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mb.asd995.cn

[K05] 深拷贝对象
来源：http://ga.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://wn.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://sd.colortex.cn

JS:   structuredClone(obj)
来源：http://he.nszjky.cn

TS:   structuredClone(obj)
来源：http://zy.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hi.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ty.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fm.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ti.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://rn.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ju.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://te.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wh.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rw.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bt.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jn.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uu.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iu.muxihuayi.cn

[K07] 进制转换
来源：http://tl.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bs.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mj.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wl.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qj.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://si.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pw.huixinmuqiang.cn


<!-- 参考信息 -->