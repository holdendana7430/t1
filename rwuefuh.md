代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://el.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://jv.szsharing.cn

[H09] 带错误码的异常
来源：http://mn.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pt.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ef.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hp.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rv.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lo.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rm.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jp.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xn.shtwfgs.cn

[H10] 资源自动释放
来源：http://hf.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cs.shxzskj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sj.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fi.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oj.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ol.jctech888.com.cn

Go:   defer f.Close()
来源：http://qy.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ni.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://np.shtwfgs.cn

================================================================================
来源：http://vx.nszjky.cn

I. 正则表达式
来源：http://ql.muxihuayi.cn

================================================================================
来源：http://em.yuexingan06.cn

[I01] 判断是否匹配
来源：http://le.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yf.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://at.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://dx.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://us.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://da.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zn.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://mx.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yp.muxihuayi.cn

[I02] 提取所有匹配
来源：http://yw.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://hi.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hq.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rd.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://an.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yd.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wn.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://rr.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rx.hnjuh.cn

[I03] 提取捕获分组
来源：http://sf.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nn.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dq.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pb.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jg.wgjwhj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mg.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wj.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ua.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fk.panjiajie.cn

[I04] 正则替换
来源：http://kb.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zp.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://us.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cq.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://za.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yk.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oy.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ld.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cq.bjjhwx.cn

[I05] 按正则拆分
来源：http://nb.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mt.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://od.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://uo.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://tc.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://ot.bookmarksfly.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gz.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xp.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sy.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gi.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ql.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pl.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hn.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kp.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gy.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zg.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ga.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ws.szxytkj.cn

[I07] 忽略大小写与多行模式
来源：http://sj.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oz.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lj.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vh.yuexingan06.cn

TS:   /error/gim
来源：http://ky.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ax.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pb.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://nc.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fs.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://zz.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pg.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xz.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fu.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mv.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vt.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://of.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yc.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vp.nszjky.cn

================================================================================
来源：http://ve.huixiangedu.cn

J. 日期与时间
来源：http://ky.shtwfgs.cn

================================================================================
来源：http://sr.asd995.cn

[J01] 获取当前时间
来源：http://nk.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kv.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kr.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://bo.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://oi.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uo.asd995.cn

Go:   time.Now()
来源：http://tl.huanxung.cn

Ruby: Time.now
来源：http://do.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://if.huixinmuqiang.cn

[J02] 格式化输出
来源：http://wv.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xe.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pa.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ci.nszjky.cn

TS:   d.toISOString()
来源：http://sj.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pu.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://um.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gs.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ia.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://ak.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://us.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ys.asd995.cn

JS:   new Date("2024-01-02")
来源：http://rc.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://gl.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zx.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://el.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://wx.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cb.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://wu.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jv.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oj.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fg.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wb.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://au.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zb.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ic.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bz.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://ny.521024.cn

Py:   now + timedelta(days=7)
来源：http://av.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rf.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://me.bookmarksfly.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wz.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://fi.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mm.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://lp.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ck.haigaiapp.cn

[J06] 计算两时间之差
来源：http://uf.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://fx.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://lz.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qg.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qp.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xj.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://xs.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://we.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://bk.9csxet.cn

[J07] 比较两个日期
来源：http://of.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://ap.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qe.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gn.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zk.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ft.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zb.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://el.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://sy.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://vp.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zf.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lu.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ry.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dx.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cn.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://li.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nx.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jb.bookmarksfly.cn

[J09] 时区处理
来源：http://dy.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ro.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dr.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sy.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bm.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ev.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://em.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lu.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tn.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://mc.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yv.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yk.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ju.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ag.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sh.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wm.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yn.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tj.haigaiapp.cn

================================================================================
来源：http://ea.jctech888.com.cn

K. JSON 与序列化
来源：http://tb.huixiangedu.cn

================================================================================
来源：http://ms.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://zh.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kk.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://op.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://kp.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://ef.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fe.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://bs.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ta.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rx.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://tw.yuexingan06.cn

Py:   json.loads(s)
来源：http://lq.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uy.colortex.cn

JS:   JSON.parse(s)
来源：http://rv.panjiajie.cn

TS:   JSON.parse(s)
来源：http://is.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wv.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://ky.9csxet.cn

Ruby: JSON.parse(s)
来源：http://vt.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kr.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://wp.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://es.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ni.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vi.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://aa.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cu.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://az.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hn.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wg.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://xm.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ws.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vm.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qf.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ke.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qb.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ah.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mx.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://at.chemitech.net.cn

[K05] 深拷贝对象
来源：http://tc.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://zf.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://ag.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://at.9csxet.cn

TS:   structuredClone(obj)
来源：http://px.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ct.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ad.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wg.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ec.nicolike.cn

[K06] 解析 URL 查询串
来源：http://ir.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oi.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pu.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ei.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ap.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nh.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yh.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ll.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sf.jianghongdianzi.cn

[K07] 进制转换
来源：http://eg.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://em.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uy.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bt.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dz.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ep.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yb.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://aj.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pm.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://mx.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://nj.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yv.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://dr.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://es.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gn.jianghongdianzi.cn

Go:   encoding/gob
来源：http://eh.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://fx.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vi.bjjhwx.cn

================================================================================
来源：http://ve.muxihuayi.cn

L. 网络请求
来源：http://ds.bookmarksfly.cn

================================================================================
来源：http://es.hahajie.cn

[L01] 发送 GET 请求
来源：http://dq.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dx.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vt.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://ko.huixiangedu.cn

TS:   await fetch(url)
来源：http://zq.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ip.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://pz.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ts.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://je.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://ot.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hw.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ro.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hp.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lz.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://po.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hx.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fq.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xr.szxytkj.cn

[L03] 设置自定义请求头
来源：http://nm.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aw.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wc.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ys.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ue.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fp.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iz.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vv.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tt.9csxet.cn

[L04] 设置超时
来源：http://mn.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://vu.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qw.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lj.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cz.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ze.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zd.lnxyls.cn


<!-- 参考信息 -->