代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://et.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://pr.yuexingan06.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://es.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://wj.newstarts.cn

Py:   value = d.get("k") or default
来源：http://kx.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qy.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ew.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hg.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rn.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://og.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://cg.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://bs.9csxet.cn

[H07] 断言
来源：http://ee.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://uc.hnjuh.cn

PHP:  assert($x > 0);
来源：http://bo.hahajie.cn

JS:   console.assert(x > 0);
来源：http://zi.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://sa.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://to.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rb.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jl.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://na.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://ww.yuexingan06.cn

Py:   str(e);  traceback.format_exc()
来源：http://eb.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uw.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://sq.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pr.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tm.szxytkj.cn

Go:   err.Error()
来源：http://qm.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://di.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://vv.szxytkj.cn

[H09] 带错误码的异常
来源：http://sx.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wu.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tq.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vp.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xf.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uq.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ip.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ay.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gs.lnxyls.cn

[H10] 资源自动释放
来源：http://ay.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vw.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fz.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hp.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jk.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bz.szxytkj.cn

Go:   defer f.Close()
来源：http://df.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kp.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://la.newstarts.cn

================================================================================
来源：http://xn.yuntaijiaju.cn

I. 正则表达式
来源：http://uh.panjiajie.cn

================================================================================
来源：http://ic.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://cw.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ah.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xt.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://mj.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://sv.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dy.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yd.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://sr.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ft.chemitech.net.cn

[I02] 提取所有匹配
来源：http://ur.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://rr.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nu.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ug.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://mb.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cq.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cn.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://kv.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://as.colortex.cn

[I03] 提取捕获分组
来源：http://fg.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xo.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mj.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ua.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bu.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ec.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mh.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ta.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ir.panjiajie.cn

[I04] 正则替换
来源：http://ly.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ym.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dz.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nl.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tq.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vb.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ab.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bl.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yp.asd995.cn

[I05] 按正则拆分
来源：http://vq.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kv.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lp.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://nn.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://bu.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://da.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://of.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mx.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rl.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ib.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pe.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dg.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mx.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wh.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cc.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ah.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vt.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ts.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://re.szxytkj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jm.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rq.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ss.haigaiapp.cn

TS:   /error/gim
来源：http://jb.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ul.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ny.asd995.cn

Ruby: s.scan(/error/i)
来源：http://ob.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://he.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://un.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xo.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ee.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jb.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rv.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nz.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ug.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://do.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wf.muxihuayi.cn

================================================================================
来源：http://tt.hahajie.cn

J. 日期与时间
来源：http://pa.huixinmuqiang.cn

================================================================================
来源：http://gc.lnxyls.cn

[J01] 获取当前时间
来源：http://sj.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vc.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sm.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://lg.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://lr.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ge.shxzukj.cn

Go:   time.Now()
来源：http://ch.jctech888.com.cn

Ruby: Time.now
来源：http://zx.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tt.szxytkj.cn

[J02] 格式化输出
来源：http://lz.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gu.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ps.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vc.panjiajie.cn

TS:   d.toISOString()
来源：http://mt.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://de.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dz.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nt.wgjwhj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://co.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://tr.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xg.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wo.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://xx.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://ag.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rq.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qx.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ob.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nt.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://gz.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pd.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ku.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xm.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hk.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dc.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vu.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fc.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ev.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://am.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://ov.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lp.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qn.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://an.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://hk.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oy.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://sm.szsharing.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pi.panjiajie.cn

[J06] 计算两时间之差
来源：http://zq.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://tj.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://dx.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yr.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zw.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qt.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://xw.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://mf.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://ny.wgjwhj.cn

[J07] 比较两个日期
来源：http://ya.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://sh.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hc.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yo.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hd.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cj.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vz.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sj.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://zs.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://su.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://me.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qa.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://za.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mp.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vd.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oq.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sf.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tk.szxytkj.cn

[J09] 时区处理
来源：http://kl.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sl.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xa.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bg.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sm.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://si.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zw.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pd.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ij.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://xh.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://to.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://io.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yk.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mx.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cb.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ii.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ok.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kv.yuntaijiaju.cn

================================================================================
来源：http://vr.muxihuayi.cn

K. JSON 与序列化
来源：http://wz.nicolike.cn

================================================================================
来源：http://gi.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://xy.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bz.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uw.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://ag.colortex.cn

TS:   JSON.stringify(obj)
来源：http://pp.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fj.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://gc.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dx.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yu.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://uy.gzmigu.cn

Py:   json.loads(s)
来源：http://de.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qj.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://vw.hahajie.cn

TS:   JSON.parse(s)
来源：http://vm.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://km.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://rf.hahajie.cn

Ruby: JSON.parse(s)
来源：http://dq.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ch.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://kj.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dd.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ry.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ch.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yq.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xo.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vz.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xk.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ya.szsharing.cn

[K04] 读取 JSON 文件
来源：http://lv.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oc.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uc.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ij.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xp.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://av.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qj.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kv.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tw.shxzukj.cn

[K05] 深拷贝对象
来源：http://yb.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://cf.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://ni.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://kp.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://eh.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kh.hnjuh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cy.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ie.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://al.asd995.cn

[K06] 解析 URL 查询串
来源：http://bq.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ad.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ds.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wn.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cz.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dx.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sx.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hn.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xe.newstarts.cn

[K07] 进制转换
来源：http://nq.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qs.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ut.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sm.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://id.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vo.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zz.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eb.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yx.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://qo.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://ho.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yy.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://qh.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://et.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ee.yuntaijiaju.cn

Go:   encoding/gob
来源：http://lm.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://el.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gj.shxzukj.cn

================================================================================
来源：http://tp.jianghongdianzi.cn

L. 网络请求
来源：http://tp.huixinmuqiang.cn

================================================================================
来源：http://fk.newstarts.cn

[L01] 发送 GET 请求
来源：http://fc.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wy.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yr.chemitech.net.cn

JS:   await fetch(url)
来源：http://yy.nszjky.cn

TS:   await fetch(url)
来源：http://ti.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fi.chemitech.net.cn


<!-- 参考信息 -->