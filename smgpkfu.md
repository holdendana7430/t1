代发 wailian999

TS:   console.assert(x > 0);
来源：http://tq.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://ta.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ju.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vm.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://fi.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://hk.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://dg.chemitech.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://di.shxzskj.cn

JS:   e.message;  e.stack
来源：http://qi.huixiangedu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qp.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xn.bjjhwx.cn

Go:   err.Error()
来源：http://np.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://iv.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://eg.9csxet.cn

[H09] 带错误码的异常
来源：http://lr.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dt.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nd.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sc.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ng.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lc.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jg.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dp.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gb.shxzukj.cn

[H10] 资源自动释放
来源：http://lp.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qd.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kc.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vh.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dt.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xz.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://ao.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oz.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cg.521024.cn

================================================================================
来源：http://jf.jctech888.com.cn

I. 正则表达式
来源：http://jd.szsharing.cn

================================================================================
来源：http://tk.haigaiapp.cn

[I01] 判断是否匹配
来源：http://ui.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aw.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pr.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://go.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://xb.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rc.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hl.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://zk.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yq.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://km.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://ed.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xp.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://in.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://hk.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xx.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kn.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://xp.bjjhwx.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ab.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://re.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bq.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bd.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wb.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bk.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nx.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oq.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ot.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xc.haigaiapp.cn

[I04] 正则替换
来源：http://em.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tw.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fm.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nc.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wm.jctech888.com.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zw.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://px.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lf.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tr.bookmarksfly.cn

[I05] 按正则拆分
来源：http://cl.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ok.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://py.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://ii.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://wz.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://kg.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zb.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bm.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ck.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nd.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sv.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wn.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ur.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mu.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eh.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mp.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ep.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zg.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://vl.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eb.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sf.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kf.lnxyls.cn

TS:   /error/gim
来源：http://ip.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rr.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vm.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://js.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xd.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://tl.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vm.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://co.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ek.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pg.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ls.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sy.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ah.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ip.panjiajie.cn

================================================================================
来源：http://ck.bookmarksfly.cn

J. 日期与时间
来源：http://jb.huanxung.cn

================================================================================
来源：http://gi.wgjwhj.cn

[J01] 获取当前时间
来源：http://zy.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gp.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hx.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://wz.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://lf.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ba.panjiajie.cn

Go:   time.Now()
来源：http://ag.chemitech.net.cn

Ruby: Time.now
来源：http://wu.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://me.521024.cn

[J02] 格式化输出
来源：http://ep.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nm.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ft.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tu.szsharing.cn

TS:   d.toISOString()
来源：http://ip.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xj.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://np.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ft.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://re.newstarts.cn

[J03] 字符串解析为日期
来源：http://vc.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hh.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pu.colortex.cn

JS:   new Date("2024-01-02")
来源：http://dn.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://bt.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://da.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://de.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://hk.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ue.hahajie.cn

[J04] 时间戳与日期互转
来源：http://jj.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ud.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gu.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pg.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jw.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nw.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rj.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ig.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ed.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://cm.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://kj.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yh.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lg.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ob.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://tw.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://my.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://ge.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pk.wgjwhj.cn

[J06] 计算两时间之差
来源：http://za.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://df.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://xn.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://er.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cc.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rw.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://up.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://zm.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://vb.bjjhwx.cn

[J07] 比较两个日期
来源：http://sq.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://wi.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hs.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zj.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cz.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mu.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xa.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fc.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://fw.gzmigu.cn

[J08] 提取年月日与星期
来源：http://gj.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ny.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sx.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ly.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pv.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fv.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ip.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://am.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rj.hahajie.cn

[J09] 时区处理
来源：http://sy.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://im.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ep.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vh.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ty.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kg.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zo.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tf.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pb.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://ic.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oe.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ag.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://re.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ee.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iz.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ze.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ro.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cd.nicolike.cn

================================================================================
来源：http://wl.newstarts.cn

K. JSON 与序列化
来源：http://mv.nszjky.cn

================================================================================
来源：http://dt.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://qz.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tm.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vq.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://ag.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://xf.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xd.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://ek.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rq.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zm.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://ay.nszjky.cn

Py:   json.loads(s)
来源：http://ts.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rs.colortex.cn

JS:   JSON.parse(s)
来源：http://ox.newstarts.cn

TS:   JSON.parse(s)
来源：http://xn.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vz.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://jl.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://rg.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ot.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://tv.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ba.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eo.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://iz.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rf.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aq.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gm.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tj.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oo.szsharing.cn

[K04] 读取 JSON 文件
来源：http://nu.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hv.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oi.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pn.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://op.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vd.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iy.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qq.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cr.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://va.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://kp.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://sz.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://ek.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://qv.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ak.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ap.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zq.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wl.colortex.cn

[K06] 解析 URL 查询串
来源：http://zp.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fe.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ro.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tt.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wt.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nj.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yr.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wh.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://py.yuexingan06.cn

[K07] 进制转换
来源：http://kd.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rb.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ow.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ws.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://om.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zk.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nc.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lm.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ju.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://sh.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://hv.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qz.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://ls.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://ip.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://it.shtwfgs.cn

Go:   encoding/gob
来源：http://bv.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://ye.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vo.nszjky.cn

================================================================================
来源：http://vs.wgjwhj.cn

L. 网络请求
来源：http://sk.haigaiapp.cn

================================================================================
来源：http://hc.9csxet.cn

[L01] 发送 GET 请求
来源：http://wq.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://je.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gl.shxzskj.cn

JS:   await fetch(url)
来源：http://ee.jctech888.com.cn

TS:   await fetch(url)
来源：http://tw.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pv.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://pj.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kj.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tn.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://gy.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qr.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uj.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yb.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fj.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kc.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mm.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xf.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mh.panjiajie.cn

[L03] 设置自定义请求头
来源：http://jm.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wn.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://np.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gd.colortex.cn


<!-- 参考信息 -->