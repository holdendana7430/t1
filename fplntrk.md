代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://go.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://gl.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://hz.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ks.gzmigu.cn

JS:   e.message;  e.stack
来源：http://ed.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cq.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://na.shtwfgs.cn

Go:   err.Error()
来源：http://fr.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://mg.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://xm.huixiangedu.cn

[H09] 带错误码的异常
来源：http://qp.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lz.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://du.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oy.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wg.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hl.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xl.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dw.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cb.colortex.cn

[H10] 资源自动释放
来源：http://oe.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ev.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nn.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zl.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xn.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cj.huixiangedu.cn

Go:   defer f.Close()
来源：http://sj.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ey.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ef.shtwfgs.cn

================================================================================
来源：http://iq.huanxung.cn

I. 正则表达式
来源：http://cj.muxihuayi.cn

================================================================================
来源：http://mn.jctech888.com.cn

[I01] 判断是否匹配
来源：http://uo.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yp.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://af.colortex.cn

JS:   /\d+/.test(s)
来源：http://hg.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://vu.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uc.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kr.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://bj.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wb.jctech888.com.cn

[I02] 提取所有匹配
来源：http://tc.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://to.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oy.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hf.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://we.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://to.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ih.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://aq.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wb.chemitech.net.cn

[I03] 提取捕获分组
来源：http://uj.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xt.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ko.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://da.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xo.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ay.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://au.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sj.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kw.hahajie.cn

[I04] 正则替换
来源：http://ju.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uv.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iz.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zd.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bf.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mk.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dy.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cn.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xq.yuexingan06.cn

[I05] 按正则拆分
来源：http://ie.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ii.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xe.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://qd.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://gj.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://nr.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dg.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://iq.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gz.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tj.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xj.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bt.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vo.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ak.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kd.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pn.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://is.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ze.szxytkj.cn

[I07] 忽略大小写与多行模式
来源：http://ae.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ry.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ss.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mj.wgjwhj.cn

TS:   /error/gim
来源：http://og.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yr.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ng.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://ea.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ss.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://wb.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mx.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dq.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xc.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zy.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qw.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oo.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://di.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vh.chemitech.net.cn

================================================================================
来源：http://sy.newstarts.cn

J. 日期与时间
来源：http://uh.panjiajie.cn

================================================================================
来源：http://nq.shxzukj.cn

[J01] 获取当前时间
来源：http://ka.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yl.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fk.colortex.cn

JS:   new Date();  Date.now()
来源：http://ba.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://kr.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hb.9csxet.cn

Go:   time.Now()
来源：http://vd.shxzukj.cn

Ruby: Time.now
来源：http://ri.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ny.colortex.cn

[J02] 格式化输出
来源：http://hl.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wd.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dn.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nu.chemitech.net.cn

TS:   d.toISOString()
来源：http://vi.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fd.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dv.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ta.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pu.szsharing.cn

[J03] 字符串解析为日期
来源：http://wt.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jt.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nd.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://au.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://ad.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zz.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lr.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://fr.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uw.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://cb.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tk.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ni.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://su.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://eg.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uj.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vm.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pz.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ws.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://it.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://rh.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qj.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://js.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ml.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://sv.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vq.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://eq.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hb.nicolike.cn

[J06] 计算两时间之差
来源：http://hq.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://hs.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://pd.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://su.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gl.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ze.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://vk.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://qv.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://qw.muxihuayi.cn

[J07] 比较两个日期
来源：http://sn.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://hc.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://we.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zt.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ef.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nm.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xe.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zd.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://fw.shxzskj.cn

[J08] 提取年月日与星期
来源：http://pu.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ub.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kg.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yw.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://er.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bs.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ro.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vi.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ti.shxzskj.cn

[J09] 时区处理
来源：http://co.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bj.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zu.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aw.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nn.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ci.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cl.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kl.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jy.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://nt.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nv.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gt.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vn.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bo.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mp.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nc.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://we.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ml.yuexingan06.cn

================================================================================
来源：http://ur.shxzukj.cn

K. JSON 与序列化
来源：http://ii.nicolike.cn

================================================================================
来源：http://mi.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://fp.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://if.huixiangedu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ue.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://vh.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://ms.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ar.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://mt.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nw.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xr.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://dm.huixiangedu.cn

Py:   json.loads(s)
来源：http://pc.huixiangedu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sn.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://na.hnjuh.cn

TS:   JSON.parse(s)
来源：http://yg.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fd.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://lf.huanxung.cn

Ruby: JSON.parse(s)
来源：http://tg.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dx.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://pw.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pf.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lz.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gj.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lo.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pg.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://en.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fk.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sy.asd995.cn

[K04] 读取 JSON 文件
来源：http://pw.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tx.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vb.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kp.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nl.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://md.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pc.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wk.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hm.nicolike.cn

[K05] 深拷贝对象
来源：http://sz.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://ed.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://jj.panjiajie.cn

JS:   structuredClone(obj)
来源：http://tt.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://ra.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bo.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gd.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zc.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xa.asd995.cn

[K06] 解析 URL 查询串
来源：http://vk.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xb.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rj.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ur.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://no.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lw.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tm.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cq.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xt.chemitech.net.cn

[K07] 进制转换
来源：http://ui.shxzskj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rc.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ii.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kt.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iz.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ah.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://he.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hk.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zk.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://ll.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://ix.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kz.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ic.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://ru.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iq.nicolike.cn

Go:   encoding/gob
来源：http://ra.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://un.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qi.bookmarksfly.cn

================================================================================
来源：http://wr.huixiangedu.cn

L. 网络请求
来源：http://no.hnjuh.cn

================================================================================
来源：http://hj.hahajie.cn

[L01] 发送 GET 请求
来源：http://ek.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ue.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qz.bookmarksfly.cn

JS:   await fetch(url)
来源：http://yb.newstarts.cn

TS:   await fetch(url)
来源：http://rl.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hd.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://zi.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fe.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sj.asd995.cn

[L02] 发送 POST JSON
来源：http://fl.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ps.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jz.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fr.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ma.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qv.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jz.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zm.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tl.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://yv.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eg.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://or.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ws.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dj.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zq.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://im.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gt.asd995.cn


<!-- 参考信息 -->