代发 wailian999

JS:   class MyError extends Error {}
来源：http://ex.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://ha.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://qp.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pt.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://fn.huanxung.cn

C#:   class MyException : Exception {}
来源：http://wr.haigaiapp.cn

[H05] 捕获特定类型
来源：http://rr.lnxyls.cn

Py:   except ValueError as e:
来源：http://dh.lnxyls.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qa.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://qb.huanxung.cn

TS:   if (e instanceof TypeError) {}
来源：http://gj.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://xw.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jl.9csxet.cn

Ruby: rescue ArgumentError => e
来源：http://py.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mp.szxytkj.cn

[H06] 可选值 / 空值安全访问
来源：http://yy.newstarts.cn

Py:   value = d.get("k") or default
来源：http://nd.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ax.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://to.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fg.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kr.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ix.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://xj.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://dd.jctech888.com.cn

[H07] 断言
来源：http://wd.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://ce.hahajie.cn

PHP:  assert($x > 0);
来源：http://iy.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://hw.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://sl.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://cz.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mw.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pw.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://ui.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://ss.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://va.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vs.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://vo.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qn.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mq.huixinmuqiang.cn

Go:   err.Error()
来源：http://xv.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://ef.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://bw.asd995.cn

[H09] 带错误码的异常
来源：http://sb.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xy.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hp.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ke.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rb.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sy.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wy.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rt.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dz.nicolike.cn

[H10] 资源自动释放
来源：http://dg.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lk.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jd.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wq.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bt.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fa.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://qj.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xp.yuntaijiaju.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bl.9csxet.cn

================================================================================
来源：http://xp.hnjuh.cn

I. 正则表达式
来源：http://ea.jianghongdianzi.cn

================================================================================
来源：http://zk.hahajie.cn

[I01] 判断是否匹配
来源：http://ns.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xu.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cr.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://so.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://zw.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ia.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kx.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://xr.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gx.9csxet.cn

[I02] 提取所有匹配
来源：http://bc.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://cp.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dx.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jk.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://ne.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oo.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aa.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://ov.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zh.colortex.cn

[I03] 提取捕获分组
来源：http://xs.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fs.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pn.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nf.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ig.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pq.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://op.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yz.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fe.shtwfgs.cn

[I04] 正则替换
来源：http://rj.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xt.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cj.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://at.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://th.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ls.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sp.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zn.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hf.huanxung.cn

[I05] 按正则拆分
来源：http://nb.9csxet.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hc.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ho.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://dz.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://um.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://fn.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sr.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://eo.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mh.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ia.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://go.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kg.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kf.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ch.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lk.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vu.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yo.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://la.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://yy.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ku.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wo.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tq.hnjuh.cn

TS:   /error/gim
来源：http://ys.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ia.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wj.colortex.cn

Ruby: s.scan(/error/i)
来源：http://yn.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ox.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://wi.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hd.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cb.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ve.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ne.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ok.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ca.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aa.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hy.wgjwhj.cn

================================================================================
来源：http://wn.bookmarksfly.cn

J. 日期与时间
来源：http://lu.chemitech.net.cn

================================================================================
来源：http://cl.nicolike.cn

[J01] 获取当前时间
来源：http://gt.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uj.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pg.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://og.9csxet.cn

TS:   new Date();  Date.now()
来源：http://tu.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cx.shxzukj.cn

Go:   time.Now()
来源：http://sv.wgjwhj.cn

Ruby: Time.now
来源：http://lv.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qc.chemitech.net.cn

[J02] 格式化输出
来源：http://ct.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ov.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dz.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gp.hahajie.cn

TS:   d.toISOString()
来源：http://vp.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gg.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xc.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://go.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xu.hnjuh.cn

[J03] 字符串解析为日期
来源：http://mv.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vn.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://di.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://hc.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://sm.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tj.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rr.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://lj.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jv.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://pd.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tn.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iq.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kz.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://at.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jr.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://op.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dh.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qo.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://nn.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://wp.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hc.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://km.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fg.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://pe.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uc.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://pn.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gh.szxytkj.cn

[J06] 计算两时间之差
来源：http://wg.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://py.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://nb.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pu.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gj.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ks.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://jt.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://yg.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://rj.muxihuayi.cn

[J07] 比较两个日期
来源：http://on.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://qc.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wz.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zb.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pb.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hf.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xd.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qe.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://ib.newstarts.cn

[J08] 提取年月日与星期
来源：http://rk.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jr.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sy.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bg.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iw.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nn.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ii.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mr.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cc.bjjhwx.cn

[J09] 时区处理
来源：http://ic.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bx.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cy.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dp.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dj.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lk.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uf.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ks.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tu.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://cy.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ia.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zn.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mx.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nn.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ib.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gw.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bg.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uw.lnxyls.cn

================================================================================
来源：http://hc.shtwfgs.cn

K. JSON 与序列化
来源：http://od.gzmigu.cn

================================================================================
来源：http://gj.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://cj.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qa.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cv.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://zo.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://qf.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://my.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://vk.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xi.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ko.huanxung.cn

[K02] JSON 字符串转对象
来源：http://lw.bjjhwx.cn

Py:   json.loads(s)
来源：http://dv.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wt.asd995.cn

JS:   JSON.parse(s)
来源：http://ay.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://ro.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jw.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ql.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://xe.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cp.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://ge.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yh.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ag.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kl.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rr.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eb.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ro.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tu.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tn.asd995.cn

[K04] 读取 JSON 文件
来源：http://nl.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gj.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ba.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ka.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oa.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tl.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kh.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xt.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qi.huixiangedu.cn

[K05] 深拷贝对象
来源：http://ei.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://ba.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://cv.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://nu.shxzukj.cn

TS:   structuredClone(obj)
来源：http://ph.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oi.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zv.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ks.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bn.colortex.cn

[K06] 解析 URL 查询串
来源：http://vi.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xm.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gb.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ga.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pn.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yg.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yc.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://je.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bu.szsharing.cn

[K07] 进制转换
来源：http://cl.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ss.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hi.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kt.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vc.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yx.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lj.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ys.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ov.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://na.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://jm.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ye.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://fc.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://ss.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tv.wgjwhj.cn


<!-- 参考信息 -->