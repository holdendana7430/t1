代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://cn.huixinmuqiang.cn

[H08] 获取错误信息与堆栈
来源：http://mc.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://jr.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cf.asd995.cn

JS:   e.message;  e.stack
来源：http://xq.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tq.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vk.huixinmuqiang.cn

Go:   err.Error()
来源：http://dl.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://kb.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://iq.shxzukj.cn

[H09] 带错误码的异常
来源：http://rx.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ez.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ve.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cv.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vv.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ya.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dd.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mx.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sx.gzmigu.cn

[H10] 资源自动释放
来源：http://dm.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ov.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iz.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gm.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vd.nicolike.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kc.szsharing.cn

Go:   defer f.Close()
来源：http://wu.gzmigu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tu.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kx.huanxung.cn

================================================================================
来源：http://ff.jctech888.com.cn

I. 正则表达式
来源：http://rx.shtwfgs.cn

================================================================================
来源：http://en.jctech888.com.cn

[I01] 判断是否匹配
来源：http://jf.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yz.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cv.huanxung.cn

JS:   /\d+/.test(s)
来源：http://um.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://xz.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nf.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yi.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://vq.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://id.chemitech.net.cn

[I02] 提取所有匹配
来源：http://fm.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://be.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://st.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yu.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://jn.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://za.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nr.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://ib.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gu.hnjuh.cn

[I03] 提取捕获分组
来源：http://of.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kf.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qz.haigaiapp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yq.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yt.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hi.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yq.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bh.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://og.hnjuh.cn

[I04] 正则替换
来源：http://zl.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ph.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nk.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xy.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mg.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fq.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://au.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://oy.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://on.bookmarksfly.cn

[I05] 按正则拆分
来源：http://nk.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wd.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uy.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://hl.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://pd.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://dq.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oo.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nu.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jk.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eq.hnjuh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vd.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pg.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rs.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zr.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dq.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qj.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zc.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iw.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://oe.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ml.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cd.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://or.szsharing.cn

TS:   /error/gim
来源：http://qq.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://od.colortex.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fo.colortex.cn

Ruby: s.scan(/error/i)
来源：http://hs.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wc.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://df.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ej.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ys.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hd.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rn.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uz.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bb.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oz.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nh.lnxyls.cn

================================================================================
来源：http://xn.huixinmuqiang.cn

J. 日期与时间
来源：http://br.bookmarksfly.cn

================================================================================
来源：http://ft.nicolike.cn

[J01] 获取当前时间
来源：http://rs.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ln.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ia.szsharing.cn

JS:   new Date();  Date.now()
来源：http://jt.huanxung.cn

TS:   new Date();  Date.now()
来源：http://at.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lr.lnxyls.cn

Go:   time.Now()
来源：http://vh.jianghongdianzi.cn

Ruby: Time.now
来源：http://ro.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vd.huanxung.cn

[J02] 格式化输出
来源：http://rw.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ev.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cc.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nt.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://hp.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wg.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zr.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wy.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://df.gzmigu.cn

[J03] 字符串解析为日期
来源：http://tl.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oa.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iw.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://wg.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://sb.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zp.panjiajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oz.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://jo.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vg.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://zz.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oc.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://at.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uo.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pu.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ok.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fp.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mq.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jy.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://so.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://wg.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xy.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ek.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zy.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://jg.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uj.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://ek.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ob.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://ov.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://nn.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://fk.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tl.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kr.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kf.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://ay.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://ee.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://zy.shtwfgs.cn

[J07] 比较两个日期
来源：http://ra.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://td.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bw.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gd.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wm.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ll.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nn.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://as.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://da.shxzskj.cn

[J08] 提取年月日与星期
来源：http://nr.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nr.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://se.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://os.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wp.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wk.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dl.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sx.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://we.gzmigu.cn

[J09] 时区处理
来源：http://uo.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ow.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gl.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ky.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hx.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nz.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ae.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zh.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zc.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://qz.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ww.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lg.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fz.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pn.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fz.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://if.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ft.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://up.huanxung.cn

================================================================================
来源：http://ij.chemitech.net.cn

K. JSON 与序列化
来源：http://qg.yuexingan06.cn

================================================================================
来源：http://ej.521024.cn

[K01] 对象转 JSON 字符串
来源：http://xx.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wu.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fw.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://zx.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://zb.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kv.huanxung.cn

Go:   json.Marshal(obj)
来源：http://ve.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tp.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://op.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://ns.lnxyls.cn

Py:   json.loads(s)
来源：http://bj.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tu.hahajie.cn

JS:   JSON.parse(s)
来源：http://er.panjiajie.cn

TS:   JSON.parse(s)
来源：http://nw.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vz.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://kn.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://xl.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://se.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://gc.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gw.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xd.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cw.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hk.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dz.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uk.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cq.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uo.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://zi.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nd.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xe.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://we.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lv.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zd.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sg.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oq.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dk.muxihuayi.cn

[K05] 深拷贝对象
来源：http://ib.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://ao.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://gv.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://qn.asd995.cn

TS:   structuredClone(obj)
来源：http://yt.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ll.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eh.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://so.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qx.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://iz.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bo.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://si.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qa.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yp.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ud.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sp.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wk.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wl.huixinmuqiang.cn

[K07] 进制转换
来源：http://pj.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ew.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pp.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yp.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jl.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tp.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vz.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ex.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yp.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://jd.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://xx.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zs.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://ii.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://mh.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hn.panjiajie.cn

Go:   encoding/gob
来源：http://zr.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://rc.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://so.huixiangedu.cn

================================================================================
来源：http://rv.yuntaijiaju.cn

L. 网络请求
来源：http://jc.colortex.cn

================================================================================
来源：http://nc.521024.cn

[L01] 发送 GET 请求
来源：http://cx.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ja.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vf.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://zi.gzmigu.cn

TS:   await fetch(url)
来源：http://gp.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cx.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://ip.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sm.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wu.hahajie.cn

[L02] 发送 POST JSON
来源：http://gw.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://js.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://te.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xv.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xg.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://js.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ot.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vo.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sc.szsharing.cn

[L03] 设置自定义请求头
来源：http://bc.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zf.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yb.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xj.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xv.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cg.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pd.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://li.asd995.cn


<!-- 参考信息 -->