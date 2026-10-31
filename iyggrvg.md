代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://jf.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://gc.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://gp.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vm.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gh.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ip.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dz.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fv.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rh.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ci.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bs.szxytkj.cn

[H10] 资源自动释放
来源：http://wi.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gq.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://al.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yt.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lp.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lh.521024.cn

Go:   defer f.Close()
来源：http://fx.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qv.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qk.szxytkj.cn

================================================================================
来源：http://hv.yuntaijiaju.cn

I. 正则表达式
来源：http://ei.lnxyls.cn

================================================================================
来源：http://rm.szsharing.cn

[I01] 判断是否匹配
来源：http://sm.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yn.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wn.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://cw.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://bp.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://is.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rv.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://kh.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://af.huixiangedu.cn

[I02] 提取所有匹配
来源：http://yn.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://jj.huanxung.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nr.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bd.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://qv.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bm.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cg.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://fb.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jf.shtwfgs.cn

[I03] 提取捕获分组
来源：http://jr.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dh.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sw.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oj.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hr.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nx.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pl.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rd.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rp.newstarts.cn

[I04] 正则替换
来源：http://ic.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://df.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://du.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ah.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://he.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gx.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lh.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://la.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jj.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://vg.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kk.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zn.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://oy.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://vc.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://nm.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jm.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sj.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tp.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bm.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jq.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mq.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pu.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lz.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ws.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sg.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ex.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wk.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://bw.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ir.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ef.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jo.9csxet.cn

TS:   /error/gim
来源：http://di.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qg.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nl.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://jn.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hy.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://jj.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vd.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dk.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eq.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zo.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qh.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hd.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qn.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://os.huixinmuqiang.cn

================================================================================
来源：http://ec.9csxet.cn

J. 日期与时间
来源：http://in.521024.cn

================================================================================
来源：http://qa.shtwfgs.cn

[J01] 获取当前时间
来源：http://rb.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cb.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zs.newstarts.cn

JS:   new Date();  Date.now()
来源：http://cw.newstarts.cn

TS:   new Date();  Date.now()
来源：http://ca.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vr.huanxung.cn

Go:   time.Now()
来源：http://pc.lnxyls.cn

Ruby: Time.now
来源：http://zf.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ku.muxihuayi.cn

[J02] 格式化输出
来源：http://kg.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vv.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://di.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nw.asd995.cn

TS:   d.toISOString()
来源：http://al.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dc.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sd.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hq.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sd.szsharing.cn

[J03] 字符串解析为日期
来源：http://xb.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zy.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bb.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://zt.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://sa.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kt.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zi.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://vu.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://up.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://ts.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xq.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ri.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uh.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ma.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uh.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ll.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yq.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dv.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://ud.asd995.cn

Py:   now + timedelta(days=7)
来源：http://ju.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fp.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kq.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ne.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://ud.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ka.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://ig.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gn.newstarts.cn

[J06] 计算两时间之差
来源：http://kx.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://pn.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://je.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fc.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://or.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ek.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://po.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://wv.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://vl.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://qk.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://va.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hn.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://py.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fq.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ig.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ql.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yk.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://qs.9csxet.cn

[J08] 提取年月日与星期
来源：http://ye.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ww.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xr.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uw.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://te.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sw.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sq.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://py.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xa.gzmigu.cn

[J09] 时区处理
来源：http://zg.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vs.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hg.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zc.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aa.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vj.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ph.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qn.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ls.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://yn.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pv.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://it.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zn.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zo.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hg.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ub.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://us.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pp.panjiajie.cn

================================================================================
来源：http://qt.lnxyls.cn

K. JSON 与序列化
来源：http://kd.panjiajie.cn

================================================================================
来源：http://az.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://ui.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wb.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gz.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://rs.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://sy.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ip.521024.cn

Go:   json.Marshal(obj)
来源：http://mz.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ie.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zh.huanxung.cn

[K02] JSON 字符串转对象
来源：http://fz.lnxyls.cn

Py:   json.loads(s)
来源：http://ic.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rf.szxytkj.cn

JS:   JSON.parse(s)
来源：http://ha.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://en.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pn.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://au.huanxung.cn

Ruby: JSON.parse(s)
来源：http://my.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fk.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://jk.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sx.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ay.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sc.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://au.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cd.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://le.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mw.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ge.521024.cn

[K04] 读取 JSON 文件
来源：http://we.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lw.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kz.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mj.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lt.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tt.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sh.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ux.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://og.nszjky.cn

[K05] 深拷贝对象
来源：http://vy.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://ut.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://mv.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://ch.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://tt.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rs.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zf.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jc.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jy.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://cr.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ct.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tn.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gu.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yl.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dj.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jz.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://og.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qh.521024.cn

[K07] 进制转换
来源：http://qg.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dv.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pk.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://im.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hw.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uj.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ag.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ni.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jh.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://cm.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://gi.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vn.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://sj.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://si.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://do.jctech888.com.cn

Go:   encoding/gob
来源：http://ij.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://xi.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ad.haigaiapp.cn

================================================================================
来源：http://ob.bookmarksfly.cn

L. 网络请求
来源：http://cg.newstarts.cn

================================================================================
来源：http://ba.lnxyls.cn

[L01] 发送 GET 请求
来源：http://dg.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://za.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yx.lnxyls.cn

JS:   await fetch(url)
来源：http://ux.chemitech.net.cn

TS:   await fetch(url)
来源：http://bq.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bg.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://mj.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zp.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gh.nicolike.cn

[L02] 发送 POST JSON
来源：http://ml.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vx.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sp.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hi.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gz.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ww.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kj.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://io.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://sf.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cx.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jy.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dx.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gn.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uu.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ag.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ix.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qt.bookmarksfly.cn

[L04] 设置超时
来源：http://eh.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://lo.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iv.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ro.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sf.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zk.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vh.newstarts.cn


<!-- 参考信息 -->