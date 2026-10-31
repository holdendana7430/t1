代发 wailian999

JS:   e.message;  e.stack
来源：http://ff.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sm.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tf.szsharing.cn

Go:   err.Error()
来源：http://cw.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://xh.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://hx.huanxung.cn

[H09] 带错误码的异常
来源：http://ag.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vu.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bp.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ea.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vt.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fg.szsharing.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://op.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cg.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bn.nszjky.cn

[H10] 资源自动释放
来源：http://uz.bjjhwx.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jj.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cd.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qc.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ht.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mi.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://dw.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gn.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gt.shxzukj.cn

================================================================================
来源：http://dv.lnxyls.cn

I. 正则表达式
来源：http://xj.hahajie.cn

================================================================================
来源：http://qy.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://jp.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vf.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mw.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://pi.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://qn.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nc.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ck.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://kd.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mv.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://ay.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://zj.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://in.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://at.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://pp.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jx.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://be.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://xf.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sp.nicolike.cn

[I03] 提取捕获分组
来源：http://sg.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://px.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ez.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://py.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dm.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dw.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kv.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jd.haigaiapp.cn

[I04] 正则替换
来源：http://th.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uf.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zy.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://af.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ag.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nn.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vy.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lt.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ph.hnjuh.cn

[I05] 按正则拆分
来源：http://oy.9csxet.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zu.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kw.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://pz.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://ov.nicolike.cn

Java: s.split("\\s*,\\s*")
来源：http://dm.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ui.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tb.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bz.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xy.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xq.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zq.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oz.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qm.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kg.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ip.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vq.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iv.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://be.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gg.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zk.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xf.hnjuh.cn

TS:   /error/gim
来源：http://ly.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sl.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cl.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://tb.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wt.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://qr.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://um.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cn.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rp.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ds.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nu.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yx.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cb.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://av.yuntaijiaju.cn

================================================================================
来源：http://ks.newstarts.cn

J. 日期与时间
来源：http://bq.newstarts.cn

================================================================================
来源：http://ba.muxihuayi.cn

[J01] 获取当前时间
来源：http://zu.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qx.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rb.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://di.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://ak.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wu.szsharing.cn

Go:   time.Now()
来源：http://dd.yuntaijiaju.cn

Ruby: Time.now
来源：http://qz.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xv.nszjky.cn

[J02] 格式化输出
来源：http://dy.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cb.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eh.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zq.gzmigu.cn

TS:   d.toISOString()
来源：http://rz.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fd.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yw.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ad.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oq.nszjky.cn

[J03] 字符串解析为日期
来源：http://nf.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wc.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rv.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://oi.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://tn.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uu.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fh.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://jj.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yt.asd995.cn

[J04] 时间戳与日期互转
来源：http://gb.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://td.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gp.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://te.lnxyls.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nb.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ih.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hu.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qh.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tz.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://xk.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://up.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://of.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rp.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ca.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://ce.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rf.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://fl.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pk.huixiangedu.cn

[J06] 计算两时间之差
来源：http://ph.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://al.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://vo.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bc.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://om.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ei.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://ki.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://ub.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://xn.colortex.cn

[J07] 比较两个日期
来源：http://ah.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://gg.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xu.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ak.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://az.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qz.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bw.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xz.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://kv.newstarts.cn

[J08] 提取年月日与星期
来源：http://qp.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tq.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kb.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ar.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ku.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cq.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tv.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ju.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cu.nszjky.cn

[J09] 时区处理
来源：http://xa.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ph.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jr.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iw.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vw.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cc.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cx.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fm.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://al.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://yp.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nt.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wi.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wj.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ra.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sv.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bz.shxzukj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://io.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ns.muxihuayi.cn

================================================================================
来源：http://li.nszjky.cn

K. JSON 与序列化
来源：http://kg.jctech888.com.cn

================================================================================
来源：http://yn.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://wd.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wu.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hp.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://zi.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://fh.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ee.521024.cn

Go:   json.Marshal(obj)
来源：http://xp.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gi.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ps.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://kb.haigaiapp.cn

Py:   json.loads(s)
来源：http://wg.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gg.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://fx.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://vu.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lv.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://of.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://le.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pq.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://zp.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qv.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ad.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yf.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ti.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bk.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lh.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://im.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ud.521024.cn

[K04] 读取 JSON 文件
来源：http://kk.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fd.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cp.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pg.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://er.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mw.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hb.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fv.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zj.hnjuh.cn

[K05] 深拷贝对象
来源：http://go.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://ps.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://dm.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://ds.huanxung.cn

TS:   structuredClone(obj)
来源：http://lq.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tr.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dl.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rs.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pz.colortex.cn

[K06] 解析 URL 查询串
来源：http://hv.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://li.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uu.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ls.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eb.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mn.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://um.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xh.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hf.huixinmuqiang.cn

[K07] 进制转换
来源：http://dh.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ub.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pa.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://et.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pj.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lc.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xy.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ry.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://up.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://dx.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://ur.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yi.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://ul.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://an.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vt.yuexingan06.cn

Go:   encoding/gob
来源：http://af.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://ik.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xd.shxzskj.cn

================================================================================
来源：http://kr.panjiajie.cn

L. 网络请求
来源：http://jy.bookmarksfly.cn

================================================================================
来源：http://ol.hnjuh.cn

[L01] 发送 GET 请求
来源：http://lx.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hl.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gf.nicolike.cn

JS:   await fetch(url)
来源：http://qi.bookmarksfly.cn

TS:   await fetch(url)
来源：http://qs.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zz.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://yj.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mr.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ud.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://pw.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yq.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uk.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lf.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ik.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ii.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zb.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pw.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mt.panjiajie.cn

[L03] 设置自定义请求头
来源：http://tc.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vp.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ps.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cf.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gi.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fs.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bb.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ow.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zi.wgjwhj.cn

[L04] 设置超时
来源：http://kn.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://mz.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gu.jctech888.com.cn


<!-- 参考信息 -->