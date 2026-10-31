代发 wailian999

JS:   e.message;  e.stack
来源：http://iw.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pz.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kb.bookmarksfly.cn

Go:   err.Error()
来源：http://bh.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://ak.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://hn.haigaiapp.cn

[H09] 带错误码的异常
来源：http://nn.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zy.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tj.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hf.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dc.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sm.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bk.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://st.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qf.huixiangedu.cn

[H10] 资源自动释放
来源：http://el.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://at.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wb.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vi.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ix.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tb.szsharing.cn

Go:   defer f.Close()
来源：http://wi.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zi.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lf.szsharing.cn

================================================================================
来源：http://si.shtwfgs.cn

I. 正则表达式
来源：http://vb.szsharing.cn

================================================================================
来源：http://iu.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://em.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ih.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pr.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://ng.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://tj.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pa.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ya.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://yn.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vw.szsharing.cn

[I02] 提取所有匹配
来源：http://xt.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://pr.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oq.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lk.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://ks.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://br.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sj.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://pi.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vv.shxzukj.cn

[I03] 提取捕获分组
来源：http://ty.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iw.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gf.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tk.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pb.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qn.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mq.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://un.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sy.asd995.cn

[I04] 正则替换
来源：http://bc.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mp.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yp.muxihuayi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ow.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rq.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jk.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tz.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nz.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yu.hahajie.cn

[I05] 按正则拆分
来源：http://yo.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kl.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pr.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://hp.lnxyls.cn

TS:   s.split(/\s*,\s*/)
来源：http://sn.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://qw.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eq.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://os.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mp.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ug.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dw.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xy.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vh.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hh.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://om.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://li.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lh.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jf.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://ij.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pp.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xo.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sy.jianghongdianzi.cn

TS:   /error/gim
来源：http://tc.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vq.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sm.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://ww.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://at.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ee.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://og.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fx.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yo.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gp.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yi.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://py.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ou.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nw.colortex.cn

================================================================================
来源：http://fx.nicolike.cn

J. 日期与时间
来源：http://yr.huixiangedu.cn

================================================================================
来源：http://sp.nicolike.cn

[J01] 获取当前时间
来源：http://bf.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xl.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ru.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://hr.9csxet.cn

TS:   new Date();  Date.now()
来源：http://xx.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ft.shtwfgs.cn

Go:   time.Now()
来源：http://wi.hnjuh.cn

Ruby: Time.now
来源：http://iu.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pf.chemitech.net.cn

[J02] 格式化输出
来源：http://tq.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hl.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mj.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ja.panjiajie.cn

TS:   d.toISOString()
来源：http://pj.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://io.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pd.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jx.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yy.szxytkj.cn

[J03] 字符串解析为日期
来源：http://dv.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gh.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ph.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://ze.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://wp.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uo.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sx.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://yk.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fh.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://ap.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kd.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dw.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://br.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dw.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pt.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iq.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hn.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pp.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://ia.colortex.cn

Py:   now + timedelta(days=7)
来源：http://bx.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xs.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sq.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iw.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://zw.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vc.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://kd.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vs.muxihuayi.cn

[J06] 计算两时间之差
来源：http://ng.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://bm.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://cy.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iy.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ja.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mn.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://ll.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://om.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://pb.szsharing.cn

[J07] 比较两个日期
来源：http://vl.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://hv.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zu.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://se.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qt.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ea.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ql.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vz.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://cf.nicolike.cn

[J08] 提取年月日与星期
来源：http://zv.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mu.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ia.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yo.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rx.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hp.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ew.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nd.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gu.521024.cn

[J09] 时区处理
来源：http://kp.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cc.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tg.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ja.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dt.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vd.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://up.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://or.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tw.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://bn.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bf.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ca.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yw.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dq.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ko.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qe.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://es.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nl.colortex.cn

================================================================================
来源：http://jc.chemitech.net.cn

K. JSON 与序列化
来源：http://bx.muxihuayi.cn

================================================================================
来源：http://mt.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://qc.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ym.gzmigu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nm.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://vk.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://pf.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dr.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://ua.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qs.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ot.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://nb.panjiajie.cn

Py:   json.loads(s)
来源：http://aj.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zk.szxytkj.cn

JS:   JSON.parse(s)
来源：http://gp.shxzskj.cn

TS:   JSON.parse(s)
来源：http://un.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ch.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://ph.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://wq.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yb.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://hm.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wk.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qg.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nd.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yj.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xd.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jo.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zo.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hm.asd995.cn

[K04] 读取 JSON 文件
来源：http://tl.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tq.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://da.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lh.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oq.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cz.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nc.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://eu.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bz.lnxyls.cn

[K05] 深拷贝对象
来源：http://ca.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://fv.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://ak.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://az.szsharing.cn

TS:   structuredClone(obj)
来源：http://au.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cu.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nz.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yb.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qg.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://am.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xh.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://is.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gw.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fu.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qi.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qq.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oa.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://as.shxzskj.cn

[K07] 进制转换
来源：http://kz.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oa.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ih.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hs.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qe.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hl.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fq.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sk.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lv.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://ex.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://hd.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sx.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://fr.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://js.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ke.lnxyls.cn

Go:   encoding/gob
来源：http://oa.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://yh.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eg.521024.cn

================================================================================
来源：http://oq.colortex.cn

L. 网络请求
来源：http://tc.lnxyls.cn

================================================================================
来源：http://us.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://sd.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jw.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tq.nicolike.cn

JS:   await fetch(url)
来源：http://kv.haigaiapp.cn

TS:   await fetch(url)
来源：http://gv.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xc.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://ja.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ts.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ap.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://rs.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://up.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ja.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vu.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://em.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ho.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vb.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://el.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://og.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://di.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nn.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qd.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vo.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://am.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iz.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://am.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mk.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jg.huanxung.cn

[L04] 设置超时
来源：http://mj.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://ub.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ve.yuntaijiaju.cn


<!-- 参考信息 -->