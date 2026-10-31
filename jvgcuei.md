代发 wailian999

Py:   value = d.get("k") or default
来源：http://bh.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nu.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rb.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jm.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zr.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://up.hahajie.cn

Ruby: d&.dig(:a, :b)
来源：http://ed.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://mb.colortex.cn

[H07] 断言
来源：http://ae.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://cq.colortex.cn

PHP:  assert($x > 0);
来源：http://ln.chemitech.net.cn

JS:   console.assert(x > 0);
来源：http://jf.newstarts.cn

TS:   console.assert(x > 0);
来源：http://hv.nicolike.cn

Java: assert x > 0 : "必须为正";
来源：http://gy.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vz.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kh.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://qt.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://av.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://fe.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sh.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://fx.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ca.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ct.jianghongdianzi.cn

Go:   err.Error()
来源：http://ca.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://rh.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://kq.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://ww.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kr.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hu.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wr.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://um.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lk.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xn.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dp.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dh.gzmigu.cn

[H10] 资源自动释放
来源：http://cs.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pg.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ez.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oq.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fg.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oy.521024.cn

Go:   defer f.Close()
来源：http://aq.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bm.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://js.huixiangedu.cn

================================================================================
来源：http://gf.haigaiapp.cn

I. 正则表达式
来源：http://ot.huixinmuqiang.cn

================================================================================
来源：http://lt.haigaiapp.cn

[I01] 判断是否匹配
来源：http://hc.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://io.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nr.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://tq.colortex.cn

TS:   /\d+/.test(s)
来源：http://qk.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qf.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ou.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://ci.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lg.shtwfgs.cn

[I02] 提取所有匹配
来源：http://pp.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://yk.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sn.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vz.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://ki.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pv.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kc.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://xg.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xx.lnxyls.cn

[I03] 提取捕获分组
来源：http://al.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pg.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lg.haigaiapp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oo.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ie.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xu.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mm.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gq.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yx.hnjuh.cn

[I04] 正则替换
来源：http://bd.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ue.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lg.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jy.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cl.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gr.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hc.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://td.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ll.521024.cn

[I05] 按正则拆分
来源：http://ed.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dc.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gd.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://ni.lnxyls.cn

TS:   s.split(/\s*,\s*/)
来源：http://ki.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://dd.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ol.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bo.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://br.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ty.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gv.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cj.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bn.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vr.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ik.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jz.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kk.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cc.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://zj.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jl.colortex.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oa.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zr.haigaiapp.cn

TS:   /error/gim
来源：http://ze.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://et.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ik.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://ch.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rg.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://lb.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pp.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ys.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zf.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oz.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ft.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cm.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ll.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yq.muxihuayi.cn

================================================================================
来源：http://js.chemitech.net.cn

J. 日期与时间
来源：http://cx.yuexingan06.cn

================================================================================
来源：http://rq.asd995.cn

[J01] 获取当前时间
来源：http://mw.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xy.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aa.hahajie.cn

JS:   new Date();  Date.now()
来源：http://dm.newstarts.cn

TS:   new Date();  Date.now()
来源：http://ta.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vg.bjjhwx.cn

Go:   time.Now()
来源：http://sz.wgjwhj.cn

Ruby: Time.now
来源：http://da.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cr.haigaiapp.cn

[J02] 格式化输出
来源：http://dy.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fi.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fa.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://at.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://mf.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ve.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dq.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ew.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gu.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://we.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ft.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vo.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://li.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://bt.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rg.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ss.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://oe.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gy.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://zl.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rz.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xb.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oj.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yl.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fq.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jo.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ba.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ee.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://kj.asd995.cn

Py:   now + timedelta(days=7)
来源：http://au.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cc.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ab.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vo.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://pv.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vi.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://af.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zi.chemitech.net.cn

[J06] 计算两时间之差
来源：http://qe.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://sy.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://wm.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mv.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eg.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zs.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://os.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://qk.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://fg.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://oi.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://sj.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://us.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wv.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bi.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ed.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kv.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kp.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://gf.szxytkj.cn

[J08] 提取年月日与星期
来源：http://xj.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ij.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qt.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ti.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://il.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pw.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://va.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mf.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xi.szxytkj.cn

[J09] 时区处理
来源：http://tb.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://on.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iq.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wb.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nh.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zd.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hn.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lb.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vi.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://cm.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hb.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qx.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cn.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nj.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xa.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fs.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zm.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hc.yuexingan06.cn

================================================================================
来源：http://ou.huanxung.cn

K. JSON 与序列化
来源：http://cy.newstarts.cn

================================================================================
来源：http://hu.521024.cn

[K01] 对象转 JSON 字符串
来源：http://hp.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bt.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://da.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://xu.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://eb.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wh.asd995.cn

Go:   json.Marshal(obj)
来源：http://xl.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ou.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pp.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://uo.9csxet.cn

Py:   json.loads(s)
来源：http://ga.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fr.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://me.shxzskj.cn

TS:   JSON.parse(s)
来源：http://of.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oy.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://yn.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://dl.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ah.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://us.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nu.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mt.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ze.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://su.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ta.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pu.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://el.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ed.newstarts.cn

[K04] 读取 JSON 文件
来源：http://rz.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rm.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ze.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lh.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eb.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tg.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xy.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ix.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://he.asd995.cn

[K05] 深拷贝对象
来源：http://ni.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://bh.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://db.521024.cn

JS:   structuredClone(obj)
来源：http://mt.panjiajie.cn

TS:   structuredClone(obj)
来源：http://tj.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ec.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wf.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zf.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hb.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://ut.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vj.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ou.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qu.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://my.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://el.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ni.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yu.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ke.hahajie.cn

[K07] 进制转换
来源：http://gr.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ag.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pn.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jg.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bn.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qi.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sb.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ew.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://um.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://al.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://dh.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mc.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://ml.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://cp.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xb.wgjwhj.cn

Go:   encoding/gob
来源：http://aj.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://kw.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vv.panjiajie.cn

================================================================================
来源：http://ot.huixinmuqiang.cn

L. 网络请求
来源：http://uy.gzmigu.cn

================================================================================
来源：http://bv.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://rh.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eg.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://si.gzmigu.cn

JS:   await fetch(url)
来源：http://bc.hnjuh.cn

TS:   await fetch(url)
来源：http://jg.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://us.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://hg.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gp.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ak.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://mm.nszjky.cn


<!-- 参考信息 -->