代发 wailian999

================================================================================
来源：http://vv.huixiangedu.cn

I. 正则表达式
来源：http://fc.wgjwhj.cn

================================================================================
来源：http://ph.bjjhwx.cn

[I01] 判断是否匹配
来源：http://hh.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://os.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oq.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://ea.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://dp.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iw.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gu.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://wi.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kh.hahajie.cn

[I02] 提取所有匹配
来源：http://mn.szsharing.cn

Py:   re.findall(r"\d+", s)
来源：http://lp.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ei.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ui.521024.cn

TS:   s.match(/\d+/g)
来源：http://mm.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ad.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dv.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://yb.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gg.wgjwhj.cn

[I03] 提取捕获分组
来源：http://uy.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sc.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vv.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gh.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mh.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vv.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cr.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://re.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://to.colortex.cn

[I04] 正则替换
来源：http://wc.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dp.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nz.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dz.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qd.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ue.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gk.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ei.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://it.huanxung.cn

[I05] 按正则拆分
来源：http://dl.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kq.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sj.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://al.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://cq.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://td.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kt.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sn.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cu.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tv.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://md.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sz.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xh.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uy.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uv.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rv.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fx.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uy.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://wk.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lv.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tk.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ej.huixinmuqiang.cn

TS:   /error/gim
来源：http://sq.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yu.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jn.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://lu.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://id.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://xg.521024.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dv.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xc.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rn.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gm.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wy.muxihuayi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cs.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hu.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uq.jctech888.com.cn

================================================================================
来源：http://ej.jctech888.com.cn

J. 日期与时间
来源：http://jl.haigaiapp.cn

================================================================================
来源：http://wl.szsharing.cn

[J01] 获取当前时间
来源：http://gf.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yh.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ci.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://ur.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://vj.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://na.wgjwhj.cn

Go:   time.Now()
来源：http://mq.521024.cn

Ruby: Time.now
来源：http://gy.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ed.jianghongdianzi.cn

[J02] 格式化输出
来源：http://cb.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vb.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jv.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://di.newstarts.cn

TS:   d.toISOString()
来源：http://ik.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://al.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://py.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xh.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sv.newstarts.cn

[J03] 字符串解析为日期
来源：http://ol.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sf.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://by.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://jb.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://ap.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://km.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yf.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://md.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cr.521024.cn

[J04] 时间戳与日期互转
来源：http://vw.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iw.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fw.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yc.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://by.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bj.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sv.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jx.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yf.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://nv.colortex.cn

Py:   now + timedelta(days=7)
来源：http://sh.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ei.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fq.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://au.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://ml.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ko.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://gd.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mz.haigaiapp.cn

[J06] 计算两时间之差
来源：http://hn.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://qr.521024.cn

PHP:  $end->diff($start)->days;
来源：http://ym.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rv.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yr.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uh.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://fg.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://bh.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://ap.panjiajie.cn

[J07] 比较两个日期
来源：http://jd.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://lv.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xg.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vi.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iu.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pj.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://im.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rx.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ay.gzmigu.cn

[J08] 提取年月日与星期
来源：http://rp.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://il.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ti.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fp.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mw.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rz.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hk.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yg.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jf.muxihuayi.cn

[J09] 时区处理
来源：http://dq.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pr.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hp.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dp.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cv.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hm.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://og.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fl.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lg.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://px.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dl.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ow.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fm.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dg.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bx.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cs.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ui.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gr.jianghongdianzi.cn

================================================================================
来源：http://wo.shxzukj.cn

K. JSON 与序列化
来源：http://ws.bookmarksfly.cn

================================================================================
来源：http://ue.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://bj.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://us.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kq.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://sc.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://fy.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qn.szsharing.cn

Go:   json.Marshal(obj)
来源：http://vf.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yz.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xk.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://il.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://tl.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bm.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://ww.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://xu.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ps.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://lp.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://sx.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ed.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://bs.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uj.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ee.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qc.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ck.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tv.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bt.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fd.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rr.huanxung.cn

[K04] 读取 JSON 文件
来源：http://jg.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cu.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ji.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nh.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oh.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uk.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ao.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ct.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oj.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://ti.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://wu.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://ai.huanxung.cn

JS:   structuredClone(obj)
来源：http://fi.9csxet.cn

TS:   structuredClone(obj)
来源：http://ri.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zp.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ed.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ue.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nu.huanxung.cn

[K06] 解析 URL 查询串
来源：http://vl.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qd.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xh.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qi.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nz.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zx.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ri.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qt.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zn.nszjky.cn

[K07] 进制转换
来源：http://tj.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mt.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://au.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://je.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pb.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nv.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zw.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nq.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ea.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ym.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://yx.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hl.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://bf.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://fy.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ba.huixiangedu.cn

Go:   encoding/gob
来源：http://co.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://zk.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://it.newstarts.cn

================================================================================
来源：http://ze.newstarts.cn

L. 网络请求
来源：http://su.lnxyls.cn

================================================================================
来源：http://ko.colortex.cn

[L01] 发送 GET 请求
来源：http://ns.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gi.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hj.wgjwhj.cn

JS:   await fetch(url)
来源：http://hx.shxzskj.cn

TS:   await fetch(url)
来源：http://fd.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fe.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://im.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sj.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fx.shxzukj.cn

[L02] 发送 POST JSON
来源：http://mz.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lr.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ij.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ng.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vi.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://et.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wm.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fl.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rr.szxytkj.cn

[L03] 设置自定义请求头
来源：http://ky.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hy.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mw.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lw.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dl.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://as.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cy.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bc.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ek.szxytkj.cn

[L04] 设置超时
来源：http://ca.shxzukj.cn

Py:   requests.get(url, timeout=5)
来源：http://dl.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://al.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bp.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://py.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wl.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hg.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pb.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yx.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://zx.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aq.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oy.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rv.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bi.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sh.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tm.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yp.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zv.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://rs.nicolike.cn

Py:   resp.json()
来源：http://id.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://we.jianghongdianzi.cn

JS:   await resp.json()
来源：http://ak.szsharing.cn

TS:   await resp.json()
来源：http://gt.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pv.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://is.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://je.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mk.nicolike.cn


<!-- 参考信息 -->