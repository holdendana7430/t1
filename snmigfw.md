代发 wailian999

TS:   console.assert(x > 0);
来源：http://mp.nicolike.cn

Java: assert x > 0 : "必须为正";
来源：http://xo.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sm.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zn.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://tx.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://mg.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://gm.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cy.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://cf.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pc.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pe.newstarts.cn

Go:   err.Error()
来源：http://cn.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://jd.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://hz.nicolike.cn

[H09] 带错误码的异常
来源：http://bo.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lp.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ch.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qi.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kn.asd995.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hq.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wr.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gg.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rc.newstarts.cn

[H10] 资源自动释放
来源：http://gh.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ph.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sc.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vw.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mz.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wc.szxytkj.cn

Go:   defer f.Close()
来源：http://ng.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ok.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ik.hahajie.cn

================================================================================
来源：http://vr.hahajie.cn

I. 正则表达式
来源：http://pt.szsharing.cn

================================================================================
来源：http://rw.hahajie.cn

[I01] 判断是否匹配
来源：http://wj.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sn.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sb.huanxung.cn

JS:   /\d+/.test(s)
来源：http://wz.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://ef.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://if.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ms.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://lf.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dd.yuexingan06.cn

[I02] 提取所有匹配
来源：http://ms.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://jz.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qt.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ye.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://sz.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zh.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://km.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://sr.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tf.asd995.cn

[I03] 提取捕获分组
来源：http://sj.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ed.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pv.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://az.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ov.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://du.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oe.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uz.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sx.chemitech.net.cn

[I04] 正则替换
来源：http://va.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ok.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ux.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nb.huanxung.cn

TS:   s.replace(/\d+/g, "#")
来源：http://np.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qy.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gz.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fd.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jj.szxytkj.cn

[I05] 按正则拆分
来源：http://ef.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ia.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hx.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://eg.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://ja.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://fj.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hk.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ed.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ul.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sb.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tb.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zs.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zo.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tq.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ut.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wr.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uq.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vk.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://wy.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zv.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kp.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cd.yuntaijiaju.cn

TS:   /error/gim
来源：http://vd.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://no.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xl.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://fw.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oj.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://mw.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hl.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ly.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tq.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ph.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://di.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gz.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pl.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qc.muxihuayi.cn

================================================================================
来源：http://bg.shxzskj.cn

J. 日期与时间
来源：http://es.huixiangedu.cn

================================================================================
来源：http://uw.huixiangedu.cn

[J01] 获取当前时间
来源：http://mu.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gs.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ma.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://lu.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://ic.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ca.haigaiapp.cn

Go:   time.Now()
来源：http://ee.gzmigu.cn

Ruby: Time.now
来源：http://lz.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mb.newstarts.cn

[J02] 格式化输出
来源：http://qx.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eu.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bq.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qo.521024.cn

TS:   d.toISOString()
来源：http://il.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://or.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://in.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yp.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xs.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://sf.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nl.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hh.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://wz.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://tg.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lg.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ft.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://im.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wf.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://hp.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://je.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dm.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ks.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://so.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eg.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pb.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://if.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mh.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://hw.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://bp.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ud.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rn.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ni.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://vo.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://od.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://vl.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jy.colortex.cn

[J06] 计算两时间之差
来源：http://mi.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://ri.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://nm.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mq.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xs.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zz.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://th.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://mv.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://qo.bjjhwx.cn

[J07] 比较两个日期
来源：http://fb.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://gh.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ws.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hp.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rg.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mt.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ie.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nm.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://bt.newstarts.cn

[J08] 提取年月日与星期
来源：http://nf.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ml.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rf.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://an.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fc.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yt.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oq.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ah.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ba.lnxyls.cn

[J09] 时区处理
来源：http://py.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ue.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yu.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mr.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ud.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bp.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wj.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ec.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fo.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://ix.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hq.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hp.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ho.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vh.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kl.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uu.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tb.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ve.shxzskj.cn

================================================================================
来源：http://qd.huanxung.cn

K. JSON 与序列化
来源：http://wz.gzmigu.cn

================================================================================
来源：http://aw.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://wn.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ad.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ka.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://qz.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://yc.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://an.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://wt.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ej.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fl.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://mi.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://mt.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ds.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://go.newstarts.cn

TS:   JSON.parse(s)
来源：http://ar.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://om.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://nq.huanxung.cn

Ruby: JSON.parse(s)
来源：http://up.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://od.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://ts.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oo.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qj.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hn.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vr.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gp.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vq.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fk.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://db.nszjky.cn

[K04] 读取 JSON 文件
来源：http://at.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kp.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zh.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tc.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zy.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xt.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qn.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dp.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mg.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://es.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://sy.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://ap.newstarts.cn

JS:   structuredClone(obj)
来源：http://xg.lnxyls.cn

TS:   structuredClone(obj)
来源：http://tm.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ck.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wq.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ai.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rc.huanxung.cn

[K06] 解析 URL 查询串
来源：http://kp.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yq.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://go.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dt.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wn.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wl.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hg.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oc.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jr.jianghongdianzi.cn

[K07] 进制转换
来源：http://ec.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://om.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dx.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://om.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ht.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cg.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yb.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tj.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rn.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://eh.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://ak.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://da.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://fe.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://sg.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nd.bjjhwx.cn

Go:   encoding/gob
来源：http://ty.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://rz.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pi.bookmarksfly.cn

================================================================================
来源：http://hz.haigaiapp.cn

L. 网络请求
来源：http://ye.shtwfgs.cn

================================================================================
来源：http://de.huanxung.cn

[L01] 发送 GET 请求
来源：http://lr.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bv.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dx.colortex.cn

JS:   await fetch(url)
来源：http://vl.jctech888.com.cn

TS:   await fetch(url)
来源：http://dj.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sg.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://bm.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qi.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://up.shxzskj.cn

[L02] 发送 POST JSON
来源：http://bs.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mt.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xi.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rm.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fl.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lm.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zd.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ag.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qz.bjjhwx.cn

[L03] 设置自定义请求头
来源：http://wl.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://br.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://la.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ce.shxzukj.cn


<!-- 参考信息 -->