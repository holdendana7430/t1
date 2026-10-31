代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://oq.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://hp.szxytkj.cn

[H09] 带错误码的异常
来源：http://ix.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ja.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zt.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zo.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nt.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xh.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vl.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lt.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wa.lnxyls.cn

[H10] 资源自动释放
来源：http://ux.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://at.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://af.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wt.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qe.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dl.haigaiapp.cn

Go:   defer f.Close()
来源：http://gi.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://di.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wq.shxzskj.cn

================================================================================
来源：http://ly.yuexingan06.cn

I. 正则表达式
来源：http://bu.jctech888.com.cn

================================================================================
来源：http://fb.shtwfgs.cn

[I01] 判断是否匹配
来源：http://xv.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hb.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pi.newstarts.cn

JS:   /\d+/.test(s)
来源：http://tk.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://yf.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jl.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oa.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://sn.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://an.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://be.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://co.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bt.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fo.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://mq.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rr.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zw.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://em.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oc.huanxung.cn

[I03] 提取捕获分组
来源：http://cv.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sb.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uj.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://en.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ga.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cd.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://si.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xp.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ql.chemitech.net.cn

[I04] 正则替换
来源：http://ni.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sy.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://su.lnxyls.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zx.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ts.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://oy.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jq.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gm.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jx.lnxyls.cn

[I05] 按正则拆分
来源：http://hc.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rq.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wb.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://xd.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://xb.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://ky.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pl.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ot.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wr.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mx.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://me.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zc.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lw.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zj.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yy.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wl.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xh.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ov.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://wy.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pe.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mu.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iq.gzmigu.cn

TS:   /error/gim
来源：http://ak.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kk.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vy.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://qm.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pe.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://ol.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zl.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rr.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ch.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vh.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rv.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yd.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dg.szsharing.cn

================================================================================
来源：http://ig.9csxet.cn

J. 日期与时间
来源：http://ub.huixinmuqiang.cn

================================================================================
来源：http://lm.hnjuh.cn

[J01] 获取当前时间
来源：http://lk.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hf.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://si.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://qm.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://mb.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bi.haigaiapp.cn

Go:   time.Now()
来源：http://ad.yuntaijiaju.cn

Ruby: Time.now
来源：http://uf.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kc.hnjuh.cn

[J02] 格式化输出
来源：http://me.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://it.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mp.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cw.hnjuh.cn

TS:   d.toISOString()
来源：http://aq.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qx.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bn.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ff.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ng.shxzskj.cn

[J03] 字符串解析为日期
来源：http://qq.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gn.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ut.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://ba.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://eg.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zw.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ng.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://lg.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ps.colortex.cn

[J04] 时间戳与日期互转
来源：http://fe.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gv.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fe.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ub.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wr.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://un.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://av.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eu.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vl.521024.cn

[J05] 时间加减（加 7 天）
来源：http://bm.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://ze.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ka.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xa.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kz.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://ft.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cn.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://uk.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rh.jctech888.com.cn

[J06] 计算两时间之差
来源：http://cl.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://vo.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://bw.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ei.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ru.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://aq.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://mu.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://sv.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://xq.hahajie.cn

[J07] 比较两个日期
来源：http://qs.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://ju.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cw.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xl.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://op.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fc.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ek.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zv.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://fj.gzmigu.cn

[J08] 提取年月日与星期
来源：http://og.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mc.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qy.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vo.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ws.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yl.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pi.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vg.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gl.yuexingan06.cn

[J09] 时区处理
来源：http://yu.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ev.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gw.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ug.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lw.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hn.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rw.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gg.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pi.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://pn.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bt.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pk.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aa.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zc.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qo.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qk.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ms.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://td.9csxet.cn

================================================================================
来源：http://cq.nszjky.cn

K. JSON 与序列化
来源：http://zw.shxzskj.cn

================================================================================
来源：http://al.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://pj.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uq.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ls.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://rt.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://lp.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ic.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://sd.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fb.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kg.asd995.cn

[K02] JSON 字符串转对象
来源：http://yt.jctech888.com.cn

Py:   json.loads(s)
来源：http://jx.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://js.shxzskj.cn

JS:   JSON.parse(s)
来源：http://ja.szsharing.cn

TS:   JSON.parse(s)
来源：http://xc.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dq.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://ji.9csxet.cn

Ruby: JSON.parse(s)
来源：http://th.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wd.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://in.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rw.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sp.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dw.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ag.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vp.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ko.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cv.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dk.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://sx.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://op.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vh.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://un.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gz.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aw.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mj.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pj.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gr.lnxyls.cn

[K05] 深拷贝对象
来源：http://nh.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://kt.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://tc.asd995.cn

JS:   structuredClone(obj)
来源：http://bh.shxzskj.cn

TS:   structuredClone(obj)
来源：http://xm.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dn.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zg.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jx.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://eg.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://xh.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gi.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mq.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aq.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jn.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pa.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bm.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wk.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://su.shxzskj.cn

[K07] 进制转换
来源：http://ms.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aj.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jq.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ju.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rf.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xt.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xb.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ul.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dx.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://vs.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://tc.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pt.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://tm.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://ga.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ar.hnjuh.cn

Go:   encoding/gob
来源：http://uo.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://xl.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ig.colortex.cn

================================================================================
来源：http://vm.asd995.cn

L. 网络请求
来源：http://ok.hahajie.cn

================================================================================
来源：http://df.nszjky.cn

[L01] 发送 GET 请求
来源：http://dc.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qk.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lp.shxzukj.cn

JS:   await fetch(url)
来源：http://kf.521024.cn

TS:   await fetch(url)
来源：http://hk.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lb.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://xf.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eu.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xw.lnxyls.cn

[L02] 发送 POST JSON
来源：http://xc.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wc.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nf.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cq.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xz.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gr.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sn.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bl.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qr.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://nx.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nw.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://md.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ca.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://om.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ka.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lq.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ro.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gr.jctech888.com.cn

[L04] 设置超时
来源：http://zs.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://hk.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iw.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nv.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vf.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://da.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wv.yuexingan06.cn


<!-- 参考信息 -->