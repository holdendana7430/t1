代发 wailian999

JS:   e.message;  e.stack
来源：http://hl.huixiangedu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://am.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gz.szsharing.cn

Go:   err.Error()
来源：http://xt.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://gj.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://kb.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://ce.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eg.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zg.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jt.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ic.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mw.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gv.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ec.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ti.jctech888.com.cn

[H10] 资源自动释放
来源：http://fm.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gc.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wv.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zm.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nz.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mb.panjiajie.cn

Go:   defer f.Close()
来源：http://dv.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ik.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sc.521024.cn

================================================================================
来源：http://ew.panjiajie.cn

I. 正则表达式
来源：http://ps.jctech888.com.cn

================================================================================
来源：http://gy.bjjhwx.cn

[I01] 判断是否匹配
来源：http://ea.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pt.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oh.hahajie.cn

JS:   /\d+/.test(s)
来源：http://vp.huanxung.cn

TS:   /\d+/.test(s)
来源：http://he.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oz.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bt.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://wa.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yb.shtwfgs.cn

[I02] 提取所有匹配
来源：http://es.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://tv.huanxung.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nc.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ki.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://kl.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qd.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nu.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://mb.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pu.chemitech.net.cn

[I03] 提取捕获分组
来源：http://zx.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xo.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://el.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ge.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://om.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://is.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://id.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tc.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gd.nszjky.cn

[I04] 正则替换
来源：http://oj.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jf.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ba.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ix.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uf.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ay.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ww.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bj.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ud.lnxyls.cn

[I05] 按正则拆分
来源：http://hw.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tg.colortex.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zx.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://bp.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://xf.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://ua.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nt.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yw.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jh.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aq.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bs.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ea.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uv.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ql.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vt.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cu.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hw.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://on.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://ga.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cd.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ha.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hd.newstarts.cn

TS:   /error/gim
来源：http://al.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://od.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mi.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://av.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kf.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://as.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dz.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ru.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fg.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zu.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://je.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zb.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rh.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://su.shtwfgs.cn

================================================================================
来源：http://xg.nszjky.cn

J. 日期与时间
来源：http://ip.huanxung.cn

================================================================================
来源：http://eu.huixiangedu.cn

[J01] 获取当前时间
来源：http://iy.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fw.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yy.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://pd.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://ry.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pf.521024.cn

Go:   time.Now()
来源：http://tb.huixinmuqiang.cn

Ruby: Time.now
来源：http://mx.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fq.lnxyls.cn

[J02] 格式化输出
来源：http://ot.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yz.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sl.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wz.huanxung.cn

TS:   d.toISOString()
来源：http://vo.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tv.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bj.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lj.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ry.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://yj.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uk.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://af.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://xn.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://nh.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sh.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fs.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://fe.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mf.521024.cn

[J04] 时间戳与日期互转
来源：http://wk.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hu.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cp.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pf.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://st.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vg.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xp.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xz.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pc.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://wx.asd995.cn

Py:   now + timedelta(days=7)
来源：http://av.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jq.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bp.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yh.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://lx.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rn.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://xn.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zt.muxihuayi.cn

[J06] 计算两时间之差
来源：http://ai.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://us.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://sl.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yq.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rb.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ov.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://hi.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://rg.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://ks.gzmigu.cn

[J07] 比较两个日期
来源：http://fd.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://su.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ee.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jt.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rk.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bp.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ch.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bt.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://gf.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://ng.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yf.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jn.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wv.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ip.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wr.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yo.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uy.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eu.bookmarksfly.cn

[J09] 时区处理
来源：http://qg.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nq.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dj.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ir.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ke.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://og.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://po.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ns.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cw.521024.cn

[J10] 取今天 / 本月第一天
来源：http://bv.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xq.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://su.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gq.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://df.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ot.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rh.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yw.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kr.bjjhwx.cn

================================================================================
来源：http://zd.huixiangedu.cn

K. JSON 与序列化
来源：http://uz.9csxet.cn

================================================================================
来源：http://ao.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://xl.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://is.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yq.521024.cn

JS:   JSON.stringify(obj)
来源：http://ro.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://lf.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xr.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://uq.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zt.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jp.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://pj.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://ty.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uh.hahajie.cn

JS:   JSON.parse(s)
来源：http://zg.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://ey.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qr.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://jz.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://tc.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://et.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://oh.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nw.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ss.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ss.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ch.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rm.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nv.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vp.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ep.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://da.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ly.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cw.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://od.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ea.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ia.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hj.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ql.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pq.gzmigu.cn

[K05] 深拷贝对象
来源：http://rz.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://xr.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://pe.szxytkj.cn

JS:   structuredClone(obj)
来源：http://ia.nszjky.cn

TS:   structuredClone(obj)
来源：http://ad.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ry.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cs.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tz.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://om.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://qr.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gp.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://on.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ev.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nn.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nf.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sr.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pu.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ep.bjjhwx.cn

[K07] 进制转换
来源：http://an.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hs.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://su.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uc.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tz.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zx.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uf.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xz.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aq.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://my.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://ix.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ns.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://eq.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://ws.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://am.panjiajie.cn

Go:   encoding/gob
来源：http://ak.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://mt.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yc.bjjhwx.cn

================================================================================
来源：http://xp.wgjwhj.cn

L. 网络请求
来源：http://he.9csxet.cn

================================================================================
来源：http://hn.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://ik.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rd.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ko.szsharing.cn

JS:   await fetch(url)
来源：http://lx.bjjhwx.cn

TS:   await fetch(url)
来源：http://uk.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rx.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://wk.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nb.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ri.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://yi.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hx.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vz.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zo.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lc.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rc.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bb.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mw.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jl.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://pe.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lz.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sw.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gd.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wp.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zt.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ui.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dm.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aa.szxytkj.cn

[L04] 设置超时
来源：http://dm.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://ll.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pe.hnjuh.cn


<!-- 参考信息 -->