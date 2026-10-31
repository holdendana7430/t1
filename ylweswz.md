代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://yz.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://bm.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://ae.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vc.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://zf.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vy.huixinmuqiang.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kl.shxzskj.cn

Go:   err.Error()
来源：http://tb.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://yk.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://hm.jctech888.com.cn

[H09] 带错误码的异常
来源：http://fb.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://re.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ny.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rt.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lz.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ew.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kz.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ap.lnxyls.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kk.jctech888.com.cn

[H10] 资源自动释放
来源：http://ew.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yw.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ec.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ef.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wx.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ka.shxzukj.cn

Go:   defer f.Close()
来源：http://rp.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://km.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vo.bjjhwx.cn

================================================================================
来源：http://dq.hnjuh.cn

I. 正则表达式
来源：http://hk.colortex.cn

================================================================================
来源：http://hn.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://nz.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rg.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oc.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://ze.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://ip.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hg.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hl.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://zc.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fk.nszjky.cn

[I02] 提取所有匹配
来源：http://iy.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://aj.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sz.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sq.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://wm.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oo.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vt.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://vx.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tl.nszjky.cn

[I03] 提取捕获分组
来源：http://hp.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tk.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://if.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wo.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ae.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://es.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yd.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xi.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://za.wgjwhj.cn

[I04] 正则替换
来源：http://up.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mg.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pp.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://al.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hd.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ws.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vw.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rj.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ed.bookmarksfly.cn

[I05] 按正则拆分
来源：http://ab.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wu.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nx.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://cp.chemitech.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://uv.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://rw.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gs.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ky.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kz.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zx.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rc.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rx.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://se.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xp.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://es.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zh.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xq.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tl.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://xd.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aw.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://el.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qw.bookmarksfly.cn

TS:   /error/gim
来源：http://fn.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wg.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vg.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://in.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fn.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://xr.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cm.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zw.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mp.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wo.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tl.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sx.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qu.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uw.nicolike.cn

================================================================================
来源：http://cu.hahajie.cn

J. 日期与时间
来源：http://qy.521024.cn

================================================================================
来源：http://mq.panjiajie.cn

[J01] 获取当前时间
来源：http://ir.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ys.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fo.colortex.cn

JS:   new Date();  Date.now()
来源：http://yc.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://zi.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ug.huixinmuqiang.cn

Go:   time.Now()
来源：http://wf.gzmigu.cn

Ruby: Time.now
来源：http://lq.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yq.521024.cn

[J02] 格式化输出
来源：http://fl.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ns.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://au.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kw.521024.cn

TS:   d.toISOString()
来源：http://um.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ng.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mc.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dj.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lw.nszjky.cn

[J03] 字符串解析为日期
来源：http://ej.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ya.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://en.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://lv.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://mp.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://si.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cp.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://bu.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://al.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://xz.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nz.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ey.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://se.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tj.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pf.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rs.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xc.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pe.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://vx.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://ft.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sg.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jq.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zg.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://hz.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yq.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://pn.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ch.shtwfgs.cn

[J06] 计算两时间之差
来源：http://jw.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://lc.521024.cn

PHP:  $end->diff($start)->days;
来源：http://kv.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jo.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ky.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ct.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://bl.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://re.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://oh.chemitech.net.cn

[J07] 比较两个日期
来源：http://od.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://qr.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zc.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://am.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nl.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ol.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vw.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://je.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://md.szsharing.cn

[J08] 提取年月日与星期
来源：http://ql.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ky.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://na.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pl.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ah.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wh.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bj.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zt.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gg.nszjky.cn

[J09] 时区处理
来源：http://uj.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fw.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bp.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://or.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dt.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eh.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nj.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xd.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xw.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://lu.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hm.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cw.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ox.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lw.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://un.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cr.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lm.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://it.shtwfgs.cn

================================================================================
来源：http://wn.szsharing.cn

K. JSON 与序列化
来源：http://zx.asd995.cn

================================================================================
来源：http://iy.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://ap.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fh.huixiangedu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wd.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://gk.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://zb.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bh.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://ae.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sh.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fl.9csxet.cn

[K02] JSON 字符串转对象
来源：http://xw.9csxet.cn

Py:   json.loads(s)
来源：http://ul.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://az.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://hk.hnjuh.cn

TS:   JSON.parse(s)
来源：http://jh.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kv.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://pl.asd995.cn

Ruby: JSON.parse(s)
来源：http://rl.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pn.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://sx.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://py.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vy.jianghongdianzi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://eq.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://er.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sw.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qt.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vc.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qf.asd995.cn

[K04] 读取 JSON 文件
来源：http://ak.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ze.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hf.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rc.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wh.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pb.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xm.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dr.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hf.hnjuh.cn

[K05] 深拷贝对象
来源：http://zu.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://rb.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://ni.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://cd.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://wz.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mh.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iv.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wt.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pv.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://pg.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jb.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ws.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cq.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pm.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://de.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tm.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rz.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zf.colortex.cn

[K07] 进制转换
来源：http://td.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qn.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fx.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xu.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tx.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ll.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bs.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rq.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jx.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://zp.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://ye.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://sn.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://sb.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://is.haigaiapp.cn

Go:   encoding/gob
来源：http://bx.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://nn.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ni.panjiajie.cn

================================================================================
来源：http://no.colortex.cn

L. 网络请求
来源：http://uu.nicolike.cn

================================================================================
来源：http://qz.521024.cn

[L01] 发送 GET 请求
来源：http://ws.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rg.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zp.yuexingan06.cn

JS:   await fetch(url)
来源：http://xc.shxzskj.cn

TS:   await fetch(url)
来源：http://xw.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uv.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://zj.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mc.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://od.newstarts.cn

[L02] 发送 POST JSON
来源：http://mv.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://se.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gr.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gi.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sg.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sm.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wb.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pm.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nu.wgjwhj.cn

[L03] 设置自定义请求头
来源：http://hf.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mb.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://la.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yr.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wz.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cz.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ae.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iv.huixinmuqiang.cn


<!-- 参考信息 -->