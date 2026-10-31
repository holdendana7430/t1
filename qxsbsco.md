代发 wailian999

JS:   e.message;  e.stack
来源：http://wm.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fv.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hp.muxihuayi.cn

Go:   err.Error()
来源：http://ht.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://hz.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://ty.yuexingan06.cn

[H09] 带错误码的异常
来源：http://fm.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mi.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fz.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fc.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gk.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mo.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dh.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fc.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://td.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://sw.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xf.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qr.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hl.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zw.asd995.cn

Go:   defer f.Close()
来源：http://ko.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qp.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dc.huixiangedu.cn

================================================================================
来源：http://tg.asd995.cn

I. 正则表达式
来源：http://kn.chemitech.net.cn

================================================================================
来源：http://vq.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://po.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ae.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bo.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://ii.nicolike.cn

TS:   /\d+/.test(s)
来源：http://xf.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rp.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://de.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://ut.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bf.muxihuayi.cn

[I02] 提取所有匹配
来源：http://fl.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://xh.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mc.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nq.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://ot.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cd.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dy.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://wp.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sy.hnjuh.cn

[I03] 提取捕获分组
来源：http://mi.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ur.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bv.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qe.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kv.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sq.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tj.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rg.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gl.chemitech.net.cn

[I04] 正则替换
来源：http://cz.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wt.huanxung.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://go.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eb.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qx.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sj.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oe.chemitech.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ow.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ir.muxihuayi.cn

[I05] 按正则拆分
来源：http://oz.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://as.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kq.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://si.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://lf.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://il.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vp.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://is.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pu.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sk.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fk.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lf.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gq.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fa.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gi.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://db.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fb.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sk.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://gh.szxytkj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nb.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ew.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wf.yuexingan06.cn

TS:   /error/gim
来源：http://rh.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tg.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bc.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://xv.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eo.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://aq.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cs.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fh.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ih.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xu.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lf.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hd.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://de.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rd.bjjhwx.cn

================================================================================
来源：http://sq.lnxyls.cn

J. 日期与时间
来源：http://bs.nszjky.cn

================================================================================
来源：http://bs.newstarts.cn

[J01] 获取当前时间
来源：http://yr.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ym.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qx.newstarts.cn

JS:   new Date();  Date.now()
来源：http://wy.521024.cn

TS:   new Date();  Date.now()
来源：http://mc.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ab.jianghongdianzi.cn

Go:   time.Now()
来源：http://gu.yuexingan06.cn

Ruby: Time.now
来源：http://nc.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wp.521024.cn

[J02] 格式化输出
来源：http://es.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ns.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xv.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://um.lnxyls.cn

TS:   d.toISOString()
来源：http://sh.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ff.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://im.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pf.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xz.szxytkj.cn

[J03] 字符串解析为日期
来源：http://gj.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wz.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cr.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://vi.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://jo.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kj.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mf.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://lm.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nk.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://oy.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bv.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fk.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jf.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bw.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ae.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rn.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dw.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gc.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://fw.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://nm.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ci.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yk.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ss.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://ob.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fz.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://vz.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ip.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://sd.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://tk.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://dv.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rw.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pa.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gf.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://pi.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://nj.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://fi.haigaiapp.cn

[J07] 比较两个日期
来源：http://eb.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://me.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kz.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://na.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hn.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://if.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vz.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sk.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://jc.colortex.cn

[J08] 提取年月日与星期
来源：http://xx.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nb.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ke.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mi.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://je.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mn.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ni.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hu.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bs.gzmigu.cn

[J09] 时区处理
来源：http://ip.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://me.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ns.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ol.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fk.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tc.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://il.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tx.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qv.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://iz.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yj.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ww.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ew.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ej.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dk.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jo.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pb.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zr.wgjwhj.cn

================================================================================
来源：http://oi.szsharing.cn

K. JSON 与序列化
来源：http://kp.szxytkj.cn

================================================================================
来源：http://ij.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://pd.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qr.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hd.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://yu.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://en.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uk.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://xa.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://by.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xs.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://ig.muxihuayi.cn

Py:   json.loads(s)
来源：http://yz.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fi.hnjuh.cn

JS:   JSON.parse(s)
来源：http://rc.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://is.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jm.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://wh.colortex.cn

Ruby: JSON.parse(s)
来源：http://uv.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xl.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://qg.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hi.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tq.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://og.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://za.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ea.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pu.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dn.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qv.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://sg.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kq.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cd.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qz.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pq.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qq.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yq.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gb.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ri.nszjky.cn

[K05] 深拷贝对象
来源：http://al.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://dn.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://nn.shxzukj.cn

JS:   structuredClone(obj)
来源：http://ld.asd995.cn

TS:   structuredClone(obj)
来源：http://vz.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ia.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://on.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pc.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wn.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://jo.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qt.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qz.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://am.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gl.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://it.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ew.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dp.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uu.nszjky.cn

[K07] 进制转换
来源：http://ts.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tz.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pi.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://de.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gb.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bi.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dc.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mw.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xz.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://xw.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://in.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ig.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://ek.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://mn.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ox.chemitech.net.cn

Go:   encoding/gob
来源：http://ha.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://gb.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://su.hahajie.cn

================================================================================
来源：http://ul.wgjwhj.cn

L. 网络请求
来源：http://jg.shxzukj.cn

================================================================================
来源：http://sx.newstarts.cn

[L01] 发送 GET 请求
来源：http://ko.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ud.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zy.chemitech.net.cn

JS:   await fetch(url)
来源：http://tw.gzmigu.cn

TS:   await fetch(url)
来源：http://hv.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://to.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://xv.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nr.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vc.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://gk.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://om.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gc.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dn.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yd.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fn.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ym.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ni.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hf.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://pc.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tr.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://br.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ug.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wj.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rb.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ln.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qn.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nh.huixinmuqiang.cn

[L04] 设置超时
来源：http://qu.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://vh.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xn.huixiangedu.cn


<!-- 参考信息 -->