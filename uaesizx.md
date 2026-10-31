代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nz.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oz.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://pk.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://sw.shtwfgs.cn

[H07] 断言
来源：http://vr.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://od.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://if.nicolike.cn

JS:   console.assert(x > 0);
来源：http://af.szsharing.cn

TS:   console.assert(x > 0);
来源：http://om.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://md.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qt.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dr.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://kh.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://xv.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://id.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wi.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://ic.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ge.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zd.shtwfgs.cn

Go:   err.Error()
来源：http://os.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://cu.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://kk.shxzukj.cn

[H09] 带错误码的异常
来源：http://cl.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uy.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fr.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sq.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://at.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gz.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://si.9csxet.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yv.gzmigu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yo.chemitech.net.cn

[H10] 资源自动释放
来源：http://uz.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pt.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ji.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ey.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oy.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eg.muxihuayi.cn

Go:   defer f.Close()
来源：http://mk.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ka.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://md.szsharing.cn

================================================================================
来源：http://vc.asd995.cn

I. 正则表达式
来源：http://vm.haigaiapp.cn

================================================================================
来源：http://lk.panjiajie.cn

[I01] 判断是否匹配
来源：http://un.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://py.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://il.shtwfgs.cn

JS:   /\d+/.test(s)
来源：http://ku.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://zm.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ht.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nm.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://hv.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ua.szsharing.cn

[I02] 提取所有匹配
来源：http://zv.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://hn.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bq.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hu.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://mu.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mn.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fq.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://pv.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zq.521024.cn

[I03] 提取捕获分组
来源：http://vf.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://en.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tg.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eh.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://en.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fi.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bp.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://na.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ec.shxzukj.cn

[I04] 正则替换
来源：http://uo.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wd.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pr.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hn.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uh.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kl.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tw.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jq.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xk.nszjky.cn

[I05] 按正则拆分
来源：http://rr.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ae.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ku.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://ul.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://vc.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://qt.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://by.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ed.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://md.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://om.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ts.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rd.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yw.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qc.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xn.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ee.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mc.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wx.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://ls.huanxung.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lu.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qp.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gh.newstarts.cn

TS:   /error/gim
来源：http://hf.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://se.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pl.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://li.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jj.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://xt.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bn.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kp.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pv.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ep.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mc.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gp.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sv.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://di.bjjhwx.cn

================================================================================
来源：http://td.lnxyls.cn

J. 日期与时间
来源：http://lz.panjiajie.cn

================================================================================
来源：http://tz.yuexingan06.cn

[J01] 获取当前时间
来源：http://th.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yh.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nb.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://ql.newstarts.cn

TS:   new Date();  Date.now()
来源：http://la.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ov.chemitech.net.cn

Go:   time.Now()
来源：http://ld.huixiangedu.cn

Ruby: Time.now
来源：http://qy.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lx.lnxyls.cn

[J02] 格式化输出
来源：http://iw.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xn.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ae.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://on.huanxung.cn

TS:   d.toISOString()
来源：http://xy.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rh.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rd.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://be.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yf.szsharing.cn

[J03] 字符串解析为日期
来源：http://hj.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qk.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bd.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://ba.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://ak.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jl.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wi.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://sz.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tq.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://lw.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://um.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ht.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://la.lnxyls.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qa.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zg.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kv.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oi.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ba.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://jj.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://dq.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gm.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qk.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qu.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://qi.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xr.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://tg.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://up.asd995.cn

[J06] 计算两时间之差
来源：http://hs.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://ck.521024.cn

PHP:  $end->diff($start)->days;
来源：http://ws.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nb.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qz.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rp.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://bb.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://bt.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://bi.panjiajie.cn

[J07] 比较两个日期
来源：http://fz.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://qv.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fw.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dc.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ec.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kb.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zl.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xi.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://au.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://cw.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yt.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gn.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://be.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ji.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uy.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ty.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qh.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ru.bjjhwx.cn

[J09] 时区处理
来源：http://ii.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zz.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ha.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ue.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hj.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xq.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tc.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lb.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lo.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://ta.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fg.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ar.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://da.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fj.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tw.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qn.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uy.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hr.9csxet.cn

================================================================================
来源：http://rm.colortex.cn

K. JSON 与序列化
来源：http://ct.colortex.cn

================================================================================
来源：http://kv.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://my.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tj.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xq.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://vn.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://ew.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ej.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://cu.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vh.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xt.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://wd.lnxyls.cn

Py:   json.loads(s)
来源：http://px.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hv.nszjky.cn

JS:   JSON.parse(s)
来源：http://eu.huanxung.cn

TS:   JSON.parse(s)
来源：http://sb.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ri.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://rz.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://bb.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fd.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://yz.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ap.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ge.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://co.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gg.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oz.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lc.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gj.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qr.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://dy.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rk.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ql.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iy.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iy.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://au.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gk.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://eo.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xy.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://fz.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://fc.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://rl.huanxung.cn

JS:   structuredClone(obj)
来源：http://yv.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://ud.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zd.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fz.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jf.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://le.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://uu.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zb.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kq.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gf.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sq.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ra.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nw.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sj.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vp.9csxet.cn

[K07] 进制转换
来源：http://zq.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rr.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vr.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uv.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://og.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bb.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iw.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uf.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://or.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://rv.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://cf.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bm.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://by.hahajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://js.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ou.bjjhwx.cn

Go:   encoding/gob
来源：http://ek.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://ej.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zv.9csxet.cn

================================================================================
来源：http://mh.shtwfgs.cn

L. 网络请求
来源：http://em.hnjuh.cn

================================================================================
来源：http://ga.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://zu.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cb.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dl.asd995.cn

JS:   await fetch(url)
来源：http://wx.shxzskj.cn

TS:   await fetch(url)
来源：http://ab.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tp.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://bo.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ok.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://me.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://ac.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yh.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mf.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hh.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nl.bjjhwx.cn


<!-- 参考信息 -->