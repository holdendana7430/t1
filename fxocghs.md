代发 wailian999

TS:   console.assert(x > 0);
来源：http://rl.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://ne.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ya.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lg.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://to.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://ij.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://nn.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eg.nicolike.cn

JS:   e.message;  e.stack
来源：http://mr.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sj.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uv.9csxet.cn

Go:   err.Error()
来源：http://pi.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://oz.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://dd.9csxet.cn

[H09] 带错误码的异常
来源：http://qj.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xr.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nk.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sk.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qj.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wx.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ml.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nb.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nw.muxihuayi.cn

[H10] 资源自动释放
来源：http://iu.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sr.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ws.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gg.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://un.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ra.521024.cn

Go:   defer f.Close()
来源：http://qy.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wd.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ap.bookmarksfly.cn

================================================================================
来源：http://cf.hahajie.cn

I. 正则表达式
来源：http://iy.huanxung.cn

================================================================================
来源：http://ra.gzmigu.cn

[I01] 判断是否匹配
来源：http://es.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jq.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ej.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://xm.colortex.cn

TS:   /\d+/.test(s)
来源：http://zc.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dw.colortex.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vb.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://vb.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hj.huanxung.cn

[I02] 提取所有匹配
来源：http://ho.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://af.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zm.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://px.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://px.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qk.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nh.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://yq.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hf.wgjwhj.cn

[I03] 提取捕获分组
来源：http://wk.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://op.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jq.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pg.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bs.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://de.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ug.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nb.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yx.521024.cn

[I04] 正则替换
来源：http://rb.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nm.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dj.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ef.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yv.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://px.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qy.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vq.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://st.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://ci.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rf.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jq.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ja.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://kv.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://nq.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oh.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gr.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ho.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://et.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jf.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rq.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ey.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bh.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gq.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://je.haigaiapp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vx.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cn.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://uc.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jl.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kq.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ok.yuexingan06.cn

TS:   /error/gim
来源：http://ma.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rg.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bh.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://ux.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ma.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://yn.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rp.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fe.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yw.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ez.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ty.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ng.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vj.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pf.szsharing.cn

================================================================================
来源：http://zt.nicolike.cn

J. 日期与时间
来源：http://rq.yuexingan06.cn

================================================================================
来源：http://ao.9csxet.cn

[J01] 获取当前时间
来源：http://am.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ie.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uv.hahajie.cn

JS:   new Date();  Date.now()
来源：http://zn.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://uj.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ba.bookmarksfly.cn

Go:   time.Now()
来源：http://ma.muxihuayi.cn

Ruby: Time.now
来源：http://bm.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tp.szsharing.cn

[J02] 格式化输出
来源：http://wa.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ig.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fd.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nm.colortex.cn

TS:   d.toISOString()
来源：http://qs.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tj.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eg.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://id.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rj.panjiajie.cn

[J03] 字符串解析为日期
来源：http://fn.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uo.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ge.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://wf.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://pd.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nv.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://la.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://pa.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wo.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://eg.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mm.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ju.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tg.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://js.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://er.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xu.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aq.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nu.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://rk.521024.cn

Py:   now + timedelta(days=7)
来源：http://qp.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://av.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kx.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zz.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://yn.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kq.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://yq.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://iy.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://zq.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://on.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://co.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://so.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xd.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jt.521024.cn

Go:   end.Sub(start).Hours()
来源：http://yy.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://yw.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://gc.jctech888.com.cn

[J07] 比较两个日期
来源：http://on.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://cm.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ap.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ql.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ya.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mg.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ft.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fc.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://lq.hnjuh.cn

[J08] 提取年月日与星期
来源：http://mz.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wb.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fs.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yu.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dp.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ie.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cg.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ld.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hx.yuntaijiaju.cn

[J09] 时区处理
来源：http://sh.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oi.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xk.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nu.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hc.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xr.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cw.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://is.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ya.521024.cn

[J10] 取今天 / 本月第一天
来源：http://fd.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vc.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sh.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://af.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://be.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mx.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gz.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cf.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aw.shxzukj.cn

================================================================================
来源：http://rh.huanxung.cn

K. JSON 与序列化
来源：http://eb.yuntaijiaju.cn

================================================================================
来源：http://qe.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://hy.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jd.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pj.asd995.cn

JS:   JSON.stringify(obj)
来源：http://xm.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://ma.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tr.9csxet.cn

Go:   json.Marshal(obj)
来源：http://dd.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ve.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vw.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://ct.gzmigu.cn

Py:   json.loads(s)
来源：http://ac.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ak.shxzukj.cn

JS:   JSON.parse(s)
来源：http://tg.521024.cn

TS:   JSON.parse(s)
来源：http://wa.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mw.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://gb.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://lq.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sr.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://fj.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lx.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gd.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ml.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nk.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://so.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ar.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sv.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mi.szsharing.cn

[K04] 读取 JSON 文件
来源：http://nx.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dq.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kt.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fu.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ch.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sx.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sl.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://au.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ul.panjiajie.cn

[K05] 深拷贝对象
来源：http://bo.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://lt.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://ry.hnjuh.cn

JS:   structuredClone(obj)
来源：http://vl.shxzukj.cn

TS:   structuredClone(obj)
来源：http://kv.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ju.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tm.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tw.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wb.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://cy.huixinmuqiang.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ur.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lq.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bd.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ty.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ba.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ym.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zz.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bc.yuexingan06.cn

[K07] 进制转换
来源：http://vy.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ra.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pi.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uh.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uc.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://na.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qo.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dk.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uy.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://mt.bjjhwx.cn

Py:   pickle.dumps(obj)
来源：http://lx.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wv.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://jn.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://bf.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zp.jianghongdianzi.cn

Go:   encoding/gob
来源：http://vn.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://kw.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mz.shxzukj.cn

================================================================================
来源：http://rp.chemitech.net.cn

L. 网络请求
来源：http://fv.gzmigu.cn

================================================================================
来源：http://fa.hahajie.cn

[L01] 发送 GET 请求
来源：http://tx.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ys.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wm.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://fj.nszjky.cn

TS:   await fetch(url)
来源：http://jk.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ke.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://nt.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dz.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zj.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://td.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ce.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pv.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pb.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sl.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mb.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lj.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xf.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xz.szxytkj.cn

[L03] 设置自定义请求头
来源：http://wm.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://us.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ge.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yi.jianghongdianzi.cn


<!-- 参考信息 -->