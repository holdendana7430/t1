代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://qs.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://fx.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://em.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jm.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://ks.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yh.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tb.colortex.cn

Go:   err.Error()
来源：http://dn.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://tx.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://jw.wgjwhj.cn

[H09] 带错误码的异常
来源：http://jr.shtwfgs.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ow.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hv.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pt.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gy.szsharing.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ov.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kw.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ez.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ax.yuexingan06.cn

[H10] 资源自动释放
来源：http://br.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sk.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qv.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qt.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ht.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eu.yuexingan06.cn

Go:   defer f.Close()
来源：http://hb.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nu.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pk.lnxyls.cn

================================================================================
来源：http://pn.gzmigu.cn

I. 正则表达式
来源：http://mi.muxihuayi.cn

================================================================================
来源：http://dn.lnxyls.cn

[I01] 判断是否匹配
来源：http://ax.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yi.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qy.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://rb.szsharing.cn

TS:   /\d+/.test(s)
来源：http://bl.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oq.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aw.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://tx.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ou.chemitech.net.cn

[I02] 提取所有匹配
来源：http://ob.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://rg.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://em.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zd.521024.cn

TS:   s.match(/\d+/g)
来源：http://bq.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mk.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fo.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://mp.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qe.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://ph.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dd.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ul.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uv.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rz.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sd.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://of.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://np.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ws.szsharing.cn

[I04] 正则替换
来源：http://kk.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oi.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ow.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qm.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kx.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://em.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://iv.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fo.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vr.nszjky.cn

[I05] 按正则拆分
来源：http://ay.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sg.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ej.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://og.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://zb.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://he.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qs.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qc.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wk.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xl.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eo.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pg.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gq.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ll.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fd.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bn.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ap.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://la.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://ni.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://px.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mr.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://da.bjjhwx.cn

TS:   /error/gim
来源：http://av.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tq.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ej.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://ge.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ft.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://rq.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hm.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://em.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zi.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vv.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://la.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ib.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ku.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nq.szxytkj.cn

================================================================================
来源：http://ev.szsharing.cn

J. 日期与时间
来源：http://pa.shtwfgs.cn

================================================================================
来源：http://is.hahajie.cn

[J01] 获取当前时间
来源：http://zj.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fh.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qy.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://qh.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://pz.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ed.hnjuh.cn

Go:   time.Now()
来源：http://iw.jianghongdianzi.cn

Ruby: Time.now
来源：http://lr.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yf.haigaiapp.cn

[J02] 格式化输出
来源：http://zr.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://om.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jo.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vl.huixiangedu.cn

TS:   d.toISOString()
来源：http://pg.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vk.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ul.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://va.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kl.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://em.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dj.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aw.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://gw.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://sj.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ju.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pi.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://vc.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hy.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://qk.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uw.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://st.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tr.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vs.9csxet.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yo.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ad.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tn.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ph.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://vq.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://pg.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dc.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eg.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ru.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://im.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bs.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://gg.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://eu.shxzskj.cn

[J06] 计算两时间之差
来源：http://et.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://fa.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://ap.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eu.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tm.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zp.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://xc.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://xk.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://jo.asd995.cn

[J07] 比较两个日期
来源：http://sp.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://sk.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tl.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dx.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://md.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sv.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jf.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qy.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://xt.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://oz.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oh.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xu.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zj.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vb.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bl.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ji.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://su.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tp.yuexingan06.cn

[J09] 时区处理
来源：http://tu.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://we.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yt.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ms.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ql.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ba.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dj.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vm.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ih.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://hc.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ai.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nl.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nl.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cm.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tl.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://it.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vn.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gp.huixinmuqiang.cn

================================================================================
来源：http://pt.gzmigu.cn

K. JSON 与序列化
来源：http://fd.wgjwhj.cn

================================================================================
来源：http://qa.521024.cn

[K01] 对象转 JSON 字符串
来源：http://il.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fo.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rg.asd995.cn

JS:   JSON.stringify(obj)
来源：http://by.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://zb.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jl.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://ul.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lp.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bs.asd995.cn

[K02] JSON 字符串转对象
来源：http://nq.hahajie.cn

Py:   json.loads(s)
来源：http://rv.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sz.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://et.szsharing.cn

TS:   JSON.parse(s)
来源：http://or.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ub.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://wr.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://xo.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eg.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://gf.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vh.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://px.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bq.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ax.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tl.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://aj.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ds.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jz.521024.cn

[K04] 读取 JSON 文件
来源：http://pv.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vv.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yl.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zg.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kg.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ue.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ck.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vp.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zv.521024.cn

[K05] 深拷贝对象
来源：http://af.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://gm.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://gd.521024.cn

JS:   structuredClone(obj)
来源：http://la.gzmigu.cn

TS:   structuredClone(obj)
来源：http://dh.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://au.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lf.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kl.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://go.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://og.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lz.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jx.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lb.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://in.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fi.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rf.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://it.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dp.huixiangedu.cn

[K07] 进制转换
来源：http://xy.panjiajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://du.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jm.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cl.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sf.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://en.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bv.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://si.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tx.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://vc.bjjhwx.cn

Py:   pickle.dumps(obj)
来源：http://ec.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dh.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://yl.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://vx.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dq.bookmarksfly.cn

Go:   encoding/gob
来源：http://zl.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://lu.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hr.bookmarksfly.cn

================================================================================
来源：http://jr.huixiangedu.cn

L. 网络请求
来源：http://lk.yuexingan06.cn

================================================================================
来源：http://hh.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://df.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yn.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wa.hnjuh.cn

JS:   await fetch(url)
来源：http://ng.huanxung.cn

TS:   await fetch(url)
来源：http://pl.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lx.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://ei.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sg.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ct.newstarts.cn

[L02] 发送 POST JSON
来源：http://te.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rs.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jo.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xy.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jm.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hv.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ye.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sn.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mj.szsharing.cn

[L03] 设置自定义请求头
来源：http://dc.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ie.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sw.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hh.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tn.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wk.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ge.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xw.newstarts.cn


<!-- 参考信息 -->