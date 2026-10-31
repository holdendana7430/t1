代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://qu.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://ih.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://rl.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cf.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://ck.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sw.yuexingan06.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oz.yuntaijiaju.cn

Go:   err.Error()
来源：http://rl.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://eu.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://rb.521024.cn

[H09] 带错误码的异常
来源：http://zi.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vk.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wk.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fb.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pd.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fq.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://la.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pd.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ms.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://kd.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qv.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zm.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uj.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bo.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tf.panjiajie.cn

Go:   defer f.Close()
来源：http://ff.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ak.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://du.haigaiapp.cn

================================================================================
来源：http://ck.nicolike.cn

I. 正则表达式
来源：http://sf.hahajie.cn

================================================================================
来源：http://xs.hnjuh.cn

[I01] 判断是否匹配
来源：http://io.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oc.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://of.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://dl.nszjky.cn

TS:   /\d+/.test(s)
来源：http://xv.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kn.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jy.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://hv.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rp.lnxyls.cn

[I02] 提取所有匹配
来源：http://zh.shxzukj.cn

Py:   re.findall(r"\d+", s)
来源：http://sc.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sh.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://be.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://rr.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oz.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://os.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://vz.muxihuayi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xz.huixiangedu.cn

[I03] 提取捕获分组
来源：http://um.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://re.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dg.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fs.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ta.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dj.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lp.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://id.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fh.muxihuayi.cn

[I04] 正则替换
来源：http://eu.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hg.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cy.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://op.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sc.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nt.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mb.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ov.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tp.hnjuh.cn

[I05] 按正则拆分
来源：http://ky.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bf.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://op.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://uo.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://vq.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://eq.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mu.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ia.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lc.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vb.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ml.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uj.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yq.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dg.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nq.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gx.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ds.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://vz.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vf.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yu.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ld.hahajie.cn

TS:   /error/gim
来源：http://fx.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vb.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hd.colortex.cn

Ruby: s.scan(/error/i)
来源：http://ob.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sh.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://wl.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://te.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cy.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cp.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dj.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mx.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://im.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fq.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vu.shtwfgs.cn

================================================================================
来源：http://en.huanxung.cn

J. 日期与时间
来源：http://zd.huixinmuqiang.cn

================================================================================
来源：http://bw.shtwfgs.cn

[J01] 获取当前时间
来源：http://av.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mw.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oq.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://kk.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://kp.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ox.huixinmuqiang.cn

Go:   time.Now()
来源：http://qe.huixiangedu.cn

Ruby: Time.now
来源：http://dh.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rl.shtwfgs.cn

[J02] 格式化输出
来源：http://pq.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://se.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bs.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sw.hahajie.cn

TS:   d.toISOString()
来源：http://bi.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lk.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hp.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ja.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hl.9csxet.cn

[J03] 字符串解析为日期
来源：http://ay.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://su.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kk.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://ew.asd995.cn

TS:   new Date("2024-01-02")
来源：http://us.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ie.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ae.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://az.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tr.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://lu.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ye.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pl.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ge.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vi.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://td.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qr.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ss.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://px.521024.cn

[J05] 时间加减（加 7 天）
来源：http://mk.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://ur.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wk.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://do.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wa.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://fe.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xk.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://ul.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ym.huixiangedu.cn

[J06] 计算两时间之差
来源：http://ek.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://bf.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://qa.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://el.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wa.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://if.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://bv.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://ta.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://oa.shxzskj.cn

[J07] 比较两个日期
来源：http://io.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://at.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nw.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ws.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xa.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bi.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://th.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qf.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://lp.nicolike.cn

[J08] 提取年月日与星期
来源：http://ef.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cn.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pu.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yb.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bf.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hl.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://re.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gq.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ey.szsharing.cn

[J09] 时区处理
来源：http://ec.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rb.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cl.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ox.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ux.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jb.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pc.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qt.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ps.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://fs.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tw.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ig.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ag.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zc.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://er.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ef.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ow.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://og.shtwfgs.cn

================================================================================
来源：http://nm.huanxung.cn

K. JSON 与序列化
来源：http://ns.nicolike.cn

================================================================================
来源：http://df.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://cf.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://om.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sz.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://jd.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://nx.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ve.szsharing.cn

Go:   json.Marshal(obj)
来源：http://kk.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://px.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ud.newstarts.cn

[K02] JSON 字符串转对象
来源：http://sa.hahajie.cn

Py:   json.loads(s)
来源：http://vx.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://av.asd995.cn

JS:   JSON.parse(s)
来源：http://cd.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://gs.gzmigu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gq.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://rh.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://ta.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jk.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://hw.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://av.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fz.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jg.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fw.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kq.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rm.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zt.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://we.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://wb.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qg.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yx.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xm.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://it.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dh.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ot.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cr.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hd.lnxyls.cn

[K05] 深拷贝对象
来源：http://ar.521024.cn

Py:   copy.deepcopy(obj)
来源：http://ty.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://ak.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://in.521024.cn

TS:   structuredClone(obj)
来源：http://ub.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ki.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jo.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zp.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hy.huanxung.cn

[K06] 解析 URL 查询串
来源：http://kw.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uv.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ee.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tt.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xi.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vb.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ih.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qn.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://in.yuexingan06.cn

[K07] 进制转换
来源：http://ab.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uh.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ab.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iv.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jl.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ai.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sj.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rj.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://og.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://qt.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://ff.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ix.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://kg.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://lj.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kq.huanxung.cn

Go:   encoding/gob
来源：http://gj.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://yh.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oo.szsharing.cn

================================================================================
来源：http://nd.muxihuayi.cn

L. 网络请求
来源：http://qd.huixiangedu.cn

================================================================================
来源：http://vv.lnxyls.cn

[L01] 发送 GET 请求
来源：http://gx.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ya.yuexingan06.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hy.szsharing.cn

JS:   await fetch(url)
来源：http://ni.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://zf.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ro.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://nm.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dj.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pg.colortex.cn

[L02] 发送 POST JSON
来源：http://eo.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dy.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ee.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bs.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uz.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gq.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pa.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fc.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yj.panjiajie.cn

[L03] 设置自定义请求头
来源：http://mx.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kz.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ct.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rq.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yw.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://la.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ny.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jg.szsharing.cn


<!-- 参考信息 -->