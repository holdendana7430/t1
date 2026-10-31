代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://of.asd995.cn

C#:   class MyException : Exception {}
来源：http://di.shxzukj.cn

[H05] 捕获特定类型
来源：http://ri.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://ah.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aa.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://ks.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://rh.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://ua.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ou.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://ah.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oz.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://le.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://qt.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zy.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ej.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bl.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pa.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qo.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://nk.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://dp.wgjwhj.cn

[H07] 断言
来源：http://ir.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://kk.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://zm.hahajie.cn

JS:   console.assert(x > 0);
来源：http://os.colortex.cn

TS:   console.assert(x > 0);
来源：http://ra.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://ie.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yp.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qs.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://zt.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://xu.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://hh.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://el.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://um.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zt.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ei.huixiangedu.cn

Go:   err.Error()
来源：http://qo.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://mz.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://lj.szsharing.cn

[H09] 带错误码的异常
来源：http://ss.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ce.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://os.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kl.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jx.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ti.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bf.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dc.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kw.colortex.cn

[H10] 资源自动释放
来源：http://iu.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zi.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qd.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ar.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eg.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dl.panjiajie.cn

Go:   defer f.Close()
来源：http://el.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wb.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mb.muxihuayi.cn

================================================================================
来源：http://sp.yuexingan06.cn

I. 正则表达式
来源：http://pw.asd995.cn

================================================================================
来源：http://dd.muxihuayi.cn

[I01] 判断是否匹配
来源：http://gf.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tb.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eq.asd995.cn

JS:   /\d+/.test(s)
来源：http://fx.newstarts.cn

TS:   /\d+/.test(s)
来源：http://wm.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bw.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ku.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://oy.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fj.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://en.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://yq.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://da.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ez.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://gw.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sn.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ic.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://aq.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vo.newstarts.cn

[I03] 提取捕获分组
来源：http://rh.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iv.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vl.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ea.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zf.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ef.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yr.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sc.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://js.shtwfgs.cn

[I04] 正则替换
来源：http://lu.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xq.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hk.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xt.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://un.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ky.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xh.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sg.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wf.panjiajie.cn

[I05] 按正则拆分
来源：http://jz.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yu.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ly.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://dg.hahajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://kp.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://nc.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://so.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cm.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yw.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://st.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ao.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cv.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ml.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vj.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://do.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wn.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pn.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gj.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://lj.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jp.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kr.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://px.asd995.cn

TS:   /error/gim
来源：http://hu.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gf.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pr.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://hq.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xy.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://av.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pw.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bm.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ou.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dk.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gk.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sc.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uk.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eq.colortex.cn

================================================================================
来源：http://ox.yuntaijiaju.cn

J. 日期与时间
来源：http://xm.nicolike.cn

================================================================================
来源：http://gm.521024.cn

[J01] 获取当前时间
来源：http://kx.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gc.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iw.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://pf.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://vs.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ep.jianghongdianzi.cn

Go:   time.Now()
来源：http://es.huixiangedu.cn

Ruby: Time.now
来源：http://xo.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yg.wgjwhj.cn

[J02] 格式化输出
来源：http://mo.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qq.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mr.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qc.521024.cn

TS:   d.toISOString()
来源：http://ez.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jy.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wi.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wf.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ym.asd995.cn

[J03] 字符串解析为日期
来源：http://ci.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dw.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cm.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://vp.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://qr.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cx.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zt.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://de.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mc.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://be.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rg.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://br.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lv.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ov.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ww.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jt.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bo.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wk.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://uo.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://rq.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ww.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tu.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lf.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://vo.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bo.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://ae.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zn.gzmigu.cn

[J06] 计算两时间之差
来源：http://ez.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://mu.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://nz.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ps.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gy.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://th.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://wa.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://gb.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://np.hahajie.cn

[J07] 比较两个日期
来源：http://qx.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://vr.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tw.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://um.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qb.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://br.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ky.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fo.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ww.asd995.cn

[J08] 提取年月日与星期
来源：http://sz.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lm.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bj.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hf.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://as.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ru.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vn.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vv.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tv.szsharing.cn

[J09] 时区处理
来源：http://eu.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ga.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kp.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://va.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ig.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zc.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fv.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://el.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lh.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://ko.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nu.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hg.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ij.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mn.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jr.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://on.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xk.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mj.hahajie.cn

================================================================================
来源：http://ds.szxytkj.cn

K. JSON 与序列化
来源：http://uv.shxzukj.cn

================================================================================
来源：http://bv.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://qr.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cn.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cs.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://py.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://ge.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zk.nicolike.cn

Go:   json.Marshal(obj)
来源：http://tj.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ov.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yg.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://up.bookmarksfly.cn

Py:   json.loads(s)
来源：http://xb.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pe.521024.cn

JS:   JSON.parse(s)
来源：http://mb.9csxet.cn

TS:   JSON.parse(s)
来源：http://us.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qk.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://zq.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://cl.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://if.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://il.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iy.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fk.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tg.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zv.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://so.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fr.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sr.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xf.asd995.cn

[K04] 读取 JSON 文件
来源：http://eo.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bd.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tr.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fm.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xc.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cj.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jo.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mn.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uj.wgjwhj.cn

[K05] 深拷贝对象
来源：http://da.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://ro.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://ab.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://ly.hahajie.cn

TS:   structuredClone(obj)
来源：http://pr.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gm.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jj.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ds.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pp.521024.cn

[K06] 解析 URL 查询串
来源：http://nx.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ce.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fx.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://we.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nw.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mu.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://oq.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gc.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bg.huixiangedu.cn

[K07] 进制转换
来源：http://uz.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cs.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vf.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yf.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tc.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vm.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ep.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pq.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://my.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://xr.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://ne.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ll.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://tb.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://pt.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://es.nicolike.cn

Go:   encoding/gob
来源：http://as.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://ul.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sx.haigaiapp.cn

================================================================================
来源：http://wo.jctech888.com.cn


<!-- 参考信息 -->