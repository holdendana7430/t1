代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://ta.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ng.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pm.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xz.muxihuayi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ae.bjjhwx.cn

Go:   defer f.Close()
来源：http://ds.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sl.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bu.asd995.cn

================================================================================
来源：http://sa.bookmarksfly.cn

I. 正则表达式
来源：http://xd.nicolike.cn

================================================================================
来源：http://ni.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://ub.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oz.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zz.colortex.cn

JS:   /\d+/.test(s)
来源：http://dd.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://qh.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ak.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://va.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://qo.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://so.hahajie.cn

[I02] 提取所有匹配
来源：http://wh.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://wn.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yd.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://im.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://uq.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yl.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://du.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://mm.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fw.lnxyls.cn

[I03] 提取捕获分组
来源：http://dn.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dq.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ip.haigaiapp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ek.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nd.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uy.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ya.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vw.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rj.panjiajie.cn

[I04] 正则替换
来源：http://gd.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hy.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tf.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rg.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://li.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tl.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qt.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://np.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dm.shxzskj.cn

[I05] 按正则拆分
来源：http://pi.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yj.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lx.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://nb.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://em.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://sl.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kn.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xe.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ra.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jn.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bl.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ji.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zc.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ld.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kv.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ru.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fd.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zr.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://rj.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sg.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vi.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dw.bjjhwx.cn

TS:   /error/gim
来源：http://jk.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://is.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wy.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://qx.521024.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tb.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://cq.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xr.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ai.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fy.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://on.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gs.muxihuayi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://su.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jj.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hy.haigaiapp.cn

================================================================================
来源：http://rx.hahajie.cn

J. 日期与时间
来源：http://ht.panjiajie.cn

================================================================================
来源：http://rj.9csxet.cn

[J01] 获取当前时间
来源：http://uv.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xa.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tj.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://hd.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://gd.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pm.9csxet.cn

Go:   time.Now()
来源：http://yr.chemitech.net.cn

Ruby: Time.now
来源：http://pk.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ph.szsharing.cn

[J02] 格式化输出
来源：http://pw.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ct.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://st.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fv.yuexingan06.cn

TS:   d.toISOString()
来源：http://vb.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wq.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nn.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ug.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gx.hahajie.cn

[J03] 字符串解析为日期
来源：http://wa.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fc.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zv.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://bk.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://yp.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://eu.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://he.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://lm.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mf.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://rt.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yw.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lg.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tu.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ec.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ak.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wm.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vy.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wr.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://us.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://nh.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wd.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pa.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://th.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://sp.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://je.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://wa.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://le.asd995.cn

[J06] 计算两时间之差
来源：http://qe.colortex.cn

Py:   (end - start).total_seconds()
来源：http://gv.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://ki.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ky.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yx.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iy.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://mm.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://jm.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://rc.shxzskj.cn

[J07] 比较两个日期
来源：http://ev.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://hc.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kn.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cf.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rr.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ku.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eb.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wd.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://ch.shxzskj.cn

[J08] 提取年月日与星期
来源：http://hu.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gr.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://il.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://og.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qi.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cu.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://un.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tu.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://js.hahajie.cn

[J09] 时区处理
来源：http://bb.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sv.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yo.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ws.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mz.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sb.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gf.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zx.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://he.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://rw.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hr.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nh.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fy.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ex.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bj.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qy.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ig.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fz.shxzskj.cn

================================================================================
来源：http://oh.bookmarksfly.cn

K. JSON 与序列化
来源：http://oy.hahajie.cn

================================================================================
来源：http://eg.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://sy.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ec.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ss.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://ys.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://ni.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kp.521024.cn

Go:   json.Marshal(obj)
来源：http://xm.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rr.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xb.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://oj.nszjky.cn

Py:   json.loads(s)
来源：http://qp.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zv.shxzukj.cn

JS:   JSON.parse(s)
来源：http://dp.panjiajie.cn

TS:   JSON.parse(s)
来源：http://hy.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ff.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://zk.nszjky.cn

Ruby: JSON.parse(s)
来源：http://ib.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ui.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://zj.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ai.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nw.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tv.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rb.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xn.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ii.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nh.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uo.colortex.cn

[K04] 读取 JSON 文件
来源：http://hz.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yd.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ib.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vi.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gg.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ol.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kd.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vu.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zc.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://ka.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://mq.lnxyls.cn

PHP:  unserialize(serialize($obj));
来源：http://fj.panjiajie.cn

JS:   structuredClone(obj)
来源：http://wk.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://vv.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pt.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qg.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ag.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ge.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://lf.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ji.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nq.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zq.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zx.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fc.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rt.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nj.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://im.bookmarksfly.cn

[K07] 进制转换
来源：http://ej.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lu.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sf.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pp.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yz.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jz.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://md.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fo.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zd.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://ob.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://zo.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ur.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://er.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://cy.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lj.haigaiapp.cn

Go:   encoding/gob
来源：http://az.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://pu.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://st.colortex.cn

================================================================================
来源：http://dr.panjiajie.cn

L. 网络请求
来源：http://jn.nicolike.cn

================================================================================
来源：http://cv.shxzukj.cn

[L01] 发送 GET 请求
来源：http://al.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://za.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://da.521024.cn

JS:   await fetch(url)
来源：http://nv.9csxet.cn

TS:   await fetch(url)
来源：http://gb.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://og.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://qa.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://da.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ds.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://tt.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fb.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://or.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gj.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xs.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yw.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wy.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ov.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gzmigu.cn

[L03] 设置自定义请求头
来源：http://ij.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://td.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uq.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yk.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mx.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kq.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ku.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xo.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mr.gzmigu.cn

[L04] 设置超时
来源：http://ku.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://ru.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ac.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://em.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ok.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://td.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zd.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ms.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rp.szsharing.cn

[L05] 上传文件（multipart）
来源：http://lz.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://us.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wo.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://th.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jh.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iv.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aa.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ch.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qn.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://sf.yuexingan06.cn


<!-- 参考信息 -->