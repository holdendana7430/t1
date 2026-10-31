代发 wailian999

JS:   e.message;  e.stack
来源：http://az.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sy.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zh.hnjuh.cn

Go:   err.Error()
来源：http://fv.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://qt.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://cq.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://bs.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bs.yuexingan06.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ye.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://of.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wz.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yg.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kw.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cc.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xw.shxzskj.cn

[H10] 资源自动释放
来源：http://vc.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sw.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sl.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uc.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jv.shxzskj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gw.wgjwhj.cn

Go:   defer f.Close()
来源：http://no.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://an.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wp.yuexingan06.cn

================================================================================
来源：http://yx.hahajie.cn

I. 正则表达式
来源：http://db.chemitech.net.cn

================================================================================
来源：http://gw.hahajie.cn

[I01] 判断是否匹配
来源：http://kp.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qt.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ca.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://eu.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://gf.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gm.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ua.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://tc.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uc.bjjhwx.cn

[I02] 提取所有匹配
来源：http://bk.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://wi.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nn.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hq.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://gw.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xn.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ke.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://ng.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xr.hnjuh.cn

[I03] 提取捕获分组
来源：http://sx.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sq.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ie.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sd.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://al.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dn.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zu.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ja.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vn.huixinmuqiang.cn

[I04] 正则替换
来源：http://ze.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kg.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tp.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ev.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cf.haigaiapp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://px.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://og.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ux.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vp.huanxung.cn

[I05] 按正则拆分
来源：http://nq.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qf.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wb.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://eh.chemitech.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://tr.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://jl.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fu.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lj.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fi.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jd.hnjuh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ts.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bp.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xl.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sf.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qd.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://el.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jh.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xv.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://ja.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ud.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://st.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ac.haigaiapp.cn

TS:   /error/gim
来源：http://ac.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ye.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://af.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://yo.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vr.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://ff.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lc.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://av.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jz.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wr.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bb.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://js.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dt.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zd.hahajie.cn

================================================================================
来源：http://fz.jianghongdianzi.cn

J. 日期与时间
来源：http://bh.shxzukj.cn

================================================================================
来源：http://yv.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://iv.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://li.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ad.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://hp.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://jk.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ky.bookmarksfly.cn

Go:   time.Now()
来源：http://uj.lnxyls.cn

Ruby: Time.now
来源：http://po.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://er.asd995.cn

[J02] 格式化输出
来源：http://nb.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jp.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gt.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sh.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://au.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vu.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sc.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vv.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ko.newstarts.cn

[J03] 字符串解析为日期
来源：http://cz.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ri.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bq.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://hh.asd995.cn

TS:   new Date("2024-01-02")
来源：http://vs.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fn.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ej.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://ue.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xd.9csxet.cn

[J04] 时间戳与日期互转
来源：http://xq.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://un.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qa.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ic.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gf.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pp.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zk.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mx.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nn.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://ez.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://wt.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fs.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://em.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://le.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://kb.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kw.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://tf.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nn.szxytkj.cn

[J06] 计算两时间之差
来源：http://iq.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://xj.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://ei.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dr.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yi.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yz.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://kh.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://dk.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://bc.haigaiapp.cn

[J07] 比较两个日期
来源：http://br.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://mm.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xt.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mu.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hw.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dy.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ny.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ss.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://wz.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://ud.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qf.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jh.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ox.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kw.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://so.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vr.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://th.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vt.huixinmuqiang.cn

[J09] 时区处理
来源：http://yg.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sq.nicolike.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ld.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jb.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ns.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nn.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yi.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xl.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ys.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://lm.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kn.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pe.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fx.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xy.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fi.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qs.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ef.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jn.lnxyls.cn

================================================================================
来源：http://ik.colortex.cn

K. JSON 与序列化
来源：http://iz.lnxyls.cn

================================================================================
来源：http://xt.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://ou.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sa.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wt.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://lf.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://gj.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pu.huanxung.cn

Go:   json.Marshal(obj)
来源：http://gt.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rq.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ug.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://an.bjjhwx.cn

Py:   json.loads(s)
来源：http://ya.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://og.521024.cn

JS:   JSON.parse(s)
来源：http://zg.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://bg.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ro.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://pk.colortex.cn

Ruby: JSON.parse(s)
来源：http://tn.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ib.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://xs.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://di.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gb.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sl.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://up.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zf.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eg.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xl.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tt.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://pp.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tf.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cx.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ae.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zv.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yv.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dy.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rk.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bk.asd995.cn

[K05] 深拷贝对象
来源：http://be.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://nx.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://dt.lnxyls.cn

JS:   structuredClone(obj)
来源：http://yu.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://lj.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ta.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kp.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yf.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nf.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://nz.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ya.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xm.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jh.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yv.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cr.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rt.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tm.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://em.huixinmuqiang.cn

[K07] 进制转换
来源：http://ze.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ah.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xh.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xy.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vc.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gt.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cq.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eu.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mk.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://ua.colortex.cn

Py:   pickle.dumps(obj)
来源：http://sz.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cw.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://zk.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://ht.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xa.chemitech.net.cn

Go:   encoding/gob
来源：http://em.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://gf.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ds.shxzukj.cn

================================================================================
来源：http://gk.jianghongdianzi.cn

L. 网络请求
来源：http://nx.szxytkj.cn

================================================================================
来源：http://xf.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://oc.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gd.yuexingan06.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sq.9csxet.cn

JS:   await fetch(url)
来源：http://nq.bookmarksfly.cn

TS:   await fetch(url)
来源：http://cq.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jt.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://by.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ui.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kj.szsharing.cn

[L02] 发送 POST JSON
来源：http://jz.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wh.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kn.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fj.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ks.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yj.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gf.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ob.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vn.hnjuh.cn

[L03] 设置自定义请求头
来源：http://lh.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ze.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wk.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rz.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ya.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fc.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tu.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mg.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yr.bookmarksfly.cn

[L04] 设置超时
来源：http://vx.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://gf.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lw.nicolike.cn


<!-- 参考信息 -->