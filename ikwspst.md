代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://ie.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://vr.haigaiapp.cn

[H09] 带错误码的异常
来源：http://fw.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jb.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yv.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ys.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://as.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://te.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yd.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ru.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qp.lnxyls.cn

[H10] 资源自动释放
来源：http://da.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fb.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tn.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fh.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qj.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fp.shxzskj.cn

Go:   defer f.Close()
来源：http://tc.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://if.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ai.9csxet.cn

================================================================================
来源：http://lr.gzmigu.cn

I. 正则表达式
来源：http://so.gzmigu.cn

================================================================================
来源：http://xa.huixiangedu.cn

[I01] 判断是否匹配
来源：http://oj.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qw.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nx.shtwfgs.cn

JS:   /\d+/.test(s)
来源：http://zm.szsharing.cn

TS:   /\d+/.test(s)
来源：http://ve.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lg.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rl.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://bx.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qz.jctech888.com.cn

[I02] 提取所有匹配
来源：http://xv.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://wx.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qp.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zg.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://zw.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sv.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dl.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://le.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ds.newstarts.cn

[I03] 提取捕获分组
来源：http://ue.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ui.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ub.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pg.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mr.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oj.9csxet.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lh.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ez.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pj.521024.cn

[I04] 正则替换
来源：http://ug.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nz.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cp.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ce.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jz.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yp.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gf.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gq.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jv.muxihuayi.cn

[I05] 按正则拆分
来源：http://ya.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rt.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ph.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://sk.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://ra.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://zd.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uj.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cw.muxihuayi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zl.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nw.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://od.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lg.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://po.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aw.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ap.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ft.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dr.hnjuh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uo.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://mu.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://em.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ee.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wv.haigaiapp.cn

TS:   /error/gim
来源：http://sr.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jw.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rg.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://dj.szsharing.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jz.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://um.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://px.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gh.shxzukj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qa.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://le.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rs.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ko.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jj.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://na.bookmarksfly.cn

================================================================================
来源：http://qy.lnxyls.cn

J. 日期与时间
来源：http://ow.521024.cn

================================================================================
来源：http://un.gzmigu.cn

[J01] 获取当前时间
来源：http://vz.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yt.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qf.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://jd.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://rr.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ua.hahajie.cn

Go:   time.Now()
来源：http://is.lnxyls.cn

Ruby: Time.now
来源：http://az.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mb.huixinmuqiang.cn

[J02] 格式化输出
来源：http://ve.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zb.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qk.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mp.nszjky.cn

TS:   d.toISOString()
来源：http://gp.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lr.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lf.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ob.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vt.521024.cn

[J03] 字符串解析为日期
来源：http://gg.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yx.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xx.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://bq.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://pe.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rl.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vl.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://op.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pd.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://vq.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ho.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ns.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ze.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ph.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vc.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jq.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://co.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gf.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://nl.521024.cn

Py:   now + timedelta(days=7)
来源：http://wb.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xv.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qq.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zu.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://yi.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fx.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://fq.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://js.yuexingan06.cn

[J06] 计算两时间之差
来源：http://rn.asd995.cn

Py:   (end - start).total_seconds()
来源：http://bp.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://vj.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uv.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wf.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wp.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://ff.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://uk.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://nz.9csxet.cn

[J07] 比较两个日期
来源：http://fz.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://eg.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gg.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tc.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vb.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ig.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ez.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mn.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://lg.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://ac.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ey.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bl.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://is.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ct.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gw.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ia.huixiangedu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ob.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oo.nszjky.cn

[J09] 时区处理
来源：http://xj.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yq.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pk.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://at.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uu.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uk.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qm.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qo.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nd.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://xz.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yw.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://so.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pn.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hx.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ij.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zy.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pa.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://st.bookmarksfly.cn

================================================================================
来源：http://hg.nszjky.cn

K. JSON 与序列化
来源：http://wb.bookmarksfly.cn

================================================================================
来源：http://yu.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://yt.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nw.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mt.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://xj.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://hl.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dg.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://ly.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oq.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uy.newstarts.cn

[K02] JSON 字符串转对象
来源：http://cq.szxytkj.cn

Py:   json.loads(s)
来源：http://rw.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fm.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://bw.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://bd.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://km.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://pz.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://pm.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xw.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://ab.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ln.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jl.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://aw.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dm.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nf.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iw.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zi.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yd.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://ac.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jw.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://he.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zt.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rr.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://os.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wp.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zx.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jo.huixiangedu.cn

[K05] 深拷贝对象
来源：http://lb.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://vi.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://ea.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://yd.newstarts.cn

TS:   structuredClone(obj)
来源：http://ww.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ji.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://as.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jj.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kw.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://yw.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yd.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tk.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cw.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pl.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pm.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ke.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://we.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wh.huixiangedu.cn

[K07] 进制转换
来源：http://os.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zx.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sj.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ns.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ws.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xr.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hb.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://po.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cd.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://kr.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://hb.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hj.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://cy.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://am.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yj.bjjhwx.cn

Go:   encoding/gob
来源：http://ny.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://zk.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xh.colortex.cn

================================================================================
来源：http://ug.huixinmuqiang.cn

L. 网络请求
来源：http://qx.nszjky.cn

================================================================================
来源：http://wf.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://tf.newstarts.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ri.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wx.nicolike.cn

JS:   await fetch(url)
来源：http://we.shtwfgs.cn

TS:   await fetch(url)
来源：http://ck.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qj.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://ro.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jy.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oc.huanxung.cn

[L02] 发送 POST JSON
来源：http://bv.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mu.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yx.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ft.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yf.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nj.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zp.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lm.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fj.szxytkj.cn

[L03] 设置自定义请求头
来源：http://mu.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vx.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ce.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uq.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xj.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tc.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ev.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://il.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kw.huixinmuqiang.cn

[L04] 设置超时
来源：http://gp.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://uu.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bq.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xg.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://co.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fb.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://np.shxzukj.cn


<!-- 参考信息 -->