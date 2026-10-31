代发 wailian999

JS:   e.message;  e.stack
来源：http://dr.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bl.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tj.lnxyls.cn

Go:   err.Error()
来源：http://nf.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://jp.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://ns.bjjhwx.cn

[H09] 带错误码的异常
来源：http://uv.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sd.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xg.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cr.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kj.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uz.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cu.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vp.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xf.hahajie.cn

[H10] 资源自动释放
来源：http://rw.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nu.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tf.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ik.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://to.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sf.bookmarksfly.cn

Go:   defer f.Close()
来源：http://bt.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kt.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nc.gzmigu.cn

================================================================================
来源：http://ax.yuntaijiaju.cn

I. 正则表达式
来源：http://se.szxytkj.cn

================================================================================
来源：http://hj.szxytkj.cn

[I01] 判断是否匹配
来源：http://tx.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dd.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://no.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://jo.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://ag.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ox.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bc.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://ol.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ug.lnxyls.cn

[I02] 提取所有匹配
来源：http://ef.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://ie.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://is.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nq.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://na.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pa.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zg.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://ey.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gg.hnjuh.cn

[I03] 提取捕获分组
来源：http://xx.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qe.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dt.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gl.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fi.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ts.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pm.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vh.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zl.asd995.cn

[I04] 正则替换
来源：http://fx.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://aa.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mi.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://px.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ig.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nr.yuntaijiaju.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ml.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hm.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ig.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://oc.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hf.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ww.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://yd.chemitech.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://yg.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://kv.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xg.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hl.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rs.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ki.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ox.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ew.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hs.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wn.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lo.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://my.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vp.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jp.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://ak.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gy.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rc.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kh.haigaiapp.cn

TS:   /error/gim
来源：http://th.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tm.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://er.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://dr.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iw.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://yb.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yc.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://az.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bl.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sq.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gv.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nw.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uw.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ch.colortex.cn

================================================================================
来源：http://jr.panjiajie.cn

J. 日期与时间
来源：http://ye.szxytkj.cn

================================================================================
来源：http://sy.gzmigu.cn

[J01] 获取当前时间
来源：http://tb.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vf.jctech888.com.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yv.szsharing.cn

JS:   new Date();  Date.now()
来源：http://yb.szsharing.cn

TS:   new Date();  Date.now()
来源：http://tm.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ze.huixinmuqiang.cn

Go:   time.Now()
来源：http://xu.nszjky.cn

Ruby: Time.now
来源：http://jz.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sp.jctech888.com.cn

[J02] 格式化输出
来源：http://lp.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zg.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kv.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rk.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://fs.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tn.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vp.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kd.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fs.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://mv.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tp.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qn.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://fe.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://ri.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bi.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ja.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://mo.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ic.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://qm.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zj.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gn.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://el.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cd.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lz.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://av.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jp.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ds.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://vz.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://gh.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ov.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jd.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tv.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://hl.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nl.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://jt.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qv.hahajie.cn

[J06] 计算两时间之差
来源：http://bn.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://su.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://zv.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jq.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aq.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tm.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://ya.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://oa.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://mj.bookmarksfly.cn

[J07] 比较两个日期
来源：http://tu.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://gr.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ou.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ou.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zu.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dg.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vq.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fm.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://xy.panjiajie.cn

[J08] 提取年月日与星期
来源：http://zh.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://po.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gb.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://il.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://im.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tc.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yt.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dq.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://to.huixinmuqiang.cn

[J09] 时区处理
来源：http://bw.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zx.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bj.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pu.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uc.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cv.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dp.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ra.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xm.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://if.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sa.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ne.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fr.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kx.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://at.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ix.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lq.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oe.huixinmuqiang.cn

================================================================================
来源：http://ki.yuexingan06.cn

K. JSON 与序列化
来源：http://nc.colortex.cn

================================================================================
来源：http://yo.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://lb.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jo.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://os.521024.cn

JS:   JSON.stringify(obj)
来源：http://kb.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://ss.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tq.colortex.cn

Go:   json.Marshal(obj)
来源：http://gq.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kb.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rt.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://uw.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://vt.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gx.521024.cn

JS:   JSON.parse(s)
来源：http://io.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://lu.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xd.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://kz.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://hw.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xf.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://ur.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dj.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ai.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ij.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ds.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cs.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tm.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wd.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dt.9csxet.cn

[K04] 读取 JSON 文件
来源：http://no.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qm.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lx.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rd.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qx.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fh.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://by.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sn.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zq.huixiangedu.cn

[K05] 深拷贝对象
来源：http://qg.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://tr.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://mx.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://fu.9csxet.cn

TS:   structuredClone(obj)
来源：http://go.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://aw.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hx.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ug.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rb.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://uy.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tg.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mi.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iy.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pj.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ze.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pi.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://el.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jl.chemitech.net.cn

[K07] 进制转换
来源：http://pq.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ng.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mr.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qg.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://id.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jx.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://et.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ud.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xt.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ll.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://hz.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ki.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://nz.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://rj.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wk.gzmigu.cn

Go:   encoding/gob
来源：http://ut.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://zo.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rb.szsharing.cn

================================================================================
来源：http://ui.asd995.cn

L. 网络请求
来源：http://yg.szxytkj.cn

================================================================================
来源：http://nn.shxzskj.cn

[L01] 发送 GET 请求
来源：http://ht.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yu.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://po.shtwfgs.cn

JS:   await fetch(url)
来源：http://bs.colortex.cn

TS:   await fetch(url)
来源：http://wp.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ay.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://kd.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zd.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bh.nszjky.cn

[L02] 发送 POST JSON
来源：http://mu.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bq.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yl.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zp.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iq.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zh.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://co.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rz.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mo.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://on.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ip.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://up.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ob.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fx.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sn.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hh.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vb.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hn.wgjwhj.cn

[L04] 设置超时
来源：http://dn.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://ky.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://to.jctech888.com.cn


<!-- 参考信息 -->