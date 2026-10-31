代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://md.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://gj.panjiajie.cn

[H09] 带错误码的异常
来源：http://fs.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wt.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yx.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mi.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jm.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://do.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mk.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zq.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nv.haigaiapp.cn

[H10] 资源自动释放
来源：http://yl.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vs.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://en.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ty.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lx.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kl.wgjwhj.cn

Go:   defer f.Close()
来源：http://fv.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gc.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://el.jianghongdianzi.cn

================================================================================
来源：http://py.szxytkj.cn

I. 正则表达式
来源：http://mo.panjiajie.cn

================================================================================
来源：http://cm.newstarts.cn

[I01] 判断是否匹配
来源：http://aw.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lk.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ko.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://vb.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://wy.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ud.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iw.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://lj.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://og.szsharing.cn

[I02] 提取所有匹配
来源：http://qd.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://fc.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fv.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mx.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://pl.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qp.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tr.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://fz.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mr.huixiangedu.cn

[I03] 提取捕获分组
来源：http://hf.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mz.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lj.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://td.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dq.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ib.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://am.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nw.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ow.hnjuh.cn

[I04] 正则替换
来源：http://sv.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mo.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mk.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lc.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ig.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vn.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rp.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wm.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pp.wgjwhj.cn

[I05] 按正则拆分
来源：http://cr.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yy.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gq.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://hw.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://tv.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://uf.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sd.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uv.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yq.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ki.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wu.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://di.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://em.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://op.szxytkj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ux.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wx.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pu.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sg.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://is.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://af.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fb.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cq.jctech888.com.cn

TS:   /error/gim
来源：http://gx.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aw.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zj.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://nf.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vz.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://xj.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dj.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iy.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ke.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yp.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vs.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bi.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nt.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pn.521024.cn

================================================================================
来源：http://nc.colortex.cn

J. 日期与时间
来源：http://wi.shxzukj.cn

================================================================================
来源：http://mq.szxytkj.cn

[J01] 获取当前时间
来源：http://fy.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dr.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wx.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://qe.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://ge.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ck.haigaiapp.cn

Go:   time.Now()
来源：http://ko.yuexingan06.cn

Ruby: Time.now
来源：http://ae.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cg.521024.cn

[J02] 格式化输出
来源：http://ju.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iz.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yd.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xq.newstarts.cn

TS:   d.toISOString()
来源：http://ci.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wf.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pt.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qt.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qp.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://fu.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rj.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fe.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://dz.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://es.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://md.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zi.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ao.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yq.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://ot.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wf.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uz.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kp.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sj.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ku.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dh.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://td.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cw.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://cn.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://uz.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iu.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fq.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ce.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://em.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vr.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://ln.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://km.9csxet.cn

[J06] 计算两时间之差
来源：http://af.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://om.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://ay.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nh.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jt.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oz.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://sq.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://ry.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://td.shxzukj.cn

[J07] 比较两个日期
来源：http://jn.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://av.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mz.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://os.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hd.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://an.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tk.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rx.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://is.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://ap.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gy.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xn.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://am.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qi.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pj.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nb.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lj.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sl.huixiangedu.cn

[J09] 时区处理
来源：http://wa.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pz.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zh.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vk.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ry.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qi.nicolike.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wu.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wo.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ye.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://dq.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xo.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mj.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uf.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hu.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ni.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dp.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tm.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vw.huixinmuqiang.cn

================================================================================
来源：http://ak.nicolike.cn

K. JSON 与序列化
来源：http://oy.lnxyls.cn

================================================================================
来源：http://sx.wgjwhj.cn

[K01] 对象转 JSON 字符串
来源：http://ii.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://my.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ge.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://ca.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://cs.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cl.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://dg.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jt.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gb.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://vi.szxytkj.cn

Py:   json.loads(s)
来源：http://mx.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pd.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://rt.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://cy.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ox.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://qb.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://gg.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zp.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://fc.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zq.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vw.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bc.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://je.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yf.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ge.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ht.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sv.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://yy.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ck.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dn.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uk.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wd.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nr.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yi.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qc.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fb.huanxung.cn

[K05] 深拷贝对象
来源：http://za.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://ce.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://az.nszjky.cn

JS:   structuredClone(obj)
来源：http://yl.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://ry.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oj.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hm.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pb.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fp.nicolike.cn

[K06] 解析 URL 查询串
来源：http://eu.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wi.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rj.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ms.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bp.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vz.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zz.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fd.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oa.hahajie.cn

[K07] 进制转换
来源：http://kj.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mz.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oq.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bm.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://md.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gm.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yw.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ym.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rh.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://jy.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://mw.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cy.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://lw.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://io.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zk.panjiajie.cn

Go:   encoding/gob
来源：http://uc.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://vr.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dq.panjiajie.cn

================================================================================
来源：http://rd.nszjky.cn

L. 网络请求
来源：http://yg.gzmigu.cn

================================================================================
来源：http://he.lnxyls.cn

[L01] 发送 GET 请求
来源：http://xh.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://te.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ym.muxihuayi.cn

JS:   await fetch(url)
来源：http://wk.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://gb.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kj.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://ko.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yw.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hu.gzmigu.cn

[L02] 发送 POST JSON
来源：http://tx.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ko.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fd.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://er.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tk.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://on.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vk.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wy.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bz.asd995.cn

[L03] 设置自定义请求头
来源：http://qx.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rb.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xs.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://du.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yv.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dj.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wq.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sg.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vf.panjiajie.cn

[L04] 设置超时
来源：http://pw.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://mc.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lq.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://at.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://am.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ly.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ja.hnjuh.cn


<!-- 参考信息 -->