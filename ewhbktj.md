代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gx.shtwfgs.cn

Go:   defer f.Close()
来源：http://hp.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ye.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xt.muxihuayi.cn

================================================================================
来源：http://ae.gzmigu.cn

I. 正则表达式
来源：http://ld.huanxung.cn

================================================================================
来源：http://yt.shtwfgs.cn

[I01] 判断是否匹配
来源：http://ym.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jc.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://iu.newstarts.cn

JS:   /\d+/.test(s)
来源：http://mn.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://ii.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qb.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hy.521024.cn

Ruby: s.match?(/\d+/)
来源：http://pv.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xj.panjiajie.cn

[I02] 提取所有匹配
来源：http://gu.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://nv.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zb.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://id.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://am.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://of.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pr.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://zi.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wi.yuexingan06.cn

[I03] 提取捕获分组
来源：http://ec.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kc.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://au.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uj.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qo.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ff.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fq.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ow.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://um.huixinmuqiang.cn

[I04] 正则替换
来源：http://ws.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lc.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ts.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wg.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wq.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hx.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hb.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://du.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ok.szsharing.cn

[I05] 按正则拆分
来源：http://ko.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://in.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zv.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://jr.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://rs.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://ua.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tp.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qc.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ig.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tr.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://us.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zp.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tz.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nt.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fw.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zk.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ds.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kn.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://kz.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yi.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sz.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xh.newstarts.cn

TS:   /error/gim
来源：http://xf.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zk.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://um.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://lz.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ji.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://ej.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zv.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tt.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nq.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xm.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qk.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bj.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gg.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wz.jianghongdianzi.cn

================================================================================
来源：http://zh.szxytkj.cn

J. 日期与时间
来源：http://yw.wgjwhj.cn

================================================================================
来源：http://sh.yuexingan06.cn

[J01] 获取当前时间
来源：http://ac.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yn.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tz.szsharing.cn

JS:   new Date();  Date.now()
来源：http://xx.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://wb.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pd.haigaiapp.cn

Go:   time.Now()
来源：http://se.szsharing.cn

Ruby: Time.now
来源：http://jz.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tg.colortex.cn

[J02] 格式化输出
来源：http://yt.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ie.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ns.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uj.bjjhwx.cn

TS:   d.toISOString()
来源：http://df.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cf.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xr.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gc.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xi.szxytkj.cn

[J03] 字符串解析为日期
来源：http://cw.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sl.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hp.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://qm.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://vc.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nn.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://og.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://kg.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nh.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://ed.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pf.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://er.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hi.lnxyls.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dx.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nf.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cu.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lu.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gl.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://hi.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://qk.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ck.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://di.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hb.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://hm.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tj.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://um.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rx.szxytkj.cn

[J06] 计算两时间之差
来源：http://ti.521024.cn

Py:   (end - start).total_seconds()
来源：http://eh.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://hs.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ep.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gr.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gb.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://sf.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://wb.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://ri.wgjwhj.cn

[J07] 比较两个日期
来源：http://gu.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://zo.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sh.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mr.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yf.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zm.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://el.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ju.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://kf.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://az.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fg.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yy.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tv.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ac.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ko.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ga.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://on.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bk.yuntaijiaju.cn

[J09] 时区处理
来源：http://wz.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://in.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hx.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dy.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ie.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yf.nicolike.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pr.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qg.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kc.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://ca.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dd.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ap.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jv.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zy.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zn.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zh.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://im.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://et.szxytkj.cn

================================================================================
来源：http://jv.szsharing.cn

K. JSON 与序列化
来源：http://fm.szsharing.cn

================================================================================
来源：http://vi.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://fx.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pt.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qw.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://kg.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://it.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wo.colortex.cn

Go:   json.Marshal(obj)
来源：http://ey.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mt.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bp.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://aa.muxihuayi.cn

Py:   json.loads(s)
来源：http://yb.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tv.nicolike.cn

JS:   JSON.parse(s)
来源：http://yw.huanxung.cn

TS:   JSON.parse(s)
来源：http://vy.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sw.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://qv.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://jr.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qs.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://ra.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uu.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zx.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gr.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vj.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jy.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ug.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yj.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cu.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://wu.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nl.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kw.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://np.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gg.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sv.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ds.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nm.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qa.bjjhwx.cn

[K05] 深拷贝对象
来源：http://fe.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://cm.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://ha.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://wg.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://xq.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hj.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ey.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yy.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tp.szsharing.cn

[K06] 解析 URL 查询串
来源：http://cw.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tm.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ci.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rt.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cg.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pv.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tl.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ki.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nt.asd995.cn

[K07] 进制转换
来源：http://zu.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ur.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pg.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uv.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ky.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yz.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sg.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ns.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://un.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://nm.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://sd.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://us.521024.cn

JS:   v8.serialize(obj)        // Node
来源：http://py.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://ne.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lc.jctech888.com.cn

Go:   encoding/gob
来源：http://ix.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://es.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yr.gzmigu.cn

================================================================================
来源：http://sw.chemitech.net.cn

L. 网络请求
来源：http://av.hnjuh.cn

================================================================================
来源：http://oz.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://oy.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kj.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fm.huanxung.cn

JS:   await fetch(url)
来源：http://nx.hahajie.cn

TS:   await fetch(url)
来源：http://wu.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ko.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://qo.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cq.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bb.colortex.cn

[L02] 发送 POST JSON
来源：http://va.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jt.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fu.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yv.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ym.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wd.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mq.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mu.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mr.gzmigu.cn

[L03] 设置自定义请求头
来源：http://ds.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jq.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jz.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ar.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yn.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nj.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tb.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ub.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rm.bjjhwx.cn

[L04] 设置超时
来源：http://uk.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://wn.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xd.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jq.jianghongdianzi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ic.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ef.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ei.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gc.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uw.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://kb.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://af.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rd.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bz.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vx.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://or.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tz.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cb.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://my.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://eq.nicolike.cn

Py:   resp.json()
来源：http://np.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://lx.lnxyls.cn

JS:   await resp.json()
来源：http://dv.huanxung.cn

TS:   await resp.json()
来源：http://vw.hahajie.cn


<!-- 参考信息 -->