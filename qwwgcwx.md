代发 wailian999

JS:   e.message;  e.stack
来源：http://qh.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xg.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gq.colortex.cn

Go:   err.Error()
来源：http://ng.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://yp.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://on.muxihuayi.cn

[H09] 带错误码的异常
来源：http://wt.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ec.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cs.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cp.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jk.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kx.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ck.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wg.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://je.bjjhwx.cn

[H10] 资源自动释放
来源：http://lj.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ei.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dm.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ev.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://as.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yu.huanxung.cn

Go:   defer f.Close()
来源：http://fr.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hg.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ru.shxzukj.cn

================================================================================
来源：http://ba.gzmigu.cn

I. 正则表达式
来源：http://ws.lnxyls.cn

================================================================================
来源：http://gc.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://mi.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iw.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zt.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://gi.shxzukj.cn

TS:   /\d+/.test(s)
来源：http://rp.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iq.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cu.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://zz.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bn.shxzskj.cn

[I02] 提取所有匹配
来源：http://rc.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://zl.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ca.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tz.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://bp.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://io.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vj.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://vt.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gq.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://rv.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gd.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fd.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aw.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qh.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fh.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pl.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ir.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ml.newstarts.cn

[I04] 正则替换
来源：http://qe.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ye.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ew.lnxyls.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tc.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ud.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ho.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://na.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://li.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ka.chemitech.net.cn

[I05] 按正则拆分
来源：http://er.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ih.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dc.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://yu.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://wo.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://za.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dd.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://at.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dv.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ir.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wy.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://je.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wz.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zg.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mi.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cs.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nx.bjjhwx.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rb.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://uu.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pc.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://im.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wp.panjiajie.cn

TS:   /error/gim
来源：http://gl.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hs.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://en.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://hj.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wq.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://ol.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ft.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uh.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ro.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ie.bookmarksfly.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gb.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yr.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pv.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kt.jianghongdianzi.cn

================================================================================
来源：http://vi.hahajie.cn

J. 日期与时间
来源：http://zs.jianghongdianzi.cn

================================================================================
来源：http://ho.shxzskj.cn

[J01] 获取当前时间
来源：http://ri.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ji.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://la.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://cd.9csxet.cn

TS:   new Date();  Date.now()
来源：http://ml.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cn.hnjuh.cn

Go:   time.Now()
来源：http://iy.hnjuh.cn

Ruby: Time.now
来源：http://oi.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wd.bookmarksfly.cn

[J02] 格式化输出
来源：http://vf.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wy.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gt.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zp.shxzukj.cn

TS:   d.toISOString()
来源：http://iu.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vm.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://to.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nz.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cp.nszjky.cn

[J03] 字符串解析为日期
来源：http://ov.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ro.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kh.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://um.521024.cn

TS:   new Date("2024-01-02")
来源：http://he.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://oc.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dk.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://iz.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hy.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://vo.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dw.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ao.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qg.lnxyls.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tk.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wt.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ue.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bb.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cn.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://ew.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://zm.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://se.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sy.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sn.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://en.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xx.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://lh.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dd.asd995.cn

[J06] 计算两时间之差
来源：http://yn.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://de.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://rf.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mn.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bd.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gx.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://zq.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://kp.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://cd.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://uh.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://vu.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ty.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kd.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ix.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nd.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jt.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tu.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://bw.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://vl.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yn.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xm.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://js.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ip.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://js.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ef.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zy.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://az.yuntaijiaju.cn

[J09] 时区处理
来源：http://sa.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yd.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wn.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fn.yuntaijiaju.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jl.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sv.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yf.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://st.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://or.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://pb.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cg.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://st.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vx.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ie.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ot.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wm.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tq.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ma.colortex.cn

================================================================================
来源：http://fm.yuntaijiaju.cn

K. JSON 与序列化
来源：http://ox.9csxet.cn

================================================================================
来源：http://fb.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://ln.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jd.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://el.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://zd.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://ln.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yq.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://dc.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gr.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gm.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://wq.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://ce.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tf.colortex.cn

JS:   JSON.parse(s)
来源：http://kw.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://wy.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ss.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://ol.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://ag.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fx.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://hj.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kn.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lq.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://at.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://iz.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dl.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uo.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gv.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://io.colortex.cn

[K04] 读取 JSON 文件
来源：http://jt.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cq.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gh.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tb.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ik.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dl.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kn.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dz.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ci.shxzskj.cn

[K05] 深拷贝对象
来源：http://xh.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://yp.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://wy.shxzskj.cn

JS:   structuredClone(obj)
来源：http://ns.shxzukj.cn

TS:   structuredClone(obj)
来源：http://iz.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ie.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lg.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://un.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zd.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://wd.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ss.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ny.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pm.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oh.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ye.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://my.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sh.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yr.521024.cn

[K07] 进制转换
来源：http://jo.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pa.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cy.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gr.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hd.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kn.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uw.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://od.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://if.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://gh.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://ip.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mk.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://tk.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://bz.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://th.muxihuayi.cn

Go:   encoding/gob
来源：http://eu.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://uh.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://am.yuexingan06.cn

================================================================================
来源：http://hj.szsharing.cn

L. 网络请求
来源：http://xg.yuexingan06.cn

================================================================================
来源：http://we.shxzukj.cn

[L01] 发送 GET 请求
来源：http://ux.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pj.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pt.shtwfgs.cn

JS:   await fetch(url)
来源：http://re.lnxyls.cn

TS:   await fetch(url)
来源：http://ib.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pn.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://wr.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mz.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mf.newstarts.cn

[L02] 发送 POST JSON
来源：http://ut.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bl.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ay.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xu.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ve.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jp.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://of.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gt.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ye.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://tp.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wb.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fv.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fq.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lh.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ya.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qp.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ld.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sd.panjiajie.cn

[L04] 设置超时
来源：http://zm.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://rp.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://as.panjiajie.cn


<!-- 参考信息 -->