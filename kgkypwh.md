代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://um.521024.cn

Go:   defer f.Close()
来源：http://nm.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xy.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pl.jianghongdianzi.cn

================================================================================
来源：http://mx.huixiangedu.cn

I. 正则表达式
来源：http://pt.chemitech.net.cn

================================================================================
来源：http://tw.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://ad.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ls.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kz.szsharing.cn

JS:   /\d+/.test(s)
来源：http://ub.newstarts.cn

TS:   /\d+/.test(s)
来源：http://lz.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zi.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://le.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://ci.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sw.shxzskj.cn

[I02] 提取所有匹配
来源：http://ix.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://md.huanxung.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sp.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fs.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://uf.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ad.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ax.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://vi.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xt.gzmigu.cn

[I03] 提取捕获分组
来源：http://di.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dh.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pn.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://br.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kl.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ei.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ts.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pv.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wa.colortex.cn

[I04] 正则替换
来源：http://aw.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uy.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sp.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://to.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cf.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://so.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://na.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://od.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://si.szxytkj.cn

[I05] 按正则拆分
来源：http://cj.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xg.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dh.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://tf.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://di.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://au.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://om.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://iz.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uv.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lk.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tw.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hd.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ed.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vc.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bd.hahajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ik.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vt.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wk.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://qu.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kw.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://us.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dg.newstarts.cn

TS:   /error/gim
来源：http://xk.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gm.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iv.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://iv.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cl.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://zg.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mv.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bn.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tl.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ke.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ms.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://up.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ty.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://op.yuexingan06.cn

================================================================================
来源：http://su.nszjky.cn

J. 日期与时间
来源：http://ob.huixiangedu.cn

================================================================================
来源：http://pf.huixiangedu.cn

[J01] 获取当前时间
来源：http://nd.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dd.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vn.asd995.cn

JS:   new Date();  Date.now()
来源：http://kn.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://ay.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ws.gzmigu.cn

Go:   time.Now()
来源：http://er.panjiajie.cn

Ruby: Time.now
来源：http://ic.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mk.wgjwhj.cn

[J02] 格式化输出
来源：http://nj.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://py.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ud.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://co.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://dn.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mg.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qs.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wz.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ij.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://hd.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lp.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ur.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://ik.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://ey.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lr.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ow.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://th.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qj.521024.cn

[J04] 时间戳与日期互转
来源：http://ov.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ez.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://el.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ru.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ia.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ac.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ho.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tc.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fb.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://mz.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://qe.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xw.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lq.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ij.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://lm.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yz.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://cj.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cb.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://ma.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://nn.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://ho.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eh.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://en.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bd.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://ed.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://bu.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://cx.9csxet.cn

[J07] 比较两个日期
来源：http://ko.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://iv.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nq.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zf.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uh.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ye.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://al.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xu.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://lk.shxzukj.cn

[J08] 提取年月日与星期
来源：http://fi.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fd.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jp.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xt.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tw.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ws.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fl.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ro.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fc.lnxyls.cn

[J09] 时区处理
来源：http://en.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bt.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dr.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ub.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fu.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://so.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dv.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fx.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://no.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://kf.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hv.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iu.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vm.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fc.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ic.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oh.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ix.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uz.shxzukj.cn

================================================================================
来源：http://ce.panjiajie.cn

K. JSON 与序列化
来源：http://iq.chemitech.net.cn

================================================================================
来源：http://tj.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://vh.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dy.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uz.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://mi.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://ma.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hy.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://gf.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gw.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ur.szsharing.cn

[K02] JSON 字符串转对象
来源：http://lf.hnjuh.cn

Py:   json.loads(s)
来源：http://yf.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mm.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://xc.asd995.cn

TS:   JSON.parse(s)
来源：http://pu.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gt.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://ov.colortex.cn

Ruby: JSON.parse(s)
来源：http://xj.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ee.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://wl.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dr.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bk.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hm.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cv.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jv.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vi.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nx.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tb.nszjky.cn

[K04] 读取 JSON 文件
来源：http://bz.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pk.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dv.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iq.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uk.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tr.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cs.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://me.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hw.bjjhwx.cn

[K05] 深拷贝对象
来源：http://sp.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://sf.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://ie.newstarts.cn

JS:   structuredClone(obj)
来源：http://iw.panjiajie.cn

TS:   structuredClone(obj)
来源：http://uo.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zd.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hv.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zn.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vi.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://lr.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mr.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://or.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rx.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qc.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hu.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lu.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://df.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yh.panjiajie.cn

[K07] 进制转换
来源：http://ls.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yd.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ae.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xk.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kq.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ke.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nl.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hr.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sq.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://pb.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://uf.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hh.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://ny.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ps.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lj.nszjky.cn

Go:   encoding/gob
来源：http://ds.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://de.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wf.haigaiapp.cn

================================================================================
来源：http://nz.huanxung.cn

L. 网络请求
来源：http://iq.shxzukj.cn

================================================================================
来源：http://wj.colortex.cn

[L01] 发送 GET 请求
来源：http://yf.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xd.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fo.szsharing.cn

JS:   await fetch(url)
来源：http://lz.shxzukj.cn

TS:   await fetch(url)
来源：http://ae.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ju.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://or.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jr.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eh.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://yu.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cr.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://me.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kq.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yn.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lz.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uy.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fd.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wt.huanxung.cn

[L03] 设置自定义请求头
来源：http://uq.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kg.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gj.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xo.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hw.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pu.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kw.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://te.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dw.nicolike.cn

[L04] 设置超时
来源：http://ui.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://vh.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hq.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ft.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hv.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://an.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yk.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nu.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gv.9csxet.cn

[L05] 上传文件（multipart）
来源：http://cx.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zl.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hj.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://om.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://re.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xx.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yr.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wf.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nh.asd995.cn

[L06] 解析响应为 JSON
来源：http://ei.nszjky.cn

Py:   resp.json()
来源：http://on.asd995.cn

PHP:  json_decode($body, true);
来源：http://gw.lnxyls.cn

JS:   await resp.json()
来源：http://zf.gzmigu.cn

TS:   await resp.json()
来源：http://jd.huixiangedu.cn


<!-- 参考信息 -->