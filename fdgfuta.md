代发 wailian999

[H07] 断言
来源：http://be.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://wk.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://ep.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://qd.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://mb.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://ag.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tp.nicolike.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zk.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://sv.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://vv.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://nc.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bj.hnjuh.cn

JS:   e.message;  e.stack
来源：http://bv.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rr.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mk.asd995.cn

Go:   err.Error()
来源：http://lk.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://uo.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://qh.newstarts.cn

[H09] 带错误码的异常
来源：http://cr.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lc.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xt.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sa.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jh.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://af.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://av.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uk.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uh.asd995.cn

[H10] 资源自动释放
来源：http://ak.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ah.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://br.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ss.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://li.muxihuayi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://de.muxihuayi.cn

Go:   defer f.Close()
来源：http://bo.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ge.shxzukj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pn.panjiajie.cn

================================================================================
来源：http://mq.nicolike.cn

I. 正则表达式
来源：http://zu.hahajie.cn

================================================================================
来源：http://ro.colortex.cn

[I01] 判断是否匹配
来源：http://gl.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ir.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jn.newstarts.cn

JS:   /\d+/.test(s)
来源：http://kp.521024.cn

TS:   /\d+/.test(s)
来源：http://js.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dr.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://st.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://hd.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uh.asd995.cn

[I02] 提取所有匹配
来源：http://kc.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://yo.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iv.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://li.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://ym.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vu.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wy.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://ma.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bv.panjiajie.cn

[I03] 提取捕获分组
来源：http://vs.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nu.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cj.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gr.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qe.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dv.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pp.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hb.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dw.panjiajie.cn

[I04] 正则替换
来源：http://eu.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yi.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uy.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mf.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vr.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nb.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://io.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bv.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://js.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://rc.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mh.asd995.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://by.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://wg.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://eb.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://bq.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ex.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rk.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rs.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ks.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lc.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ci.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qp.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://am.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://of.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kp.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yp.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wn.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://tj.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vm.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ni.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://in.szsharing.cn

TS:   /error/gim
来源：http://ci.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zw.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://er.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://qn.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://da.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://qo.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uy.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jk.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ky.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cs.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://al.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vf.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ys.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ml.asd995.cn

================================================================================
来源：http://ug.9csxet.cn

J. 日期与时间
来源：http://qq.nszjky.cn

================================================================================
来源：http://cd.asd995.cn

[J01] 获取当前时间
来源：http://yr.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yn.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://el.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://zf.nicolike.cn

TS:   new Date();  Date.now()
来源：http://ea.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cr.panjiajie.cn

Go:   time.Now()
来源：http://pn.9csxet.cn

Ruby: Time.now
来源：http://hg.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wo.bjjhwx.cn

[J02] 格式化输出
来源：http://mp.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aw.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vs.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mh.huixiangedu.cn

TS:   d.toISOString()
来源：http://ep.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sz.newstarts.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kd.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ns.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uf.nszjky.cn

[J03] 字符串解析为日期
来源：http://cq.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rr.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ag.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://kh.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://ts.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qe.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kf.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://ud.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cv.nszjky.cn

[J04] 时间戳与日期互转
来源：http://dj.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://up.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://je.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ag.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mg.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eo.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tp.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gh.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bg.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://km.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://he.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wz.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oh.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://up.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://zk.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wm.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://nh.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qj.yuexingan06.cn

[J06] 计算两时间之差
来源：http://cv.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://il.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://wo.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qy.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pe.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wy.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://qv.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://wp.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://am.gzmigu.cn

[J07] 比较两个日期
来源：http://xa.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://rs.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dd.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://om.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://er.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cx.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gz.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qc.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://rb.nszjky.cn

[J08] 提取年月日与星期
来源：http://ap.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mk.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oi.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://is.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://my.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://og.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fy.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uv.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://on.521024.cn

[J09] 时区处理
来源：http://ha.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xw.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://me.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sp.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pc.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vv.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ph.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jp.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ea.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://wo.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kk.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qd.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hk.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://er.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tg.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zs.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oc.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bi.colortex.cn

================================================================================
来源：http://xi.jianghongdianzi.cn

K. JSON 与序列化
来源：http://mx.asd995.cn

================================================================================
来源：http://zb.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://wb.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pg.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uz.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://yl.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://ym.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fg.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://zk.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bf.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wg.huanxung.cn

[K02] JSON 字符串转对象
来源：http://gk.gzmigu.cn

Py:   json.loads(s)
来源：http://rp.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vg.asd995.cn

JS:   JSON.parse(s)
来源：http://sa.colortex.cn

TS:   JSON.parse(s)
来源：http://mm.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nf.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://vm.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://tk.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nc.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://nb.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ts.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fe.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wr.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tf.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tr.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ed.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cw.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ym.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://ny.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qz.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sg.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sn.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uq.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pw.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ag.shtwfgs.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qe.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yb.chemitech.net.cn

[K05] 深拷贝对象
来源：http://zu.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://bx.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://nk.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://yz.shxzukj.cn

TS:   structuredClone(obj)
来源：http://yl.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vc.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://co.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ug.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ed.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://jm.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vr.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xf.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bs.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fa.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://he.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ee.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uj.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qz.colortex.cn

[K07] 进制转换
来源：http://ft.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rv.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ph.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pv.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ns.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xz.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sj.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ea.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gv.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://ii.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://oz.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mt.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://fq.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://rl.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uf.bookmarksfly.cn

Go:   encoding/gob
来源：http://mi.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://xo.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ra.bjjhwx.cn

================================================================================
来源：http://im.bookmarksfly.cn

L. 网络请求
来源：http://sk.gzmigu.cn

================================================================================
来源：http://ww.szxytkj.cn

[L01] 发送 GET 请求
来源：http://rs.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ab.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jg.bookmarksfly.cn

JS:   await fetch(url)
来源：http://gq.bjjhwx.cn

TS:   await fetch(url)
来源：http://ef.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lq.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://je.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fq.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ld.gzmigu.cn

[L02] 发送 POST JSON
来源：http://zs.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vv.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://do.wgjwhj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bj.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vy.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kn.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jv.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oq.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://id.wgjwhj.cn


<!-- 参考信息 -->