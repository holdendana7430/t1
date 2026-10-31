代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://sk.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://dg.szxytkj.cn

[H09] 带错误码的异常
来源：http://ao.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nx.yuexingan06.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lc.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sk.9csxet.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jm.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vw.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wl.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lp.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oh.hahajie.cn

[H10] 资源自动释放
来源：http://he.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qy.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sm.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qt.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oy.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sy.gzmigu.cn

Go:   defer f.Close()
来源：http://tf.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aa.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pm.szsharing.cn

================================================================================
来源：http://po.huixinmuqiang.cn

I. 正则表达式
来源：http://ip.9csxet.cn

================================================================================
来源：http://we.newstarts.cn

[I01] 判断是否匹配
来源：http://rb.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mb.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ec.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://er.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://jp.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gu.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yu.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://oz.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://il.nszjky.cn

[I02] 提取所有匹配
来源：http://di.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://lk.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dv.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lo.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://pc.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wq.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rl.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://vs.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jw.wgjwhj.cn

[I03] 提取捕获分组
来源：http://ou.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://px.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ku.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wp.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ww.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xs.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cf.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kv.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://su.bookmarksfly.cn

[I04] 正则替换
来源：http://pi.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tm.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vx.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://er.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gu.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dp.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ty.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wu.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jo.asd995.cn

[I05] 按正则拆分
来源：http://bv.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ey.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sh.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://rz.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://ic.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://vg.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nm.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ws.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tn.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yq.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sp.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xl.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://it.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vs.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://th.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qy.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jp.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lt.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://zz.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cj.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://di.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bc.hnjuh.cn

TS:   /error/gim
来源：http://ix.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fs.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://np.szxytkj.cn

Ruby: s.scan(/error/i)
来源：http://iu.521024.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sl.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://kr.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ny.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ro.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xz.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oa.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xy.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://id.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cl.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ml.huanxung.cn

================================================================================
来源：http://sc.haigaiapp.cn

J. 日期与时间
来源：http://rm.jianghongdianzi.cn

================================================================================
来源：http://ys.wgjwhj.cn

[J01] 获取当前时间
来源：http://pr.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vw.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lq.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://pj.9csxet.cn

TS:   new Date();  Date.now()
来源：http://gq.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nh.9csxet.cn

Go:   time.Now()
来源：http://iq.szsharing.cn

Ruby: Time.now
来源：http://mz.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hp.lnxyls.cn

[J02] 格式化输出
来源：http://oa.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gy.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nt.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hc.szsharing.cn

TS:   d.toISOString()
来源：http://lf.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://od.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vm.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://no.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rx.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://qs.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tj.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rf.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://jb.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://jl.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xz.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zu.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://wo.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ol.521024.cn

[J04] 时间戳与日期互转
来源：http://nu.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tv.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hh.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://er.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nv.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pu.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yj.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kl.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://km.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://ea.asd995.cn

Py:   now + timedelta(days=7)
来源：http://fw.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ao.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kg.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oj.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://vr.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fr.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://su.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yh.shxzukj.cn

[J06] 计算两时间之差
来源：http://ol.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://kg.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://zo.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ns.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fs.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ku.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://qv.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://jv.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://tx.szsharing.cn

[J07] 比较两个日期
来源：http://vq.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://cn.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sy.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fc.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://or.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://th.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zh.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jz.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://tq.huanxung.cn

[J08] 提取年月日与星期
来源：http://sw.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uu.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eo.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gw.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gp.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wq.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lu.huixiangedu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://po.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ox.shxzskj.cn

[J09] 时区处理
来源：http://jk.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ch.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tx.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wi.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zd.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ev.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xp.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gb.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jz.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://zu.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jl.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zm.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nc.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ih.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mv.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ne.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nj.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bf.lnxyls.cn

================================================================================
来源：http://bj.panjiajie.cn

K. JSON 与序列化
来源：http://kp.panjiajie.cn

================================================================================
来源：http://ry.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://rr.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ho.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nw.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://fb.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://vf.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yp.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://xy.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kg.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://eb.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://gu.shxzskj.cn

Py:   json.loads(s)
来源：http://qk.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mv.9csxet.cn

JS:   JSON.parse(s)
来源：http://wg.szxytkj.cn

TS:   JSON.parse(s)
来源：http://oh.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vg.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://mb.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://xi.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cj.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://jk.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ns.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://da.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://we.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cs.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dk.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tf.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ec.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ot.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://uz.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uj.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nd.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sa.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fz.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zm.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ts.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://he.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rn.gzmigu.cn

[K05] 深拷贝对象
来源：http://mv.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://ak.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://qn.asd995.cn

JS:   structuredClone(obj)
来源：http://ue.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://ml.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yb.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ri.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bm.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vg.newstarts.cn

[K06] 解析 URL 查询串
来源：http://ym.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gs.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oi.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ok.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bc.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fw.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hk.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wo.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qj.szsharing.cn

[K07] 进制转换
来源：http://fs.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ip.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nx.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cn.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rp.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://os.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bs.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ov.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hl.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://rr.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://yg.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ho.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://gu.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://mt.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://go.huixiangedu.cn

Go:   encoding/gob
来源：http://hk.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://fa.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xs.521024.cn

================================================================================
来源：http://lz.yuntaijiaju.cn

L. 网络请求
来源：http://pe.lnxyls.cn

================================================================================
来源：http://bt.gzmigu.cn

[L01] 发送 GET 请求
来源：http://ao.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hs.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tr.wgjwhj.cn

JS:   await fetch(url)
来源：http://ym.jctech888.com.cn

TS:   await fetch(url)
来源：http://kg.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lv.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://pw.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cn.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rk.nszjky.cn

[L02] 发送 POST JSON
来源：http://nl.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://aa.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ot.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://in.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tl.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://td.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ky.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tz.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vk.521024.cn

[L03] 设置自定义请求头
来源：http://mk.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nb.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mt.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sc.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ce.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tp.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://em.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lh.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gc.gzmigu.cn

[L04] 设置超时
来源：http://db.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://nh.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ry.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fu.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iv.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qw.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qw.shxzskj.cn


<!-- 参考信息 -->