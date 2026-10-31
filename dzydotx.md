代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://nt.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://uw.jianghongdianzi.cn

[H09] 带错误码的异常
来源：http://ne.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qx.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ll.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wj.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eb.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uq.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wx.9csxet.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qy.lnxyls.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nd.jctech888.com.cn

[H10] 资源自动释放
来源：http://yt.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zh.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://se.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xu.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xs.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nj.bjjhwx.cn

Go:   defer f.Close()
来源：http://vp.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vw.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zl.shxzskj.cn

================================================================================
来源：http://jg.shxzukj.cn

I. 正则表达式
来源：http://xi.hnjuh.cn

================================================================================
来源：http://vp.newstarts.cn

[I01] 判断是否匹配
来源：http://tf.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tu.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sa.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://ta.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://tp.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://he.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bd.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://bc.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aq.yuexingan06.cn

[I02] 提取所有匹配
来源：http://gm.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://kp.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qj.bookmarksfly.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zf.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://nk.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kf.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pw.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://bc.bjjhwx.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mz.521024.cn

[I03] 提取捕获分组
来源：http://vu.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oj.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uh.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://th.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ma.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://an.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oo.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://to.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://if.yuexingan06.cn

[I04] 正则替换
来源：http://eh.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ap.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ni.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bs.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zy.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ce.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kc.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ec.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hv.hahajie.cn

[I05] 按正则拆分
来源：http://or.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xg.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uu.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://if.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://io.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://bd.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ri.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bw.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ts.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rz.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iu.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://by.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zs.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xa.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iv.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ze.haigaiapp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://su.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nm.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://jm.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oq.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vb.bjjhwx.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yi.jctech888.com.cn

TS:   /error/gim
来源：http://wc.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jk.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ii.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://qy.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mf.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://zy.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ct.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xj.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ja.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qz.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ra.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xy.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bu.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ea.yuntaijiaju.cn

================================================================================
来源：http://mi.haigaiapp.cn

J. 日期与时间
来源：http://kg.hahajie.cn

================================================================================
来源：http://fb.asd995.cn

[J01] 获取当前时间
来源：http://va.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ht.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fd.lnxyls.cn

JS:   new Date();  Date.now()
来源：http://gx.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://zy.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lb.hahajie.cn

Go:   time.Now()
来源：http://db.lnxyls.cn

Ruby: Time.now
来源：http://pt.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ro.521024.cn

[J02] 格式化输出
来源：http://wi.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ve.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yh.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xi.521024.cn

TS:   d.toISOString()
来源：http://xc.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vp.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aq.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nx.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lx.shxzukj.cn

[J03] 字符串解析为日期
来源：http://ck.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ux.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gm.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://ji.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://uc.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://li.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xu.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://be.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qg.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://mr.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qj.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ov.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://le.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ui.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://og.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yf.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rb.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cy.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://mm.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://jb.jianghongdianzi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://if.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ai.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iu.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://gq.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tl.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://hu.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xk.9csxet.cn

[J06] 计算两时间之差
来源：http://ws.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://mu.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://nb.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qw.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ks.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bx.521024.cn

Go:   end.Sub(start).Hours()
来源：http://nf.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://ny.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://ps.haigaiapp.cn

[J07] 比较两个日期
来源：http://tm.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://fz.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mb.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ee.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vr.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fa.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yv.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://po.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://xf.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://lt.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://am.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ai.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dl.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cl.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wv.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ug.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wu.szsharing.cn

[J09] 时区处理
来源：http://nx.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xw.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ga.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://av.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rq.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gy.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://me.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ta.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gu.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://in.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zv.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kb.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qa.shxzukj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dt.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oh.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xy.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hd.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rh.gzmigu.cn

================================================================================
来源：http://nm.gzmigu.cn

K. JSON 与序列化
来源：http://du.lnxyls.cn

================================================================================
来源：http://dg.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://ul.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nm.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mj.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://aj.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://hu.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rt.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://yo.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sy.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://av.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://dw.muxihuayi.cn

Py:   json.loads(s)
来源：http://vl.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hb.gzmigu.cn

JS:   JSON.parse(s)
来源：http://qy.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://ml.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hq.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://at.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://eo.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ne.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://rm.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://om.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rm.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jd.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kp.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uv.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://of.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://am.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wu.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://ud.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://as.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://no.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xg.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://at.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ak.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dh.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qw.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ky.szxytkj.cn

[K05] 深拷贝对象
来源：http://fr.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://px.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://gj.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://ol.colortex.cn

TS:   structuredClone(obj)
来源：http://ug.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uw.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ff.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vm.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xa.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://kl.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ys.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ru.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kp.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mc.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rg.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nh.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://na.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bg.shxzskj.cn

[K07] 进制转换
来源：http://df.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hk.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uj.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tt.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gu.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jd.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bm.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gv.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gz.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://wt.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://jv.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ua.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://ui.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://wb.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xu.huixiangedu.cn

Go:   encoding/gob
来源：http://ph.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://mu.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hy.panjiajie.cn

================================================================================
来源：http://wt.yuntaijiaju.cn

L. 网络请求
来源：http://ny.bjjhwx.cn

================================================================================
来源：http://uz.szsharing.cn

[L01] 发送 GET 请求
来源：http://pp.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ez.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://el.hnjuh.cn

JS:   await fetch(url)
来源：http://mi.asd995.cn

TS:   await fetch(url)
来源：http://nl.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oa.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://hq.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bg.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dx.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://wd.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://my.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mt.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cv.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gq.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bw.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://om.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bs.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lf.asd995.cn

[L03] 设置自定义请求头
来源：http://fk.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lc.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nw.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ru.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xu.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vp.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oh.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uv.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://th.9csxet.cn

[L04] 设置超时
来源：http://vg.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://wb.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uv.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wy.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kb.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ou.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kb.yuntaijiaju.cn


<!-- 参考信息 -->