代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://bb.hahajie.cn

C#:   class MyException : Exception {}
来源：http://iw.nszjky.cn

[H05] 捕获特定类型
来源：http://xt.wgjwhj.cn

Py:   except ValueError as e:
来源：http://nr.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://et.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://af.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://kg.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://cy.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bg.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://ck.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://we.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://sr.hahajie.cn

Py:   value = d.get("k") or default
来源：http://se.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bi.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mn.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ts.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dx.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qg.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://oy.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://ug.hnjuh.cn

[H07] 断言
来源：http://ul.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://hz.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://bc.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://mr.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://ls.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://yz.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ak.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sh.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://hh.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://vn.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://du.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://da.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://me.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ke.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rb.lnxyls.cn

Go:   err.Error()
来源：http://jv.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://gf.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://ig.jctech888.com.cn

[H09] 带错误码的异常
来源：http://xk.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ab.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://va.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uu.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tr.asd995.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bq.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dx.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vw.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mq.newstarts.cn

[H10] 资源自动释放
来源：http://cd.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://og.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bt.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ts.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xg.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gn.newstarts.cn

Go:   defer f.Close()
来源：http://id.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uw.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gu.shtwfgs.cn

================================================================================
来源：http://jr.jctech888.com.cn

I. 正则表达式
来源：http://nh.haigaiapp.cn

================================================================================
来源：http://ly.shtwfgs.cn

[I01] 判断是否匹配
来源：http://ly.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eq.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yw.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://aj.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://fz.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bv.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mj.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://fi.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wj.wgjwhj.cn

[I02] 提取所有匹配
来源：http://re.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://am.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cu.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://si.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://ty.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xv.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cx.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://sr.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oi.huixiangedu.cn

[I03] 提取捕获分组
来源：http://ws.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hl.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ar.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bd.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bk.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cr.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qb.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ql.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ax.panjiajie.cn

[I04] 正则替换
来源：http://fd.szxytkj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rm.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zu.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ru.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xz.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fj.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bl.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vm.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ak.jctech888.com.cn

[I05] 按正则拆分
来源：http://qp.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kn.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nn.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://ka.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://ce.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://if.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ul.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yk.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nd.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gy.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gr.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vs.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nr.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://no.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jw.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dy.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hr.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zy.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://xo.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xo.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jq.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ol.nicolike.cn

TS:   /error/gim
来源：http://mb.yuexingan06.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ht.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rg.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://uq.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zg.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://hv.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ab.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cg.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ou.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mz.yuntaijiaju.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ft.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vv.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yd.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gl.nszjky.cn

================================================================================
来源：http://al.bookmarksfly.cn

J. 日期与时间
来源：http://ld.szsharing.cn

================================================================================
来源：http://ss.bjjhwx.cn

[J01] 获取当前时间
来源：http://jk.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ly.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wt.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://dx.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://oa.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ow.yuexingan06.cn

Go:   time.Now()
来源：http://wt.huanxung.cn

Ruby: Time.now
来源：http://ep.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://of.hahajie.cn

[J02] 格式化输出
来源：http://pa.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ci.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hp.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wr.szxytkj.cn

TS:   d.toISOString()
来源：http://yo.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aj.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xh.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ld.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ev.gzmigu.cn

[J03] 字符串解析为日期
来源：http://kj.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yv.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qj.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://nd.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://wl.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bw.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mx.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://dz.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ko.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://ab.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ho.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vd.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oc.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kx.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zo.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mp.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ky.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nr.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://cz.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://ax.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gn.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yr.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jt.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://ld.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mn.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://ic.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zb.huanxung.cn

[J06] 计算两时间之差
来源：http://pi.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://lo.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://xw.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wa.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sv.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ro.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://xc.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://ji.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://fv.gzmigu.cn

[J07] 比较两个日期
来源：http://xt.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://uo.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oe.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fv.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://my.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ac.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eg.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xt.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://dg.huixiangedu.cn

[J08] 提取年月日与星期
来源：http://wb.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wv.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fn.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sf.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kj.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ja.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rt.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fi.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bw.gzmigu.cn

[J09] 时区处理
来源：http://hd.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uw.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hw.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jq.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ew.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lq.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tg.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wt.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ur.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://tv.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hp.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ly.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xd.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ss.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ai.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sl.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lf.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fe.yuntaijiaju.cn

================================================================================
来源：http://yk.chemitech.net.cn

K. JSON 与序列化
来源：http://cg.huanxung.cn

================================================================================
来源：http://nw.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://lk.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lj.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ts.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://cz.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://es.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gk.newstarts.cn

Go:   json.Marshal(obj)
来源：http://zd.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ud.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dl.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://ag.muxihuayi.cn

Py:   json.loads(s)
来源：http://gw.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ht.521024.cn

JS:   JSON.parse(s)
来源：http://dw.nicolike.cn

TS:   JSON.parse(s)
来源：http://mh.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uq.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://yl.9csxet.cn

Ruby: JSON.parse(s)
来源：http://ro.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://il.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://ol.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iq.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xj.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ff.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ll.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cp.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fr.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kd.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dr.nicolike.cn

[K04] 读取 JSON 文件
来源：http://yq.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cf.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tj.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qp.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ih.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://on.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kq.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vf.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uw.yuexingan06.cn

[K05] 深拷贝对象
来源：http://rf.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://or.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://lk.shxzskj.cn

JS:   structuredClone(obj)
来源：http://zd.hnjuh.cn

TS:   structuredClone(obj)
来源：http://vd.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xa.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://va.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xa.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jp.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://uv.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qy.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vd.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vh.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wo.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://us.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://di.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yj.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vn.yuntaijiaju.cn

[K07] 进制转换
来源：http://pi.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://st.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pz.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bj.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tt.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hi.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://br.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kp.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ud.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://wh.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://af.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pe.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://uy.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://bm.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fh.huixiangedu.cn

Go:   encoding/gob
来源：http://hb.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://ea.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cv.huanxung.cn

================================================================================
来源：http://zs.nicolike.cn


<!-- 参考信息 -->