代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://cb.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ve.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nx.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://om.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ld.gzmigu.cn

Go:   defer f.Close()
来源：http://qh.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zt.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cb.bookmarksfly.cn

================================================================================
来源：http://py.bjjhwx.cn

I. 正则表达式
来源：http://as.wgjwhj.cn

================================================================================
来源：http://fi.hahajie.cn

[I01] 判断是否匹配
来源：http://vd.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://te.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://my.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://nh.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://ws.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ot.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aa.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://hj.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oa.wgjwhj.cn

[I02] 提取所有匹配
来源：http://we.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://ox.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qq.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://up.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://uy.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kv.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tn.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://qq.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uz.muxihuayi.cn

[I03] 提取捕获分组
来源：http://nh.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jd.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yl.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fp.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://up.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ny.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ad.nszjky.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yo.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zh.huixiangedu.cn

[I04] 正则替换
来源：http://uj.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ur.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zt.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jh.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zw.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ih.huanxung.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ob.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lx.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sr.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://uj.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dp.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gt.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://pm.lnxyls.cn

TS:   s.split(/\s*,\s*/)
来源：http://xz.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://gz.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qx.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ue.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ke.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ov.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ze.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iv.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iv.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xk.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yp.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wb.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pu.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ws.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://nc.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hx.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gi.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sb.chemitech.net.cn

TS:   /error/gim
来源：http://lx.yuexingan06.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rk.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vl.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://zm.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ls.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://dk.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pp.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ba.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rd.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zw.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kc.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ow.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ee.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xz.gzmigu.cn

================================================================================
来源：http://wk.nicolike.cn

J. 日期与时间
来源：http://bh.jianghongdianzi.cn

================================================================================
来源：http://wl.9csxet.cn

[J01] 获取当前时间
来源：http://xw.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jm.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cq.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://ip.huanxung.cn

TS:   new Date();  Date.now()
来源：http://ya.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zq.nicolike.cn

Go:   time.Now()
来源：http://ie.9csxet.cn

Ruby: Time.now
来源：http://la.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wa.gzmigu.cn

[J02] 格式化输出
来源：http://mp.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://th.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://od.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kq.bookmarksfly.cn

TS:   d.toISOString()
来源：http://mm.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ew.newstarts.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xs.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dp.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gy.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://rp.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hc.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yt.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://ya.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://kt.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fa.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://au.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://tt.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pt.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://ly.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ot.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hx.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dx.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rq.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cl.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mx.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qp.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gy.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://vc.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://xq.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ne.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uz.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fc.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://ec.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tz.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://zp.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bk.shtwfgs.cn

[J06] 计算两时间之差
来源：http://ae.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://hw.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://iq.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ku.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eu.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bq.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://nf.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://vv.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://du.shtwfgs.cn

[J07] 比较两个日期
来源：http://kv.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://ng.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jw.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gg.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fo.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tp.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://en.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jp.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://gw.shxzukj.cn

[J08] 提取年月日与星期
来源：http://il.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dl.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sb.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xl.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ri.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xw.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://om.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mv.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vo.jianghongdianzi.cn

[J09] 时区处理
来源：http://op.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bh.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fv.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jv.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zi.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lw.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vn.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gf.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://du.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://di.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wn.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rp.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xh.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ky.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rn.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mm.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ia.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dj.jianghongdianzi.cn

================================================================================
来源：http://af.huixinmuqiang.cn

K. JSON 与序列化
来源：http://ix.hnjuh.cn

================================================================================
来源：http://ox.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://mq.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qv.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://el.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://vy.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://bn.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sh.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://kr.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sb.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pq.huanxung.cn

[K02] JSON 字符串转对象
来源：http://dz.yuexingan06.cn

Py:   json.loads(s)
来源：http://wq.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tz.9csxet.cn

JS:   JSON.parse(s)
来源：http://nz.szxytkj.cn

TS:   JSON.parse(s)
来源：http://hs.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pb.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://wl.colortex.cn

Ruby: JSON.parse(s)
来源：http://nf.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gp.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://bg.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gs.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qq.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jo.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lx.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wb.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tg.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pw.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ek.9csxet.cn

[K04] 读取 JSON 文件
来源：http://ig.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hx.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://na.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sl.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ju.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mp.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jz.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sb.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cj.huixiangedu.cn

[K05] 深拷贝对象
来源：http://kg.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://xf.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://ru.asd995.cn

JS:   structuredClone(obj)
来源：http://ee.szsharing.cn

TS:   structuredClone(obj)
来源：http://sc.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gt.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rr.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://br.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://to.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://zv.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aw.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yl.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pw.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ot.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vi.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hi.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sw.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fo.panjiajie.cn

[K07] 进制转换
来源：http://gk.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xo.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://da.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zr.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gt.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fb.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yp.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ft.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yq.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://pk.asd995.cn

Py:   pickle.dumps(obj)
来源：http://sz.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bv.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://tc.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://my.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://am.hnjuh.cn

Go:   encoding/gob
来源：http://fk.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://hh.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wc.newstarts.cn

================================================================================
来源：http://hs.shxzukj.cn

L. 网络请求
来源：http://zx.panjiajie.cn

================================================================================
来源：http://pb.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://pq.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tl.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ca.szsharing.cn

JS:   await fetch(url)
来源：http://ge.nicolike.cn

TS:   await fetch(url)
来源：http://bi.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hx.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://cx.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xj.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ty.nicolike.cn

[L02] 发送 POST JSON
来源：http://eh.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ct.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gz.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ed.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mi.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://on.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fl.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oq.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hd.hnjuh.cn

[L03] 设置自定义请求头
来源：http://cs.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://la.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jj.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kj.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nn.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sp.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ok.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mt.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rt.chemitech.net.cn

[L04] 设置超时
来源：http://dp.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://ne.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yk.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rk.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xy.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bf.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://za.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ie.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eq.szsharing.cn

[L05] 上传文件（multipart）
来源：http://ji.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hx.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gw.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ik.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jz.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ew.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wm.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kq.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ug.newstarts.cn

[L06] 解析响应为 JSON
来源：http://vi.asd995.cn


<!-- 参考信息 -->