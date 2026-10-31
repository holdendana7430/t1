代发 wailian999

TS:   console.assert(x > 0);
来源：http://ar.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://nv.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oc.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vg.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://hz.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://lb.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://sk.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lm.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://vr.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tj.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ol.haigaiapp.cn

Go:   err.Error()
来源：http://fm.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://xx.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://gv.bjjhwx.cn

[H09] 带错误码的异常
来源：http://um.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lg.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bf.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ad.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fd.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gs.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kt.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vv.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wx.colortex.cn

[H10] 资源自动释放
来源：http://dz.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cy.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://po.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sq.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wn.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yy.szxytkj.cn

Go:   defer f.Close()
来源：http://ok.gzmigu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://md.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wh.bookmarksfly.cn

================================================================================
来源：http://ta.panjiajie.cn

I. 正则表达式
来源：http://fn.huanxung.cn

================================================================================
来源：http://vd.asd995.cn

[I01] 判断是否匹配
来源：http://pw.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oi.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wb.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://qn.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://hh.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://um.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wj.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://yk.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xb.bjjhwx.cn

[I02] 提取所有匹配
来源：http://vm.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://xw.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zc.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rt.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://fe.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fg.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ku.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://ro.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ki.jctech888.com.cn

[I03] 提取捕获分组
来源：http://fa.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://td.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mp.nszjky.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fh.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yi.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wl.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qx.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nr.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ei.shxzukj.cn

[I04] 正则替换
来源：http://kr.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kc.huanxung.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vn.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gp.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ys.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ub.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gm.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xh.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bb.hahajie.cn

[I05] 按正则拆分
来源：http://sd.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ox.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ps.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://kj.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://em.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://oz.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pp.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ji.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rd.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ih.bookmarksfly.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eu.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://of.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ay.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jz.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ln.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mo.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hc.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bb.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://ol.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mv.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://de.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://we.colortex.cn

TS:   /error/gim
来源：http://ia.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wb.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ak.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://jf.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qr.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://jv.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cq.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://om.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://on.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gq.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xx.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rx.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://re.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qp.hahajie.cn

================================================================================
来源：http://tl.nicolike.cn

J. 日期与时间
来源：http://tp.jctech888.com.cn

================================================================================
来源：http://bx.lnxyls.cn

[J01] 获取当前时间
来源：http://qw.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lb.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sg.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://sy.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://np.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pt.nicolike.cn

Go:   time.Now()
来源：http://jv.nszjky.cn

Ruby: Time.now
来源：http://mo.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sy.szxytkj.cn

[J02] 格式化输出
来源：http://uw.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rx.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ej.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sk.szxytkj.cn

TS:   d.toISOString()
来源：http://yk.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://em.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pq.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bu.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tv.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://jr.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jq.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gu.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://wf.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://eu.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cf.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xa.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://fk.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yo.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://xm.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://px.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xl.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mv.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ll.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zc.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lz.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ha.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://io.521024.cn

[J05] 时间加减（加 7 天）
来源：http://zn.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://em.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qi.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bt.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ku.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://nq.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zy.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://xh.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nm.szsharing.cn

[J06] 计算两时间之差
来源：http://et.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://as.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://ix.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xp.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://of.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tj.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://wt.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://iv.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://mr.nicolike.cn

[J07] 比较两个日期
来源：http://iq.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://wm.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ez.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jr.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iu.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zu.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ss.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xj.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://su.hahajie.cn

[J08] 提取年月日与星期
来源：http://va.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qx.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xk.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://te.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xa.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iq.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://io.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rw.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fs.huixiangedu.cn

[J09] 时区处理
来源：http://vh.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://po.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eb.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ba.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ad.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ti.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hq.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tk.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vs.521024.cn

[J10] 取今天 / 本月第一天
来源：http://lx.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://am.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ca.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xd.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zk.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jq.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zq.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zq.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kb.lnxyls.cn

================================================================================
来源：http://bm.colortex.cn

K. JSON 与序列化
来源：http://jl.bjjhwx.cn

================================================================================
来源：http://mk.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://rh.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cx.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tc.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://ob.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://kc.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zg.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://ac.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zf.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jv.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://xz.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://zl.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uf.asd995.cn

JS:   JSON.parse(s)
来源：http://fe.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://oc.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ze.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://kt.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://ny.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://kl.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lg.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dp.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wl.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://er.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qg.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fy.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ja.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://od.szsharing.cn

[K04] 读取 JSON 文件
来源：http://em.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oo.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://go.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hs.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ry.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pn.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hm.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fy.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vg.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://nk.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://qq.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://aa.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://wn.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://fe.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yk.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zd.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sv.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sh.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://rs.huixinmuqiang.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kk.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gn.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uw.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jc.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yg.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pl.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wo.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hd.shtwfgs.cn

[K07] 进制转换
来源：http://oi.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rv.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mf.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xp.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yo.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zv.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ce.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gb.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://en.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://tm.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://ex.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://eo.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://uw.yuexingan06.cn

TS:   v8.serialize(obj)        // Node
来源：http://cm.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zp.jctech888.com.cn

Go:   encoding/gob
来源：http://yi.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://hb.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cc.huixiangedu.cn

================================================================================
来源：http://zb.521024.cn

L. 网络请求
来源：http://ml.chemitech.net.cn

================================================================================
来源：http://rf.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://vs.shxzukj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wf.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wi.chemitech.net.cn

JS:   await fetch(url)
来源：http://se.newstarts.cn

TS:   await fetch(url)
来源：http://px.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nt.521024.cn

Go:   resp, err := http.Get(url)
来源：http://om.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qo.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hr.nszjky.cn

[L02] 发送 POST JSON
来源：http://la.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fg.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rc.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rt.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ua.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hd.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iv.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xp.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tx.shxzukj.cn

[L03] 设置自定义请求头
来源：http://wf.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ft.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xh.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hw.newstarts.cn


<!-- 参考信息 -->