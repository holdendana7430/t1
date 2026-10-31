代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://ob.chemitech.net.cn

[H08] 获取错误信息与堆栈
来源：http://ax.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://ka.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hs.521024.cn

JS:   e.message;  e.stack
来源：http://xl.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hw.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cy.huanxung.cn

Go:   err.Error()
来源：http://yy.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://oh.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://xb.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://ts.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dq.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ge.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jq.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://du.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kd.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ue.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hq.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qm.huixiangedu.cn

[H10] 资源自动释放
来源：http://kp.huixinmuqiang.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fl.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lt.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wk.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jg.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://en.shxzukj.cn

Go:   defer f.Close()
来源：http://en.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oy.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qh.panjiajie.cn

================================================================================
来源：http://ui.hnjuh.cn

I. 正则表达式
来源：http://aq.newstarts.cn

================================================================================
来源：http://vu.huanxung.cn

[I01] 判断是否匹配
来源：http://hy.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ql.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ao.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://na.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://pg.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aj.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xa.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://oc.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wa.chemitech.net.cn

[I02] 提取所有匹配
来源：http://zo.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://eb.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ni.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jd.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://rg.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mj.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xm.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://xq.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://we.bjjhwx.cn

[I03] 提取捕获分组
来源：http://gi.jianghongdianzi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lj.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hl.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cy.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wi.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://if.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ny.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hf.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bi.huanxung.cn

[I04] 正则替换
来源：http://xm.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zi.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bw.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jh.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fh.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kh.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kn.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dh.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://da.jctech888.com.cn

[I05] 按正则拆分
来源：http://ie.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pe.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bu.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://ef.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://xr.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://qj.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nk.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jn.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ga.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sc.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nk.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ht.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://km.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xp.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pc.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aj.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qg.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qx.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://sg.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ci.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qq.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zh.521024.cn

TS:   /error/gim
来源：http://ms.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yl.hnjuh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pq.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://cr.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dd.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://xd.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ag.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wh.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jp.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qa.huanxung.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ss.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xh.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pq.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hd.bjjhwx.cn

================================================================================
来源：http://rh.szsharing.cn

J. 日期与时间
来源：http://ck.muxihuayi.cn

================================================================================
来源：http://va.szsharing.cn

[J01] 获取当前时间
来源：http://ig.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dm.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sq.asd995.cn

JS:   new Date();  Date.now()
来源：http://ix.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://uq.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rv.hahajie.cn

Go:   time.Now()
来源：http://li.hnjuh.cn

Ruby: Time.now
来源：http://ct.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://or.lnxyls.cn

[J02] 格式化输出
来源：http://va.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ik.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xh.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nz.nicolike.cn

TS:   d.toISOString()
来源：http://ia.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uc.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ar.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lh.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vr.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://kk.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jj.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lg.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://il.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://fe.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hn.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yd.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://zk.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yr.521024.cn

[J04] 时间戳与日期互转
来源：http://cj.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://su.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aj.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tc.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://if.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://va.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jt.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sp.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ps.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://mo.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://sz.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jf.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xd.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oa.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://ro.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qb.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://sk.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://oi.shxzskj.cn

[J06] 计算两时间之差
来源：http://hx.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://ps.521024.cn

PHP:  $end->diff($start)->days;
来源：http://zi.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qk.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wj.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lk.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://ob.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://nb.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://ma.jctech888.com.cn

[J07] 比较两个日期
来源：http://rz.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://jn.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ro.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://um.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pj.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qg.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gq.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://be.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://gn.gzmigu.cn

[J08] 提取年月日与星期
来源：http://st.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fx.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fe.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vo.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vw.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pm.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vz.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://np.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bl.jianghongdianzi.cn

[J09] 时区处理
来源：http://yi.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oj.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zu.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aa.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tx.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zl.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qi.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://br.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uv.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://pp.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ms.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jd.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ln.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mm.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qd.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ox.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nv.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mz.jctech888.com.cn

================================================================================
来源：http://hi.huixinmuqiang.cn

K. JSON 与序列化
来源：http://gt.huixinmuqiang.cn

================================================================================
来源：http://vn.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://qh.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lb.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://le.asd995.cn

JS:   JSON.stringify(obj)
来源：http://yy.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://cm.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vx.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://ug.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bi.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zm.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://xz.wgjwhj.cn

Py:   json.loads(s)
来源：http://ot.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jw.nicolike.cn

JS:   JSON.parse(s)
来源：http://yd.nszjky.cn

TS:   JSON.parse(s)
来源：http://fc.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yp.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://la.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://tr.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xr.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://nr.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://an.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://my.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ta.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ka.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cf.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jl.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mh.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fn.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://gm.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fp.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://no.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kl.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ga.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cw.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kk.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hb.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ye.9csxet.cn

[K05] 深拷贝对象
来源：http://qu.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://os.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://fw.nicolike.cn

JS:   structuredClone(obj)
来源：http://ex.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://qs.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ad.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wv.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zv.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sp.colortex.cn

[K06] 解析 URL 查询串
来源：http://tb.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://og.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jz.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pe.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xw.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ux.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hf.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wf.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gt.asd995.cn

[K07] 进制转换
来源：http://zk.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gw.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hj.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ea.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lu.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kw.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yq.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rb.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xh.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://kf.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://oo.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bc.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://sg.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://fv.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ep.szsharing.cn

Go:   encoding/gob
来源：http://kr.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://cu.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tr.shxzskj.cn

================================================================================
来源：http://vl.521024.cn

L. 网络请求
来源：http://sx.chemitech.net.cn

================================================================================
来源：http://sp.szxytkj.cn

[L01] 发送 GET 请求
来源：http://ar.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://un.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ju.shtwfgs.cn

JS:   await fetch(url)
来源：http://yu.hahajie.cn

TS:   await fetch(url)
来源：http://vq.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pu.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://zy.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ls.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kq.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://jv.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zs.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ka.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rt.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nf.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gc.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fn.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fr.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hc.hnjuh.cn

[L03] 设置自定义请求头
来源：http://kl.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qo.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hp.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kz.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wf.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wf.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mb.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://or.haigaiapp.cn


<!-- 参考信息 -->