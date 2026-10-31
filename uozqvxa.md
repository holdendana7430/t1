代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://mi.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dy.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gx.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jx.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uo.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hi.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kd.shxzukj.cn

[H10] 资源自动释放
来源：http://ny.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ye.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rq.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wy.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yi.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dl.shxzukj.cn

Go:   defer f.Close()
来源：http://js.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cu.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nt.lnxyls.cn

================================================================================
来源：http://ps.hnjuh.cn

I. 正则表达式
来源：http://st.jctech888.com.cn

================================================================================
来源：http://qv.521024.cn

[I01] 判断是否匹配
来源：http://cz.lnxyls.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gc.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wj.colortex.cn

JS:   /\d+/.test(s)
来源：http://fc.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://wo.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yj.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eg.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://jb.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mj.hahajie.cn

[I02] 提取所有匹配
来源：http://fm.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://ar.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gw.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ti.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://pl.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dg.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lq.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://sw.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gj.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://yy.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ft.panjiajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zb.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gy.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dd.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uh.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jf.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hf.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sd.shxzukj.cn

[I04] 正则替换
来源：http://wb.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jf.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://il.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://to.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ko.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ny.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pk.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qf.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yv.hahajie.cn

[I05] 按正则拆分
来源：http://al.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ip.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yh.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://dp.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://vf.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://me.bookmarksfly.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nu.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://as.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fd.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bh.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mi.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lp.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mg.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mh.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kq.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zx.jianghongdianzi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rz.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ig.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://qw.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mt.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vi.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ko.bookmarksfly.cn

TS:   /error/gim
来源：http://so.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ny.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nk.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://dd.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sv.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://yu.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gm.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qh.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xq.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cp.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vl.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cu.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xe.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mx.jctech888.com.cn

================================================================================
来源：http://hj.lnxyls.cn

J. 日期与时间
来源：http://ob.muxihuayi.cn

================================================================================
来源：http://hv.shxzukj.cn

[J01] 获取当前时间
来源：http://cl.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ei.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ht.hahajie.cn

JS:   new Date();  Date.now()
来源：http://hw.521024.cn

TS:   new Date();  Date.now()
来源：http://au.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sa.huanxung.cn

Go:   time.Now()
来源：http://ng.szxytkj.cn

Ruby: Time.now
来源：http://ml.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yz.9csxet.cn

[J02] 格式化输出
来源：http://sv.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kw.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yw.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oj.nicolike.cn

TS:   d.toISOString()
来源：http://qy.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pg.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kt.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dr.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bh.lnxyls.cn

[J03] 字符串解析为日期
来源：http://do.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kf.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pi.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://ij.asd995.cn

TS:   new Date("2024-01-02")
来源：http://zz.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vi.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qa.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://hf.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vl.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://vd.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xj.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hl.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uq.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ry.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jj.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bg.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wz.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ot.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://bi.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://on.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qc.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ve.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://im.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://ti.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ot.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://pc.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ch.shxzskj.cn

[J06] 计算两时间之差
来源：http://fa.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://hd.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://li.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hk.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jk.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sf.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://mi.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://id.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://jg.haigaiapp.cn

[J07] 比较两个日期
来源：http://wm.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://hq.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mj.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qu.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xc.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://id.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mv.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cn.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://cv.huixiangedu.cn

[J08] 提取年月日与星期
来源：http://zf.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cq.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iz.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://om.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xr.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hc.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fi.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wv.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://io.yuexingan06.cn

[J09] 时区处理
来源：http://tz.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jp.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sl.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qs.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://so.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yk.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://by.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lu.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ja.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://qq.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rb.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lx.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://te.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xu.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wu.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mi.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ez.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ms.hahajie.cn

================================================================================
来源：http://gc.hahajie.cn

K. JSON 与序列化
来源：http://dd.hahajie.cn

================================================================================
来源：http://sj.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://qe.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ty.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tu.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://to.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://vf.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ul.asd995.cn

Go:   json.Marshal(obj)
来源：http://si.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wn.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ng.nszjky.cn

[K02] JSON 字符串转对象
来源：http://eg.chemitech.net.cn

Py:   json.loads(s)
来源：http://hj.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lg.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://or.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://ij.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://io.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://fu.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://gr.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jy.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://qh.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://os.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ux.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vo.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vd.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bl.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ap.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oj.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xl.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://qt.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uh.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vc.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ow.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oe.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ii.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hf.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uq.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nf.szxytkj.cn

[K05] 深拷贝对象
来源：http://ax.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://rh.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://wj.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://ek.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://hl.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bv.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mg.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wk.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dc.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://bo.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yv.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mj.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oh.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kb.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ye.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wu.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ff.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rp.nszjky.cn

[K07] 进制转换
来源：http://kz.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tn.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nn.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qt.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kr.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zw.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oc.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lm.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pm.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://km.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://rv.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://te.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://jp.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://bk.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cp.yuntaijiaju.cn

Go:   encoding/gob
来源：http://pw.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://qa.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ev.jctech888.com.cn

================================================================================
来源：http://ex.huixinmuqiang.cn

L. 网络请求
来源：http://id.shxzskj.cn

================================================================================
来源：http://yy.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://po.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fz.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wy.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://xp.haigaiapp.cn

TS:   await fetch(url)
来源：http://lp.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ww.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://hc.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ix.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gg.shxzukj.cn

[L02] 发送 POST JSON
来源：http://uf.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yw.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ac.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hm.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://td.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nn.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oc.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yb.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pf.wgjwhj.cn

[L03] 设置自定义请求头
来源：http://xv.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bh.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mv.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dw.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gb.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zr.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ii.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yf.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cr.bjjhwx.cn

[L04] 设置超时
来源：http://tt.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://wd.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://da.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ie.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gh.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bf.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://to.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mm.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cu.colortex.cn

[L05] 上传文件（multipart）
来源：http://hl.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iw.huixinmuqiang.cn


<!-- 参考信息 -->