代发 wailian999

JS:   e.message;  e.stack
来源：http://en.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ab.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sl.hahajie.cn

Go:   err.Error()
来源：http://yq.panjiajie.cn

Ruby: e.message;  e.backtrace
来源：http://ti.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://dk.muxihuayi.cn

[H09] 带错误码的异常
来源：http://uf.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ab.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://en.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ci.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lr.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yb.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ql.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mt.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cq.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://wp.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://le.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jf.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tx.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eo.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jq.panjiajie.cn

Go:   defer f.Close()
来源：http://cm.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ek.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sv.hnjuh.cn

================================================================================
来源：http://qn.shxzskj.cn

I. 正则表达式
来源：http://nk.newstarts.cn

================================================================================
来源：http://vf.yuexingan06.cn

[I01] 判断是否匹配
来源：http://mq.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fq.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nr.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://rb.huixiangedu.cn

TS:   /\d+/.test(s)
来源：http://yi.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vi.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yo.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://zb.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dy.szxytkj.cn

[I02] 提取所有匹配
来源：http://mi.szsharing.cn

Py:   re.findall(r"\d+", s)
来源：http://uy.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qt.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ci.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://bb.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tq.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cr.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://jj.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mh.nicolike.cn

[I03] 提取捕获分组
来源：http://ej.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ap.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bl.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hn.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qj.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ce.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hp.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yq.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zu.yuntaijiaju.cn

[I04] 正则替换
来源：http://il.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gk.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ab.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uh.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uh.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gw.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jo.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vd.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://at.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://st.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dj.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uo.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://uc.hahajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://fp.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://up.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jv.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sl.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oq.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://do.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nu.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qq.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fr.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://by.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vg.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://om.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://em.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nw.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://xg.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ki.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eh.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zq.bookmarksfly.cn

TS:   /error/gim
来源：http://km.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yj.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dv.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://rq.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vu.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://jh.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pr.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ls.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bf.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bo.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zr.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kn.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://py.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vf.huixiangedu.cn

================================================================================
来源：http://mo.nszjky.cn

J. 日期与时间
来源：http://sp.shxzskj.cn

================================================================================
来源：http://pg.bjjhwx.cn

[J01] 获取当前时间
来源：http://zb.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://es.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xq.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://dx.newstarts.cn

TS:   new Date();  Date.now()
来源：http://up.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://no.hnjuh.cn

Go:   time.Now()
来源：http://td.colortex.cn

Ruby: Time.now
来源：http://lc.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xc.bjjhwx.cn

[J02] 格式化输出
来源：http://ti.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gc.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mz.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pw.huixiangedu.cn

TS:   d.toISOString()
来源：http://pn.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lg.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vj.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fy.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ah.9csxet.cn

[J03] 字符串解析为日期
来源：http://zm.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qf.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://we.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://fx.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://ek.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qh.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tr.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ja.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nj.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://ei.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tc.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://my.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://te.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mc.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tq.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gk.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wv.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ku.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://zn.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://qn.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xb.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://co.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sx.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://gw.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cw.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://wo.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wo.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://io.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://lh.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://tf.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sy.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dy.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xs.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://il.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://ch.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://vt.szxytkj.cn

[J07] 比较两个日期
来源：http://jj.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://ih.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kq.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lq.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ky.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pf.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mr.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yn.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://mm.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://gg.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xc.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nj.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yg.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rc.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ig.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nx.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fq.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qo.newstarts.cn

[J09] 时区处理
来源：http://pk.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ah.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pg.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ti.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yr.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iz.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dq.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yr.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://df.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://jb.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cd.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cp.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jl.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ss.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bs.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yl.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ki.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bf.yuntaijiaju.cn

================================================================================
来源：http://pk.szsharing.cn

K. JSON 与序列化
来源：http://vv.jianghongdianzi.cn

================================================================================
来源：http://la.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://pr.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sq.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dz.colortex.cn

JS:   JSON.stringify(obj)
来源：http://oq.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://cn.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://av.huanxung.cn

Go:   json.Marshal(obj)
来源：http://ve.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://po.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qz.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://yu.shxzukj.cn

Py:   json.loads(s)
来源：http://bu.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vi.hnjuh.cn

JS:   JSON.parse(s)
来源：http://bw.hahajie.cn

TS:   JSON.parse(s)
来源：http://bp.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mv.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://rv.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://wj.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ir.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://go.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oy.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uv.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ol.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ll.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lq.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rq.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://im.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kv.521024.cn

[K04] 读取 JSON 文件
来源：http://li.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xe.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gs.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://we.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qy.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kr.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ua.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://km.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gz.shtwfgs.cn

[K05] 深拷贝对象
来源：http://bb.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://zb.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://nl.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://yk.hnjuh.cn

TS:   structuredClone(obj)
来源：http://km.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fo.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yj.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pu.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xg.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://td.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ug.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gm.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vx.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jl.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ev.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zs.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vi.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lf.huixinmuqiang.cn

[K07] 进制转换
来源：http://sh.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://st.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yu.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fp.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mo.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aj.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fc.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oj.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://se.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://nx.bjjhwx.cn

Py:   pickle.dumps(obj)
来源：http://th.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yo.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://wz.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://kt.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ps.haigaiapp.cn

Go:   encoding/gob
来源：http://xr.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://zd.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sa.huixinmuqiang.cn

================================================================================
来源：http://zq.szsharing.cn

L. 网络请求
来源：http://lm.chemitech.net.cn

================================================================================
来源：http://bk.shxzskj.cn

[L01] 发送 GET 请求
来源：http://ix.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gg.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vt.shtwfgs.cn

JS:   await fetch(url)
来源：http://sp.bjjhwx.cn

TS:   await fetch(url)
来源：http://nt.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xm.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://wc.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://em.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ao.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://bc.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hb.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ya.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jl.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vj.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pm.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dj.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rm.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vw.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://vs.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jb.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rp.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pg.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pc.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ck.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ai.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tx.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://av.huanxung.cn

[L04] 设置超时
来源：http://vn.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://dq.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yf.521024.cn


<!-- 参考信息 -->