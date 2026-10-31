代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kx.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://ta.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mp.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://dl.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://dn.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dr.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nl.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qn.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qp.chemitech.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vv.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://yw.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://yu.shxzskj.cn

[H07] 断言
来源：http://zl.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://qo.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://gu.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://nz.hahajie.cn

TS:   console.assert(x > 0);
来源：http://tn.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://xx.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sw.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ah.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://lc.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://yl.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://eo.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wt.panjiajie.cn

JS:   e.message;  e.stack
来源：http://tb.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ti.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ri.gzmigu.cn

Go:   err.Error()
来源：http://wy.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://ja.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://rn.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://uc.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ro.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yd.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pe.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ux.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hp.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ps.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://th.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nt.shtwfgs.cn

[H10] 资源自动释放
来源：http://yl.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ob.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iq.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mc.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://df.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fe.nszjky.cn

Go:   defer f.Close()
来源：http://rg.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ax.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sc.newstarts.cn

================================================================================
来源：http://bm.nicolike.cn

I. 正则表达式
来源：http://gy.huixiangedu.cn

================================================================================
来源：http://dl.panjiajie.cn

[I01] 判断是否匹配
来源：http://vl.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hu.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cy.colortex.cn

JS:   /\d+/.test(s)
来源：http://ma.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://zc.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xr.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gs.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://ae.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sy.hahajie.cn

[I02] 提取所有匹配
来源：http://hk.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://ml.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://st.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vo.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://oh.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tl.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hp.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://ld.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ho.wgjwhj.cn

[I03] 提取捕获分组
来源：http://zh.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gm.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qc.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yn.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qn.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yz.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kx.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ik.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sd.521024.cn

[I04] 正则替换
来源：http://rp.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://aa.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://px.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ie.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zq.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://do.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uu.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://li.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nu.nszjky.cn

[I05] 按正则拆分
来源：http://oh.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bc.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gn.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://cs.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://hl.nicolike.cn

Java: s.split("\\s*,\\s*")
来源：http://tl.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qo.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qt.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hx.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hr.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pl.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://av.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qq.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nj.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qx.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jp.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ro.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ok.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://fu.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vm.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rr.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nb.szxytkj.cn

TS:   /error/gim
来源：http://nf.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ee.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pn.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://sn.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pa.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://ac.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ch.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dz.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ck.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wz.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dw.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hp.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ih.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oe.521024.cn

================================================================================
来源：http://cr.panjiajie.cn

J. 日期与时间
来源：http://nl.521024.cn

================================================================================
来源：http://uj.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://he.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://aj.jctech888.com.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ak.hahajie.cn

JS:   new Date();  Date.now()
来源：http://zn.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://yk.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://br.panjiajie.cn

Go:   time.Now()
来源：http://mw.jianghongdianzi.cn

Ruby: Time.now
来源：http://ap.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sl.yuntaijiaju.cn

[J02] 格式化输出
来源：http://po.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ut.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dm.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jk.shxzskj.cn

TS:   d.toISOString()
来源：http://ki.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fa.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tf.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vm.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vr.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://pp.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ms.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uj.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://kt.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://ja.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ur.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ig.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://sa.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lf.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://qh.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://if.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rp.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hr.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gz.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ic.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rs.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xg.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nj.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://qv.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://sa.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ru.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vg.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ti.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://hv.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fs.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://tj.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nm.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://ww.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://dh.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://sa.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xt.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xe.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jw.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://fr.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://gg.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://lg.huixiangedu.cn

[J07] 比较两个日期
来源：http://in.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://sz.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oy.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://il.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gv.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ae.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://le.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lh.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://kw.lnxyls.cn

[J08] 提取年月日与星期
来源：http://yr.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ky.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ao.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fy.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pm.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bg.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hu.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://il.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zi.muxihuayi.cn

[J09] 时区处理
来源：http://yi.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jn.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gn.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rh.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cj.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cd.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sh.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://to.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://po.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://hm.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://df.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pm.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rk.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nw.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ms.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://im.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://le.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nh.hnjuh.cn

================================================================================
来源：http://ju.hahajie.cn

K. JSON 与序列化
来源：http://ne.haigaiapp.cn

================================================================================
来源：http://oi.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://vb.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pi.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qn.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://hf.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://av.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nd.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://qs.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qy.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tn.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://bl.chemitech.net.cn

Py:   json.loads(s)
来源：http://su.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rm.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://tu.shxzskj.cn

TS:   JSON.parse(s)
来源：http://un.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bu.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://em.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://nj.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jd.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://cu.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qu.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tu.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oa.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zn.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zv.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ar.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xp.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yu.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://jh.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ox.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vd.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xe.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://no.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jf.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kd.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lv.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tx.hahajie.cn

[K05] 深拷贝对象
来源：http://kx.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://qz.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://hw.colortex.cn

JS:   structuredClone(obj)
来源：http://vf.nicolike.cn

TS:   structuredClone(obj)
来源：http://ex.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ki.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iw.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pn.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ra.nszjky.cn

[K06] 解析 URL 查询串
来源：http://wl.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dc.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ye.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xf.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xo.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sc.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bw.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ku.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kp.huanxung.cn

[K07] 进制转换
来源：http://jf.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ii.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fl.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zh.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ss.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ei.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pa.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mk.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tg.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://yz.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://yv.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gz.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://vn.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://dl.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jr.hnjuh.cn

Go:   encoding/gob
来源：http://xq.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://lf.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zd.bookmarksfly.cn

================================================================================
来源：http://mf.bjjhwx.cn

L. 网络请求
来源：http://vn.colortex.cn

================================================================================
来源：http://qu.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://qn.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fd.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sd.hnjuh.cn

JS:   await fetch(url)
来源：http://jm.521024.cn

TS:   await fetch(url)
来源：http://yt.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ey.szxytkj.cn


<!-- 参考信息 -->