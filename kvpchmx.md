代发 wailian999

JS:   e.message;  e.stack
来源：http://lg.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uv.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zv.jctech888.com.cn

Go:   err.Error()
来源：http://gw.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://vu.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://nk.haigaiapp.cn

[H09] 带错误码的异常
来源：http://ow.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://je.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gz.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dx.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dn.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ab.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bx.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yi.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fk.shtwfgs.cn

[H10] 资源自动释放
来源：http://dg.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ok.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uf.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fb.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ns.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lv.asd995.cn

Go:   defer f.Close()
来源：http://po.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sv.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bv.muxihuayi.cn

================================================================================
来源：http://cs.colortex.cn

I. 正则表达式
来源：http://zi.lnxyls.cn

================================================================================
来源：http://kg.lnxyls.cn

[I01] 判断是否匹配
来源：http://de.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gd.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gh.nicolike.cn

JS:   /\d+/.test(s)
来源：http://jn.521024.cn

TS:   /\d+/.test(s)
来源：http://ph.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lm.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ff.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://en.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zh.shtwfgs.cn

[I02] 提取所有匹配
来源：http://gr.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://rc.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ml.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mz.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://in.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qx.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ns.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://qq.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oq.asd995.cn

[I03] 提取捕获分组
来源：http://fi.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hf.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zc.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ic.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iw.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ne.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bo.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kq.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vq.521024.cn

[I04] 正则替换
来源：http://dq.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cv.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fs.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yw.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hw.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yw.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://eh.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://he.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fu.shxzukj.cn

[I05] 按正则拆分
来源：http://qn.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://at.521024.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ub.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://fr.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://wf.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://sl.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bg.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wu.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dg.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ku.bookmarksfly.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ny.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gf.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ck.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wo.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dm.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lv.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jq.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://px.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://ct.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ue.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ct.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bk.huixinmuqiang.cn

TS:   /error/gim
来源：http://si.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ov.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kq.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://we.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fz.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://ac.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://io.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jw.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qz.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ix.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rk.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gy.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ku.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hy.shxzskj.cn

================================================================================
来源：http://ki.haigaiapp.cn

J. 日期与时间
来源：http://ls.shtwfgs.cn

================================================================================
来源：http://vu.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://sc.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://li.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://as.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://go.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://yc.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jh.szsharing.cn

Go:   time.Now()
来源：http://sh.muxihuayi.cn

Ruby: Time.now
来源：http://re.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eo.szsharing.cn

[J02] 格式化输出
来源：http://bv.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zd.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tf.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jr.shxzukj.cn

TS:   d.toISOString()
来源：http://qb.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gj.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nv.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ta.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cj.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://dq.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yi.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xv.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://ze.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://qu.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fu.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mk.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://xi.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mk.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://uq.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bs.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gy.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fe.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://am.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ml.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ps.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rh.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ai.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://ou.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://zr.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jl.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mg.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dc.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://rj.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://th.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://sq.szsharing.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ix.shtwfgs.cn

[J06] 计算两时间之差
来源：http://dg.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://sv.521024.cn

PHP:  $end->diff($start)->days;
来源：http://sb.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bf.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nx.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sh.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://aj.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://st.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://jk.jctech888.com.cn

[J07] 比较两个日期
来源：http://fy.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://av.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wl.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ny.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ac.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ob.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qi.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vv.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://fk.nicolike.cn

[J08] 提取年月日与星期
来源：http://sr.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zi.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dv.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bn.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lv.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://el.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lm.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ex.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ls.lnxyls.cn

[J09] 时区处理
来源：http://kv.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ll.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gx.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gy.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wt.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bj.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qg.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ky.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ap.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://is.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fo.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fu.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xh.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://us.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ik.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tw.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://di.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ow.bjjhwx.cn

================================================================================
来源：http://ee.shtwfgs.cn

K. JSON 与序列化
来源：http://iu.nszjky.cn

================================================================================
来源：http://yw.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://mb.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ql.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uj.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://rw.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://ai.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iq.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://zv.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ky.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ie.nicolike.cn

[K02] JSON 字符串转对象
来源：http://nl.hnjuh.cn

Py:   json.loads(s)
来源：http://hs.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://up.hnjuh.cn

JS:   JSON.parse(s)
来源：http://vj.hahajie.cn

TS:   JSON.parse(s)
来源：http://ze.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://of.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://zr.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://ls.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yl.bookmarksfly.cn

[K03] JSON 美化输出（带缩进）
来源：http://rr.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sx.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bg.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hi.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fi.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ig.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hc.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sg.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://os.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://zg.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ft.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yl.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ah.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oc.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kl.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lb.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hg.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sh.wgjwhj.cn

[K05] 深拷贝对象
来源：http://tb.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://sg.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://ad.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://oj.lnxyls.cn

TS:   structuredClone(obj)
来源：http://oa.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ds.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qt.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mw.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pm.9csxet.cn

[K06] 解析 URL 查询串
来源：http://sd.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qt.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mr.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aq.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oa.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lt.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ih.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tt.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oz.shxzskj.cn

[K07] 进制转换
来源：http://zu.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sa.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ha.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://au.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xi.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qt.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oa.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jr.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pv.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://nm.521024.cn

Py:   pickle.dumps(obj)
来源：http://yt.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qw.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://el.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://ad.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jn.9csxet.cn

Go:   encoding/gob
来源：http://nu.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://in.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uj.nszjky.cn

================================================================================
来源：http://pc.chemitech.net.cn

L. 网络请求
来源：http://zw.hahajie.cn

================================================================================
来源：http://ve.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://tz.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ek.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xp.521024.cn

JS:   await fetch(url)
来源：http://nn.szxytkj.cn

TS:   await fetch(url)
来源：http://gi.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qm.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://dv.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dd.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gb.hahajie.cn

[L02] 发送 POST JSON
来源：http://lv.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cu.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wn.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zf.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sh.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ip.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lb.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xp.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kw.nszjky.cn

[L03] 设置自定义请求头
来源：http://od.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xp.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vf.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ot.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eb.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hk.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wc.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://st.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rx.muxihuayi.cn

[L04] 设置超时
来源：http://nm.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://dz.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rt.chemitech.net.cn


<!-- 参考信息 -->