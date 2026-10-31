代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://bw.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://fw.asd995.cn

[H09] 带错误码的异常
来源：http://zy.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sl.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pj.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bk.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vz.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mf.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vz.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eo.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tq.gzmigu.cn

[H10] 资源自动释放
来源：http://xz.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dm.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ss.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tx.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wc.nicolike.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dt.chemitech.net.cn

Go:   defer f.Close()
来源：http://dz.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lq.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kb.huixiangedu.cn

================================================================================
来源：http://kp.colortex.cn

I. 正则表达式
来源：http://el.yuntaijiaju.cn

================================================================================
来源：http://co.bjjhwx.cn

[I01] 判断是否匹配
来源：http://wg.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rd.bookmarksfly.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xg.asd995.cn

JS:   /\d+/.test(s)
来源：http://ft.9csxet.cn

TS:   /\d+/.test(s)
来源：http://ro.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tp.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hn.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://xd.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sf.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://vn.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://qt.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pv.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qv.521024.cn

TS:   s.match(/\d+/g)
来源：http://km.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sv.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hd.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://ts.muxihuayi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://st.muxihuayi.cn

[I03] 提取捕获分组
来源：http://ng.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xf.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rw.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jr.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wd.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ql.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fq.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gs.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ov.nszjky.cn

[I04] 正则替换
来源：http://gt.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ni.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bz.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ih.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://er.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gx.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ez.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://po.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cf.muxihuayi.cn

[I05] 按正则拆分
来源：http://td.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://te.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hj.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://qq.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://mz.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://ij.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hf.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gr.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ej.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qo.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wn.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ym.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hi.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ei.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xl.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://so.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bd.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qe.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://kk.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tu.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hl.gzmigu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gj.yuexingan06.cn

TS:   /error/gim
来源：http://gu.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zl.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ag.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://el.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ds.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://qi.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ui.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://it.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ll.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fd.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hr.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://up.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zr.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ef.bookmarksfly.cn

================================================================================
来源：http://hd.asd995.cn

J. 日期与时间
来源：http://gd.panjiajie.cn

================================================================================
来源：http://pb.hnjuh.cn

[J01] 获取当前时间
来源：http://fv.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bv.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tf.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://zq.hahajie.cn

TS:   new Date();  Date.now()
来源：http://es.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dp.chemitech.net.cn

Go:   time.Now()
来源：http://fz.bookmarksfly.cn

Ruby: Time.now
来源：http://zl.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ko.521024.cn

[J02] 格式化输出
来源：http://ob.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dj.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wz.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gu.newstarts.cn

TS:   d.toISOString()
来源：http://jk.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ee.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ms.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yb.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xv.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://gz.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://du.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wg.colortex.cn

JS:   new Date("2024-01-02")
来源：http://lt.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://qh.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zf.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pf.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://rx.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qp.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://mr.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qy.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ve.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lx.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ac.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wm.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hu.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jp.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://go.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://cu.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://dw.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ie.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wr.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ha.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://aa.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dg.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://me.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hn.jctech888.com.cn

[J06] 计算两时间之差
来源：http://mk.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://ry.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://cj.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://df.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wu.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wj.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://bb.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://qy.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://fu.panjiajie.cn

[J07] 比较两个日期
来源：http://ah.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://yn.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ut.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bb.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pl.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iz.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pq.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wi.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://nq.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://od.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eo.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hy.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ai.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://if.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vl.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qz.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zg.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fw.asd995.cn

[J09] 时区处理
来源：http://xu.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gf.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pe.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dt.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xd.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sr.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bt.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fh.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hc.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://xi.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ud.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ox.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qc.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vc.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fc.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eq.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sq.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pk.nszjky.cn

================================================================================
来源：http://zd.shxzskj.cn

K. JSON 与序列化
来源：http://un.newstarts.cn

================================================================================
来源：http://wb.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://pj.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yt.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dy.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://xq.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://ov.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ot.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://cy.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nt.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rv.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://je.jctech888.com.cn

Py:   json.loads(s)
来源：http://uq.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gj.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://gc.newstarts.cn

TS:   JSON.parse(s)
来源：http://rg.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nq.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://ap.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://uq.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ul.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://bb.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hc.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://me.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pd.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uq.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vl.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ro.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://eh.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zc.hahajie.cn

[K04] 读取 JSON 文件
来源：http://ys.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hf.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ca.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lj.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gr.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hn.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sh.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dw.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cq.shxzukj.cn

[K05] 深拷贝对象
来源：http://gg.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://py.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://az.asd995.cn

JS:   structuredClone(obj)
来源：http://wp.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://dt.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lr.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kp.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pe.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://od.colortex.cn

[K06] 解析 URL 查询串
来源：http://dd.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sm.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mk.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lh.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wv.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ux.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gg.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rt.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lu.bjjhwx.cn

[K07] 进制转换
来源：http://px.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pt.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://am.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zk.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ai.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gi.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cy.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sa.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sq.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://zm.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://qt.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xw.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://cy.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://pz.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ai.gzmigu.cn

Go:   encoding/gob
来源：http://hp.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://fx.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mg.gzmigu.cn

================================================================================
来源：http://nt.shxzskj.cn

L. 网络请求
来源：http://sy.9csxet.cn

================================================================================
来源：http://rf.szxytkj.cn

[L01] 发送 GET 请求
来源：http://ah.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xm.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fp.wgjwhj.cn

JS:   await fetch(url)
来源：http://sr.newstarts.cn

TS:   await fetch(url)
来源：http://jj.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jg.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://ek.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nj.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vs.hahajie.cn

[L02] 发送 POST JSON
来源：http://fc.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cv.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nm.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ea.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sw.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vq.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nd.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jq.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lz.nszjky.cn

[L03] 设置自定义请求头
来源：http://cv.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://di.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ca.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ce.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kd.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ux.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pl.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kc.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qq.hahajie.cn

[L04] 设置超时
来源：http://rj.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://ii.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hk.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sg.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ha.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wg.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vw.yuexingan06.cn


<!-- 参考信息 -->