代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://uc.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://ri.gzmigu.cn

[H09] 带错误码的异常
来源：http://wk.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dq.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rg.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kn.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qs.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kc.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zk.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://av.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://av.9csxet.cn

[H10] 资源自动释放
来源：http://il.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pc.shxzskj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ob.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vx.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kt.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rc.panjiajie.cn

Go:   defer f.Close()
来源：http://ch.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qx.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oy.bjjhwx.cn

================================================================================
来源：http://mv.szsharing.cn

I. 正则表达式
来源：http://yi.wgjwhj.cn

================================================================================
来源：http://it.nicolike.cn

[I01] 判断是否匹配
来源：http://to.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ih.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gw.newstarts.cn

JS:   /\d+/.test(s)
来源：http://kr.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://ic.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zl.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ua.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://hw.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ah.shxzukj.cn

[I02] 提取所有匹配
来源：http://sm.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://sy.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qh.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://du.asd995.cn

TS:   s.match(/\d+/g)
来源：http://lq.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kh.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nv.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://sk.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kq.521024.cn

[I03] 提取捕获分组
来源：http://pk.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jp.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ev.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hn.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hd.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gp.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sx.nszjky.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ia.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ef.9csxet.cn

[I04] 正则替换
来源：http://lc.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ae.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nk.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nm.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cw.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hu.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ag.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://li.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jp.hnjuh.cn

[I05] 按正则拆分
来源：http://vr.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zi.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hq.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://re.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://jj.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://yr.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ma.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://za.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rm.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kd.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kh.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uz.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zt.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ou.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fh.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://at.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dm.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://af.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://ib.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://at.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fy.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fq.9csxet.cn

TS:   /error/gim
来源：http://hk.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bs.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://at.szxytkj.cn

Ruby: s.scan(/error/i)
来源：http://db.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wv.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://az.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vl.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ux.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vj.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pp.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rx.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zl.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ry.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://we.chemitech.net.cn

================================================================================
来源：http://ug.shxzskj.cn

J. 日期与时间
来源：http://fe.newstarts.cn

================================================================================
来源：http://sy.haigaiapp.cn

[J01] 获取当前时间
来源：http://rj.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nn.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://od.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://uv.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://lx.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tb.jianghongdianzi.cn

Go:   time.Now()
来源：http://zm.nicolike.cn

Ruby: Time.now
来源：http://iw.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eh.gzmigu.cn

[J02] 格式化输出
来源：http://pa.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yj.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cb.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xh.shxzukj.cn

TS:   d.toISOString()
来源：http://nk.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oi.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xx.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ah.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kd.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://dj.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ih.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gf.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://sq.chemitech.net.cn

TS:   new Date("2024-01-02")
来源：http://ch.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mo.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kv.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://ml.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aq.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://ju.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eq.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rn.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ag.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fn.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qj.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fi.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://se.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vg.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://ig.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://kg.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pr.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zi.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eg.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://ak.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fo.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://et.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zh.szsharing.cn

[J06] 计算两时间之差
来源：http://xn.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://mb.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://ga.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ya.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zp.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ht.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://le.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://lt.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://yv.9csxet.cn

[J07] 比较两个日期
来源：http://vt.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://gm.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cr.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cr.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gu.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rf.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://it.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rh.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://nu.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://jx.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ke.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hk.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ad.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mi.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vl.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gc.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uw.bjjhwx.cn

[J09] 时区处理
来源：http://tr.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rb.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ns.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://im.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ya.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ih.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qw.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zw.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wk.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://at.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lq.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lo.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ya.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ty.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kd.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://if.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mo.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wd.bookmarksfly.cn

================================================================================
来源：http://hu.nszjky.cn

K. JSON 与序列化
来源：http://dt.lnxyls.cn

================================================================================
来源：http://az.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://ai.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rt.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uf.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://sa.huanxung.cn

TS:   JSON.stringify(obj)
来源：http://ox.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lf.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://ew.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bb.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ly.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://ss.panjiajie.cn

Py:   json.loads(s)
来源：http://bu.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vm.asd995.cn

JS:   JSON.parse(s)
来源：http://gp.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://la.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bo.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://ds.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://ne.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://my.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://ad.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://et.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fi.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rk.szxytkj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://aj.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ai.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://md.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uh.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bb.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://ab.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dr.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wh.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ba.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wv.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://md.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wx.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ii.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hx.jctech888.com.cn

[K05] 深拷贝对象
来源：http://pd.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://li.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://rj.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://xr.hahajie.cn

TS:   structuredClone(obj)
来源：http://fl.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jl.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ri.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ov.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tc.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://kk.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ci.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ny.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ju.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ey.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xw.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pz.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://da.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pw.newstarts.cn

[K07] 进制转换
来源：http://bl.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uu.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ck.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zz.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cl.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ms.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ol.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xn.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://so.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://bj.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://tt.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qe.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://qd.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://uz.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nm.yuntaijiaju.cn

Go:   encoding/gob
来源：http://kl.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://fo.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jw.nszjky.cn

================================================================================
来源：http://yj.szsharing.cn

L. 网络请求
来源：http://ql.szxytkj.cn

================================================================================
来源：http://sw.asd995.cn

[L01] 发送 GET 请求
来源：http://yk.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sa.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kj.newstarts.cn

JS:   await fetch(url)
来源：http://wa.shxzskj.cn

TS:   await fetch(url)
来源：http://sn.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xu.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://jz.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xp.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bk.521024.cn

[L02] 发送 POST JSON
来源：http://kw.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ny.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ob.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vt.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ja.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xu.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oj.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ge.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sy.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://wo.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hf.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ct.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mx.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kq.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mw.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dj.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nb.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://co.haigaiapp.cn

[L04] 设置超时
来源：http://mq.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://vl.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ec.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oi.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bg.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lo.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lo.szxytkj.cn


<!-- 参考信息 -->