代发 wailian999

TS:   console.assert(x > 0);
来源：http://xu.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://eh.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://as.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qn.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://cb.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://rp.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://dl.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qm.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://pc.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bw.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://md.muxihuayi.cn

Go:   err.Error()
来源：http://vu.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://md.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://ca.nicolike.cn

[H09] 带错误码的异常
来源：http://uh.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bv.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hi.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fh.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pp.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sb.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://df.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://va.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fl.nszjky.cn

[H10] 资源自动释放
来源：http://ym.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ju.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kx.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vz.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wu.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vz.9csxet.cn

Go:   defer f.Close()
来源：http://rh.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yi.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://be.newstarts.cn

================================================================================
来源：http://uz.gzmigu.cn

I. 正则表达式
来源：http://tn.newstarts.cn

================================================================================
来源：http://va.lnxyls.cn

[I01] 判断是否匹配
来源：http://be.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ca.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fn.nszjky.cn

JS:   /\d+/.test(s)
来源：http://jt.shxzukj.cn

TS:   /\d+/.test(s)
来源：http://sg.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cw.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://us.521024.cn

Ruby: s.match?(/\d+/)
来源：http://ix.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xm.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://bp.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://ow.hnjuh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sn.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://or.521024.cn

TS:   s.match(/\d+/g)
来源：http://vy.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dl.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ay.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://gl.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://by.nszjky.cn

[I03] 提取捕获分组
来源：http://yo.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fh.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ud.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ic.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://we.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gi.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nh.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://km.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bt.shxzskj.cn

[I04] 正则替换
来源：http://qs.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oe.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aw.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ir.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ex.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ly.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xh.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bq.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cz.hahajie.cn

[I05] 按正则拆分
来源：http://xc.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lg.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ly.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://nn.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://pu.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://ci.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cp.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://aa.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iq.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ap.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://an.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wa.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vy.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yt.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tg.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://te.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hu.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nh.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://ui.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ov.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bd.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zk.hahajie.cn

TS:   /error/gim
来源：http://nt.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://an.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ql.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://wc.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://md.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://jj.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rd.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kg.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pb.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://it.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dv.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jl.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lr.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ed.huixiangedu.cn

================================================================================
来源：http://ev.huixiangedu.cn

J. 日期与时间
来源：http://pc.hahajie.cn

================================================================================
来源：http://kz.shxzskj.cn

[J01] 获取当前时间
来源：http://ei.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pj.szsharing.cn

JS:   new Date();  Date.now()
来源：http://ts.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://jp.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ot.gzmigu.cn

Go:   time.Now()
来源：http://mo.szsharing.cn

Ruby: Time.now
来源：http://kr.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://te.yuexingan06.cn

[J02] 格式化输出
来源：http://ht.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qu.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zf.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://de.szsharing.cn

TS:   d.toISOString()
来源：http://dz.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pm.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hg.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ak.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vo.nicolike.cn

[J03] 字符串解析为日期
来源：http://bt.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://of.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dg.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://dx.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://xs.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mu.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tm.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://sx.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wj.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://hg.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ox.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nj.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dz.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yc.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fe.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yd.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lq.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ss.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://eb.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://tk.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zz.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xp.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lt.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://mw.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ws.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://qz.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vh.szxytkj.cn

[J06] 计算两时间之差
来源：http://nu.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://ki.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://no.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kd.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rk.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qn.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://nx.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://zk.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://il.chemitech.net.cn

[J07] 比较两个日期
来源：http://qw.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://cx.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gm.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ud.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iy.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ig.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hc.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qg.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://id.panjiajie.cn

[J08] 提取年月日与星期
来源：http://rr.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wx.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zb.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yi.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oc.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bb.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://re.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lj.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rc.shtwfgs.cn

[J09] 时区处理
来源：http://pr.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xw.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ot.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dz.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hd.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sz.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dq.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://py.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zs.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://ep.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zs.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jb.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ay.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hw.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tk.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xo.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zu.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jn.bjjhwx.cn

================================================================================
来源：http://su.hnjuh.cn

K. JSON 与序列化
来源：http://op.hahajie.cn

================================================================================
来源：http://db.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://zs.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://se.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ny.asd995.cn

JS:   JSON.stringify(obj)
来源：http://ac.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://dp.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hd.bjjhwx.cn

Go:   json.Marshal(obj)
来源：http://hd.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vj.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bw.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://im.szsharing.cn

Py:   json.loads(s)
来源：http://wi.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fe.colortex.cn

JS:   JSON.parse(s)
来源：http://oo.nicolike.cn

TS:   JSON.parse(s)
来源：http://oh.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://je.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://ts.newstarts.cn

Ruby: JSON.parse(s)
来源：http://gv.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ki.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://od.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lh.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ey.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pb.szxytkj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yt.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sy.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ds.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ja.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ke.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://kh.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ar.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dc.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zi.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ud.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pf.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kd.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qc.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hw.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://rq.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://hm.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://iz.nszjky.cn

JS:   structuredClone(obj)
来源：http://zl.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://td.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ww.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://me.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gt.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tq.asd995.cn

[K06] 解析 URL 查询串
来源：http://so.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mi.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kh.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mg.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zo.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yy.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hc.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yk.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wn.lnxyls.cn

[K07] 进制转换
来源：http://ke.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jg.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bt.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zu.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nz.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://if.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ze.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mm.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gb.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://gb.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://eu.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yz.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://rz.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://sw.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mx.newstarts.cn

Go:   encoding/gob
来源：http://ft.bookmarksfly.cn

Ruby: Marshal.dump(obj)
来源：http://mq.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ms.panjiajie.cn

================================================================================
来源：http://eo.yuexingan06.cn

L. 网络请求
来源：http://wi.gzmigu.cn

================================================================================
来源：http://ul.9csxet.cn

[L01] 发送 GET 请求
来源：http://dk.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ko.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ah.jctech888.com.cn

JS:   await fetch(url)
来源：http://qd.lnxyls.cn

TS:   await fetch(url)
来源：http://ah.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tn.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://oc.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yw.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zc.gzmigu.cn

[L02] 发送 POST JSON
来源：http://cq.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bh.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gy.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lw.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xi.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sp.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vk.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fq.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gt.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://tf.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ka.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ar.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ec.newstarts.cn


<!-- 参考信息 -->