代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://yv.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://gh.nszjky.cn

[H09] 带错误码的异常
来源：http://wv.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zg.hnjuh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lh.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ik.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zb.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://td.asd995.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ks.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sr.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ps.colortex.cn

[H10] 资源自动释放
来源：http://fj.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rw.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fu.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rd.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://am.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://du.wgjwhj.cn

Go:   defer f.Close()
来源：http://bz.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://az.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xp.muxihuayi.cn

================================================================================
来源：http://ed.yuntaijiaju.cn

I. 正则表达式
来源：http://jg.shxzskj.cn

================================================================================
来源：http://am.shxzskj.cn

[I01] 判断是否匹配
来源：http://dg.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zk.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rf.colortex.cn

JS:   /\d+/.test(s)
来源：http://sh.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://ln.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mb.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vv.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://xh.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gw.huanxung.cn

[I02] 提取所有匹配
来源：http://ji.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://gp.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dx.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xk.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://vx.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bu.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tf.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://ms.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ul.asd995.cn

[I03] 提取捕获分组
来源：http://rx.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lp.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wk.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xh.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pd.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vc.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://om.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rs.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lq.asd995.cn

[I04] 正则替换
来源：http://sx.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uy.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jy.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://oz.huanxung.cn

TS:   s.replace(/\d+/g, "#")
来源：http://li.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ha.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ek.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wv.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nd.yuexingan06.cn

[I05] 按正则拆分
来源：http://cm.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jg.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yf.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://kf.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://xw.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://jl.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bb.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tj.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dy.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vc.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ne.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ix.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zn.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cm.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ns.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zd.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zw.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xn.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://rg.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xk.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kv.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sz.wgjwhj.cn

TS:   /error/gim
来源：http://vv.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zl.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://im.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://rc.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ho.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://wa.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qh.yuntaijiaju.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://os.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zn.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kg.yuntaijiaju.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ie.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gd.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jb.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ny.jctech888.com.cn

================================================================================
来源：http://dd.shxzskj.cn

J. 日期与时间
来源：http://ac.haigaiapp.cn

================================================================================
来源：http://bf.haigaiapp.cn

[J01] 获取当前时间
来源：http://ia.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ii.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ir.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://pk.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://pa.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ck.panjiajie.cn

Go:   time.Now()
来源：http://iy.wgjwhj.cn

Ruby: Time.now
来源：http://kc.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ty.muxihuayi.cn

[J02] 格式化输出
来源：http://nt.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dd.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qm.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pl.newstarts.cn

TS:   d.toISOString()
来源：http://dv.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lf.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tf.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bb.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ck.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://fb.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vi.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fw.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://qz.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://dk.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wy.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sb.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://zk.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fl.newstarts.cn

[J04] 时间戳与日期互转
来源：http://vi.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jx.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vh.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jd.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ns.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sa.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pl.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zz.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://as.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://js.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://rk.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uq.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bc.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lf.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://dy.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tx.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://uo.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ph.asd995.cn

[J06] 计算两时间之差
来源：http://xu.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://qg.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://cf.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tx.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ws.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bd.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://li.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://dw.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://cd.muxihuayi.cn

[J07] 比较两个日期
来源：http://xe.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://ip.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ld.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ui.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ni.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lu.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fh.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uu.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://oz.lnxyls.cn

[J08] 提取年月日与星期
来源：http://ov.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ef.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dc.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xd.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://du.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pm.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qj.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uo.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qu.lnxyls.cn

[J09] 时区处理
来源：http://yu.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gp.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://im.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ue.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ii.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xp.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vt.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mc.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hq.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://pv.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nk.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://za.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lb.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uo.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qq.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rn.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ek.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ol.wgjwhj.cn

================================================================================
来源：http://rb.huixiangedu.cn

K. JSON 与序列化
来源：http://la.szsharing.cn

================================================================================
来源：http://vl.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://rn.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ia.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jn.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://wx.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://cm.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://te.huanxung.cn

Go:   json.Marshal(obj)
来源：http://va.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ty.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ap.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://ci.hahajie.cn

Py:   json.loads(s)
来源：http://px.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fv.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://do.newstarts.cn

TS:   JSON.parse(s)
来源：http://wq.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yp.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://gw.newstarts.cn

Ruby: JSON.parse(s)
来源：http://hf.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ss.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://az.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wt.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yh.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bf.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jq.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ti.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jo.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lt.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rp.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://ak.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bd.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fu.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ah.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kc.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://is.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gd.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tf.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://le.asd995.cn

[K05] 深拷贝对象
来源：http://tb.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://yj.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://xx.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://dr.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://km.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gr.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gt.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tk.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qj.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://hs.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://og.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mk.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://es.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sy.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jr.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vq.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jk.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qk.lnxyls.cn

[K07] 进制转换
来源：http://jt.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ph.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hh.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ux.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dj.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ml.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iz.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ce.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://na.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://se.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://kw.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uv.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://yq.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://jg.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jc.lnxyls.cn

Go:   encoding/gob
来源：http://bv.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://ts.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kk.hnjuh.cn

================================================================================
来源：http://zn.hahajie.cn

L. 网络请求
来源：http://kn.szsharing.cn

================================================================================
来源：http://dq.huixinmuqiang.cn

[L01] 发送 GET 请求
来源：http://nm.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uh.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fl.yuexingan06.cn

JS:   await fetch(url)
来源：http://bs.colortex.cn

TS:   await fetch(url)
来源：http://vp.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ut.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://gt.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lv.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ij.newstarts.cn

[L02] 发送 POST JSON
来源：http://eo.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zh.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ao.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://am.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ij.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cr.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://di.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ea.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://le.gzmigu.cn

[L03] 设置自定义请求头
来源：http://tw.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rx.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vj.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hp.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vz.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nx.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ry.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ph.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wk.szsharing.cn

[L04] 设置超时
来源：http://fh.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://qr.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xx.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oq.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mp.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fx.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xn.szxytkj.cn


<!-- 参考信息 -->