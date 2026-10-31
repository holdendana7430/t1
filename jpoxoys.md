代发 wailian999

JS:   e.message;  e.stack
来源：http://au.huixiangedu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://eb.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uv.colortex.cn

Go:   err.Error()
来源：http://gm.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://nz.panjiajie.cn

C#:   e.Message;  e.StackTrace
来源：http://dj.colortex.cn

[H09] 带错误码的异常
来源：http://jo.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ru.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://aj.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ae.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://km.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ss.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hc.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ym.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gd.colortex.cn

[H10] 资源自动释放
来源：http://br.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ec.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ab.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xm.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mq.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://db.szxytkj.cn

Go:   defer f.Close()
来源：http://xb.521024.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://id.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kr.lnxyls.cn

================================================================================
来源：http://hz.521024.cn

I. 正则表达式
来源：http://su.szsharing.cn

================================================================================
来源：http://po.9csxet.cn

[I01] 判断是否匹配
来源：http://in.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://li.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cz.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://ak.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://rx.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ze.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ed.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://ir.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qq.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://tq.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://tj.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ze.bookmarksfly.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ag.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://hc.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ov.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bn.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://ut.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jp.huanxung.cn

[I03] 提取捕获分组
来源：http://xr.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pv.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rc.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://li.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://og.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sb.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fs.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://is.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jr.panjiajie.cn

[I04] 正则替换
来源：http://am.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oj.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yj.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mi.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ak.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wk.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wi.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://go.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fw.bookmarksfly.cn

[I05] 按正则拆分
来源：http://pc.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ow.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rr.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://wy.hahajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://sh.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://yv.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vc.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cy.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ve.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rx.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sa.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vn.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ng.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bb.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xr.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jd.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oz.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tt.szxytkj.cn

[I07] 忽略大小写与多行模式
来源：http://bt.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iv.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tq.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ij.gzmigu.cn

TS:   /error/gim
来源：http://bi.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lm.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lf.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://cx.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ew.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://ch.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bb.huixiangedu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bn.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ry.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gi.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lm.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lc.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://px.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fx.huanxung.cn

================================================================================
来源：http://fi.nicolike.cn

J. 日期与时间
来源：http://af.shxzskj.cn

================================================================================
来源：http://fy.bjjhwx.cn

[J01] 获取当前时间
来源：http://kv.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xz.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yo.9csxet.cn

JS:   new Date();  Date.now()
来源：http://ca.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://hd.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hh.bookmarksfly.cn

Go:   time.Now()
来源：http://sn.huanxung.cn

Ruby: Time.now
来源：http://of.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vl.bookmarksfly.cn

[J02] 格式化输出
来源：http://et.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hi.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://id.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://im.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://uy.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xl.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qb.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qa.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lb.panjiajie.cn

[J03] 字符串解析为日期
来源：http://nw.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ws.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ca.colortex.cn

JS:   new Date("2024-01-02")
来源：http://ji.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://ur.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wl.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bo.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://sp.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hs.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://dl.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zi.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gq.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zv.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vm.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://py.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://of.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ea.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lm.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://ow.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://ux.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uz.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://di.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ms.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://ud.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ki.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://rp.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lr.asd995.cn

[J06] 计算两时间之差
来源：http://xe.asd995.cn

Py:   (end - start).total_seconds()
来源：http://ek.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://or.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nk.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bh.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hx.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://hj.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://ac.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://ti.shxzukj.cn

[J07] 比较两个日期
来源：http://ln.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://qw.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cr.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://df.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ik.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zw.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ay.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mj.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://mh.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://gr.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lz.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ot.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qr.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zc.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kp.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ar.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dv.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ed.gzmigu.cn

[J09] 时区处理
来源：http://vp.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tu.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vf.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://da.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xp.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://we.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aj.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sy.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lx.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://qz.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ld.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ih.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aj.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sk.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fp.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dl.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vd.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zd.nszjky.cn

================================================================================
来源：http://js.jctech888.com.cn

K. JSON 与序列化
来源：http://ai.newstarts.cn

================================================================================
来源：http://lp.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://bw.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mb.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://un.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://sh.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://cc.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oj.newstarts.cn

Go:   json.Marshal(obj)
来源：http://np.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dm.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fw.hahajie.cn

[K02] JSON 字符串转对象
来源：http://ft.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://cu.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fr.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://jh.nicolike.cn

TS:   JSON.parse(s)
来源：http://gd.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ii.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://bb.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://hp.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://if.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://ng.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fb.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sg.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ps.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ja.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rp.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rj.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zd.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://db.asd995.cn

[K04] 读取 JSON 文件
来源：http://zt.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hi.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://go.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rr.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://he.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ar.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eu.shtwfgs.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ql.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://co.gzmigu.cn

[K05] 深拷贝对象
来源：http://hn.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://sv.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://os.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://fc.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://bk.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hi.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ug.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ws.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dc.nszjky.cn

[K06] 解析 URL 查询串
来源：http://vi.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yb.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ng.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://en.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nn.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nw.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ls.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pk.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ah.jianghongdianzi.cn

[K07] 进制转换
来源：http://bh.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xy.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ee.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lf.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ww.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yx.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mu.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rs.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mb.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://pb.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://qy.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vq.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://ug.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://je.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://it.521024.cn

Go:   encoding/gob
来源：http://po.521024.cn

Ruby: Marshal.dump(obj)
来源：http://nz.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bw.hnjuh.cn

================================================================================
来源：http://qw.yuntaijiaju.cn

L. 网络请求
来源：http://vu.hahajie.cn

================================================================================
来源：http://gh.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://lv.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ey.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wm.newstarts.cn

JS:   await fetch(url)
来源：http://ss.nicolike.cn

TS:   await fetch(url)
来源：http://vu.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xo.521024.cn

Go:   resp, err := http.Get(url)
来源：http://bj.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bn.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tb.shxzukj.cn

[L02] 发送 POST JSON
来源：http://ev.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vz.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ch.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zs.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dw.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://em.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iu.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vq.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zk.shxzukj.cn

[L03] 设置自定义请求头
来源：http://ck.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ns.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sp.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wj.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dt.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ih.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qq.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qq.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cf.panjiajie.cn

[L04] 设置超时
来源：http://kv.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://gl.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tf.haigaiapp.cn


<!-- 参考信息 -->