代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://pj.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dl.newstarts.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zb.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ew.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fe.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kk.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ia.bjjhwx.cn

[H10] 资源自动释放
来源：http://sm.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xo.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ah.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uz.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dx.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://us.lnxyls.cn

Go:   defer f.Close()
来源：http://xd.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://id.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bx.szxytkj.cn

================================================================================
来源：http://vd.shxzskj.cn

I. 正则表达式
来源：http://bp.huixiangedu.cn

================================================================================
来源：http://bk.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://lb.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gp.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gz.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://jr.nicolike.cn

TS:   /\d+/.test(s)
来源：http://ae.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ro.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tl.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://qr.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://po.nszjky.cn

[I02] 提取所有匹配
来源：http://zu.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://fb.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zm.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ka.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://gx.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gq.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yb.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://tw.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qd.shxzskj.cn

[I03] 提取捕获分组
来源：http://ep.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lv.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jj.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oh.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kj.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zz.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ab.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hb.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gv.nicolike.cn

[I04] 正则替换
来源：http://fx.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://iz.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yw.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fa.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fp.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sl.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://iz.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://en.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wm.huixiangedu.cn

[I05] 按正则拆分
来源：http://bx.nszjky.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wv.asd995.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ff.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ga.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://on.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://sg.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vb.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ly.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://am.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zu.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rl.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cu.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gp.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jh.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ww.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://td.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://op.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cx.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://lx.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://es.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cr.gzmigu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://me.yuntaijiaju.cn

TS:   /error/gim
来源：http://et.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://je.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eb.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://wl.521024.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ij.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://rd.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ds.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ji.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yb.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oy.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sa.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mm.szxytkj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sx.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kf.huanxung.cn

================================================================================
来源：http://ty.haigaiapp.cn

J. 日期与时间
来源：http://nq.521024.cn

================================================================================
来源：http://dr.szxytkj.cn

[J01] 获取当前时间
来源：http://gq.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vs.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://er.colortex.cn

JS:   new Date();  Date.now()
来源：http://pv.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://nq.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ek.9csxet.cn

Go:   time.Now()
来源：http://ol.bookmarksfly.cn

Ruby: Time.now
来源：http://at.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nj.chemitech.net.cn

[J02] 格式化输出
来源：http://bv.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bh.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cu.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xr.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://qr.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://to.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wo.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uq.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cc.newstarts.cn

[J03] 字符串解析为日期
来源：http://uo.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cj.hnjuh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sq.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://pm.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://zg.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://du.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yd.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://sh.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ef.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://sf.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ic.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bm.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ai.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ux.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fm.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bt.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qn.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ia.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://rx.asd995.cn

Py:   now + timedelta(days=7)
来源：http://qv.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ml.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://po.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://al.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://jc.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ns.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://ws.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sg.lnxyls.cn

[J06] 计算两时间之差
来源：http://hb.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://zx.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://ww.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pi.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://la.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dp.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://vn.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://pj.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://vb.hahajie.cn

[J07] 比较两个日期
来源：http://tg.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://gh.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yr.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cz.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wy.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lq.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fw.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tk.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://sz.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://jl.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jj.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zr.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gu.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yf.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ij.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wv.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://po.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://is.chemitech.net.cn

[J09] 时区处理
来源：http://gw.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yu.nicolike.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fo.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dc.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ep.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hx.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ky.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hw.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zj.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://ki.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mg.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://if.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://go.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tv.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eo.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jg.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hq.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gf.9csxet.cn

================================================================================
来源：http://co.wgjwhj.cn

K. JSON 与序列化
来源：http://ou.9csxet.cn

================================================================================
来源：http://tp.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://id.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hc.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uy.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://lh.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://rl.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yb.nszjky.cn

Go:   json.Marshal(obj)
来源：http://jn.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vm.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ae.colortex.cn

[K02] JSON 字符串转对象
来源：http://io.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://to.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gy.nicolike.cn

JS:   JSON.parse(s)
来源：http://aw.shxzskj.cn

TS:   JSON.parse(s)
来源：http://ki.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cp.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://vj.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://ok.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cg.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://uq.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ld.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ld.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tb.szxytkj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ft.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rp.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ia.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zy.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sx.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://fh.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bx.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ow.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ov.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ar.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dt.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aq.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hg.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fb.jctech888.com.cn

[K05] 深拷贝对象
来源：http://ve.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://th.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://by.szxytkj.cn

JS:   structuredClone(obj)
来源：http://zj.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://kz.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mi.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yn.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uk.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jq.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://gk.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xo.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lu.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ty.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gb.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cj.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fx.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ig.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jt.huanxung.cn

[K07] 进制转换
来源：http://ov.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://is.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bm.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://et.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://to.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ah.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tw.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nu.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gf.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://qm.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://jq.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fq.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://xw.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://fi.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sr.nszjky.cn

Go:   encoding/gob
来源：http://dz.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://tp.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qr.huanxung.cn

================================================================================
来源：http://ug.colortex.cn

L. 网络请求
来源：http://pk.yuntaijiaju.cn

================================================================================
来源：http://ao.nicolike.cn

[L01] 发送 GET 请求
来源：http://lo.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oh.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://br.bookmarksfly.cn

JS:   await fetch(url)
来源：http://kx.shtwfgs.cn

TS:   await fetch(url)
来源：http://dl.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vy.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://lr.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mn.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uo.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://hn.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wb.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hs.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kr.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ng.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mq.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dd.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ln.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ti.hnjuh.cn

[L03] 设置自定义请求头
来源：http://lm.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kh.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rl.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ga.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://br.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nk.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rv.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zv.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fu.shxzukj.cn

[L04] 设置超时
来源：http://tu.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://qp.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ht.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gn.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ab.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tr.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rj.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kp.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://by.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://vr.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ce.muxihuayi.cn


<!-- 参考信息 -->