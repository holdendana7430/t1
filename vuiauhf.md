代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bo.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sn.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://gm.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://aj.huixinmuqiang.cn

[H07] 断言
来源：http://nc.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://ce.hahajie.cn

PHP:  assert($x > 0);
来源：http://gg.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://eo.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://bp.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://fp.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pc.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jd.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://vz.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://ry.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://qr.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yw.shxzskj.cn

JS:   e.message;  e.stack
来源：http://ip.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tg.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uo.newstarts.cn

Go:   err.Error()
来源：http://sz.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://fj.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://rt.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://wy.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ff.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yq.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fj.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tv.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zm.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yl.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ts.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wf.huixinmuqiang.cn

[H10] 资源自动释放
来源：http://he.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hp.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gs.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fr.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://so.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rq.jctech888.com.cn

Go:   defer f.Close()
来源：http://al.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zs.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hp.bookmarksfly.cn

================================================================================
来源：http://ek.521024.cn

I. 正则表达式
来源：http://tk.jctech888.com.cn

================================================================================
来源：http://gt.shtwfgs.cn

[I01] 判断是否匹配
来源：http://ds.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xp.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ji.szsharing.cn

JS:   /\d+/.test(s)
来源：http://uj.huixiangedu.cn

TS:   /\d+/.test(s)
来源：http://jq.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gk.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oj.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://gp.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lr.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://ty.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://dt.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uq.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://we.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://nr.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bh.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hb.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://ti.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wf.shxzukj.cn

[I03] 提取捕获分组
来源：http://pq.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ju.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zo.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hr.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dn.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cl.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jn.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cb.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vj.hnjuh.cn

[I04] 正则替换
来源：http://sv.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://la.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vc.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yg.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zy.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dd.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oc.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xk.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://le.wgjwhj.cn

[I05] 按正则拆分
来源：http://im.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rr.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tq.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://gj.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://fk.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://uv.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sh.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vw.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bn.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ic.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fh.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://di.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rp.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jd.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qz.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lk.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yi.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cy.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://oj.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ou.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://om.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ix.szsharing.cn

TS:   /error/gim
来源：http://ig.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hq.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pu.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://np.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sw.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://zr.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pc.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ni.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://of.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yn.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zn.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ny.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fn.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hv.shxzskj.cn

================================================================================
来源：http://zi.newstarts.cn

J. 日期与时间
来源：http://er.szsharing.cn

================================================================================
来源：http://xu.chemitech.net.cn

[J01] 获取当前时间
来源：http://pk.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://og.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rn.huanxung.cn

JS:   new Date();  Date.now()
来源：http://yv.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://ab.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cb.chemitech.net.cn

Go:   time.Now()
来源：http://xi.bjjhwx.cn

Ruby: Time.now
来源：http://gf.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rh.9csxet.cn

[J02] 格式化输出
来源：http://vh.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nw.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ic.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xs.asd995.cn

TS:   d.toISOString()
来源：http://bm.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sx.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ru.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hi.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yd.szsharing.cn

[J03] 字符串解析为日期
来源：http://xo.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ta.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qf.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://sx.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://dq.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ft.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ji.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://yn.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fa.9csxet.cn

[J04] 时间戳与日期互转
来源：http://jn.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eb.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tk.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ic.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kd.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ea.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oa.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iv.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fg.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://gd.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://uo.jianghongdianzi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rl.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kp.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xt.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://oq.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pg.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://nc.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jf.bjjhwx.cn

[J06] 计算两时间之差
来源：http://mj.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://xx.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://bt.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://br.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vw.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mg.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://nd.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://jx.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://gb.huanxung.cn

[J07] 比较两个日期
来源：http://zl.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://jh.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pi.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cd.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://eg.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rx.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tw.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ks.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://ne.huixiangedu.cn

[J08] 提取年月日与星期
来源：http://ry.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ip.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sq.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hx.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pq.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://af.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tx.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://os.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ho.huixiangedu.cn

[J09] 时区处理
来源：http://pe.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ft.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xe.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lx.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cl.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vv.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ei.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://su.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yo.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://xw.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vn.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yi.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vh.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pp.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ou.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://br.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xu.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iy.chemitech.net.cn

================================================================================
来源：http://kz.yuntaijiaju.cn

K. JSON 与序列化
来源：http://yx.huanxung.cn

================================================================================
来源：http://ra.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://yi.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gg.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vz.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://qw.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://rv.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gn.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://oq.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mz.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qf.colortex.cn

[K02] JSON 字符串转对象
来源：http://us.newstarts.cn

Py:   json.loads(s)
来源：http://yw.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ji.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://po.nszjky.cn

TS:   JSON.parse(s)
来源：http://il.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ba.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://bl.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://kt.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ss.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://hs.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lx.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nf.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dg.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ki.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cc.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vu.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qi.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lk.nicolike.cn

[K04] 读取 JSON 文件
来源：http://wm.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://df.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uu.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ft.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qw.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://af.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ha.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yb.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://an.bjjhwx.cn

[K05] 深拷贝对象
来源：http://kd.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://gn.lnxyls.cn

PHP:  unserialize(serialize($obj));
来源：http://ff.nszjky.cn

JS:   structuredClone(obj)
来源：http://xd.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://yn.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qv.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ry.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nh.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vy.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://fc.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sc.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xc.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ov.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fg.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xk.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ue.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fx.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ng.shxzukj.cn

[K07] 进制转换
来源：http://yk.shxzskj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nw.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://en.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sa.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qd.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vc.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yk.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ig.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tm.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://gi.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://tu.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://be.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://fo.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ru.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uv.colortex.cn

Go:   encoding/gob
来源：http://pn.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://qt.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vc.shxzukj.cn

================================================================================
来源：http://dc.jctech888.com.cn

L. 网络请求
来源：http://qm.colortex.cn

================================================================================
来源：http://cr.gzmigu.cn

[L01] 发送 GET 请求
来源：http://zq.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lw.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yp.hnjuh.cn

JS:   await fetch(url)
来源：http://jh.yuexingan06.cn

TS:   await fetch(url)
来源：http://fb.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sx.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://wh.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://de.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gx.huanxung.cn

[L02] 发送 POST JSON
来源：http://qk.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://un.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://os.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vx.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yj.huixinmuqiang.cn


<!-- 参考信息 -->