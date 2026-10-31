代发 wailian999

JS:   e.message;  e.stack
来源：http://vz.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ui.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zo.9csxet.cn

Go:   err.Error()
来源：http://ig.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://vn.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://ux.haigaiapp.cn

[H09] 带错误码的异常
来源：http://dt.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jj.muxihuayi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://or.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://td.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mg.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cx.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fd.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hx.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://md.szsharing.cn

[H10] 资源自动释放
来源：http://ce.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rs.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dx.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qw.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xp.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xg.bjjhwx.cn

Go:   defer f.Close()
来源：http://mn.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zr.shxzukj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vm.wgjwhj.cn

================================================================================
来源：http://ov.szsharing.cn

I. 正则表达式
来源：http://ih.hnjuh.cn

================================================================================
来源：http://ef.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://dd.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://om.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pp.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://am.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://fb.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nx.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pf.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://hs.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zv.asd995.cn

[I02] 提取所有匹配
来源：http://me.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://kt.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uw.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fj.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://nx.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jy.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yx.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://kb.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gv.huixiangedu.cn

[I03] 提取捕获分组
来源：http://kc.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://km.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ku.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mq.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yf.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fb.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gf.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sv.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ss.szxytkj.cn

[I04] 正则替换
来源：http://be.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://em.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gd.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nf.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lq.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://en.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vl.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vm.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ud.szsharing.cn

[I05] 按正则拆分
来源：http://jv.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cw.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://px.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://az.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://ha.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://nl.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tn.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qd.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ci.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yv.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hl.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xa.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yz.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ri.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iy.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bb.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xs.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rv.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://cc.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ks.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ky.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dg.szsharing.cn

TS:   /error/gim
来源：http://wl.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://to.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tn.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://sh.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lu.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://zt.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uy.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ki.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sr.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qn.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qw.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hj.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hg.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mc.yuexingan06.cn

================================================================================
来源：http://xa.nicolike.cn

J. 日期与时间
来源：http://ys.shxzukj.cn

================================================================================
来源：http://ny.yuexingan06.cn

[J01] 获取当前时间
来源：http://en.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yv.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uw.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://ao.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://ek.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wj.szxytkj.cn

Go:   time.Now()
来源：http://gt.jctech888.com.cn

Ruby: Time.now
来源：http://ak.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sd.jianghongdianzi.cn

[J02] 格式化输出
来源：http://tq.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tt.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ba.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jg.muxihuayi.cn

TS:   d.toISOString()
来源：http://mr.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vz.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iu.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vg.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nf.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://eb.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://je.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wz.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://ao.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://pb.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ha.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wg.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://gf.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zy.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://up.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qr.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yr.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://js.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wx.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://di.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bk.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dx.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bz.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://cv.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://fb.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rt.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oq.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bq.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://fu.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tb.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://ux.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sz.muxihuayi.cn

[J06] 计算两时间之差
来源：http://lq.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://tz.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://vq.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ko.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eh.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qb.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://xg.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://oi.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://qs.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://oj.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://ze.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mr.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gi.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lr.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cs.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aa.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pj.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://mn.huanxung.cn

[J08] 提取年月日与星期
来源：http://yi.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kr.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dr.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xp.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bl.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bq.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iv.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zn.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hm.bookmarksfly.cn

[J09] 时区处理
来源：http://bs.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jd.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ce.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qw.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mp.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pg.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bf.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://md.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zo.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://dp.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wj.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kr.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://de.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bz.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kj.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xv.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yo.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cu.panjiajie.cn

================================================================================
来源：http://nv.bjjhwx.cn

K. JSON 与序列化
来源：http://vu.hnjuh.cn

================================================================================
来源：http://jy.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://im.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://my.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zl.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://ej.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://nr.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jp.bjjhwx.cn

Go:   json.Marshal(obj)
来源：http://jb.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://no.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fp.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://xg.bjjhwx.cn

Py:   json.loads(s)
来源：http://ys.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vv.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://wo.huanxung.cn

TS:   JSON.parse(s)
来源：http://bx.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://le.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://mm.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://cb.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dp.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://hw.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wy.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bj.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://iy.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xz.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://we.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fr.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jz.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xv.nicolike.cn

[K04] 读取 JSON 文件
来源：http://gs.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pp.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fv.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mf.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ar.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nv.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hv.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://el.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tm.shxzskj.cn

[K05] 深拷贝对象
来源：http://xe.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://as.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://wx.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://xo.9csxet.cn

TS:   structuredClone(obj)
来源：http://dw.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xf.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zv.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dw.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pl.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://rw.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://df.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ry.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yt.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kr.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bk.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dj.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yh.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cg.szsharing.cn

[K07] 进制转换
来源：http://vt.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vx.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xl.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cb.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pn.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yo.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jv.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ex.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hv.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://gj.bjjhwx.cn

Py:   pickle.dumps(obj)
来源：http://rl.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dn.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://wq.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://if.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gr.nszjky.cn

Go:   encoding/gob
来源：http://wc.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://qq.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zq.9csxet.cn

================================================================================
来源：http://om.521024.cn

L. 网络请求
来源：http://ct.haigaiapp.cn

================================================================================
来源：http://hy.newstarts.cn

[L01] 发送 GET 请求
来源：http://pm.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pa.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nc.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://pe.colortex.cn

TS:   await fetch(url)
来源：http://kt.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://er.521024.cn

Go:   resp, err := http.Get(url)
来源：http://nl.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ua.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://df.huanxung.cn

[L02] 发送 POST JSON
来源：http://vc.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qj.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://to.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iw.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yh.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vj.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ah.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gr.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ak.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://br.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mg.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vx.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fs.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zk.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nx.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gk.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://we.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://za.nicolike.cn

[L04] 设置超时
来源：http://ov.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://fr.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oq.lnxyls.cn


<!-- 参考信息 -->