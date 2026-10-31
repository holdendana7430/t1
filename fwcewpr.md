代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ty.muxihuayi.cn

Go:   defer f.Close()
来源：http://nc.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ep.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zo.muxihuayi.cn

================================================================================
来源：http://uo.huanxung.cn

I. 正则表达式
来源：http://fv.9csxet.cn

================================================================================
来源：http://dh.shtwfgs.cn

[I01] 判断是否匹配
来源：http://bl.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bt.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gt.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://zq.huanxung.cn

TS:   /\d+/.test(s)
来源：http://cn.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ps.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ai.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://yi.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rt.panjiajie.cn

[I02] 提取所有匹配
来源：http://bv.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://pf.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jm.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jc.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://ib.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ck.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ms.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://au.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gl.panjiajie.cn

[I03] 提取捕获分组
来源：http://po.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ig.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gr.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ik.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://km.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ke.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gy.nszjky.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bi.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yq.yuexingan06.cn

[I04] 正则替换
来源：http://si.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tc.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iy.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ls.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cq.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qm.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wg.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xd.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sv.panjiajie.cn

[I05] 按正则拆分
来源：http://oa.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://do.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ch.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://pa.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://rw.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://ao.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ba.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uo.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vm.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qv.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ip.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nx.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bi.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dj.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ip.yuntaijiaju.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://du.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tj.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://co.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://ow.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kz.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wa.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qx.asd995.cn

TS:   /error/gim
来源：http://ex.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://op.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uh.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://kk.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yw.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://yu.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://az.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ox.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yt.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gj.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vu.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fa.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ni.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gf.hnjuh.cn

================================================================================
来源：http://hp.huanxung.cn

J. 日期与时间
来源：http://gl.szxytkj.cn

================================================================================
来源：http://rk.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://dy.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://an.jctech888.com.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wa.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://zv.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://sv.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lz.yuntaijiaju.cn

Go:   time.Now()
来源：http://td.huanxung.cn

Ruby: Time.now
来源：http://xm.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://be.shxzskj.cn

[J02] 格式化输出
来源：http://sy.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pq.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kj.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wf.colortex.cn

TS:   d.toISOString()
来源：http://fn.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jr.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tj.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qh.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hb.colortex.cn

[J03] 字符串解析为日期
来源：http://xn.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://we.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bm.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://ez.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://ce.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ps.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ff.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://de.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yv.szsharing.cn

[J04] 时间戳与日期互转
来源：http://xs.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://li.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://in.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iq.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ml.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ir.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://li.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ud.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yw.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://ap.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://kq.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pc.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yo.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://td.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://vj.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zr.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://rd.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kx.521024.cn

[J06] 计算两时间之差
来源：http://ci.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://rb.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://or.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xc.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sk.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rr.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://uk.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://oo.521024.cn

C#:   (end - start).TotalSeconds
来源：http://bg.muxihuayi.cn

[J07] 比较两个日期
来源：http://ek.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://wf.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cz.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ca.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gv.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gr.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ft.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mw.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://rq.nszjky.cn

[J08] 提取年月日与星期
来源：http://sq.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qk.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ax.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bo.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aq.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rd.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hj.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fd.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rm.yuntaijiaju.cn

[J09] 时区处理
来源：http://pp.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wz.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ax.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ni.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bt.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ee.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qp.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oy.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://re.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://gm.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mv.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lc.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xw.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hh.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xm.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xe.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mq.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ed.haigaiapp.cn

================================================================================
来源：http://ez.szsharing.cn

K. JSON 与序列化
来源：http://mv.jctech888.com.cn

================================================================================
来源：http://xl.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://lr.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sh.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nv.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://qs.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://pb.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lt.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://ur.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://br.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dr.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://jm.hahajie.cn

Py:   json.loads(s)
来源：http://an.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ub.panjiajie.cn

JS:   JSON.parse(s)
来源：http://np.colortex.cn

TS:   JSON.parse(s)
来源：http://rl.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iv.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://dp.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://eq.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pp.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://dz.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fq.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fx.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://de.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://di.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xi.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pm.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qx.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iq.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://gu.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rr.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hu.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zi.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lm.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://li.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gm.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nb.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sb.bjjhwx.cn

[K05] 深拷贝对象
来源：http://wr.521024.cn

Py:   copy.deepcopy(obj)
来源：http://ui.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://iq.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://qz.szsharing.cn

TS:   structuredClone(obj)
来源：http://sz.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ni.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zt.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zw.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vu.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://qb.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rf.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mw.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iu.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mw.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fc.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vf.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ms.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wa.asd995.cn

[K07] 进制转换
来源：http://or.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gp.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sl.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oa.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wn.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fg.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://es.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ca.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oj.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://iw.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://te.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sa.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://au.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://vr.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sg.bookmarksfly.cn

Go:   encoding/gob
来源：http://pb.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://mc.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nt.haigaiapp.cn

================================================================================
来源：http://wj.jianghongdianzi.cn

L. 网络请求
来源：http://md.521024.cn

================================================================================
来源：http://ga.nszjky.cn

[L01] 发送 GET 请求
来源：http://cv.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tz.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ug.bookmarksfly.cn

JS:   await fetch(url)
来源：http://eb.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://ju.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vi.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://cd.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wr.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ub.521024.cn

[L02] 发送 POST JSON
来源：http://ki.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://iv.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yp.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wc.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://th.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ga.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yl.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pi.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fy.nszjky.cn

[L03] 设置自定义请求头
来源：http://no.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ng.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://on.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ya.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pm.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yi.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pp.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mt.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bi.chemitech.net.cn

[L04] 设置超时
来源：http://or.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://wh.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wp.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://db.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dt.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ia.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://th.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vz.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cx.hahajie.cn

[L05] 上传文件（multipart）
来源：http://cs.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wg.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gy.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ul.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://em.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wn.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vp.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lf.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ag.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://pf.jianghongdianzi.cn

Py:   resp.json()
来源：http://vs.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://iq.asd995.cn

JS:   await resp.json()
来源：http://fc.hnjuh.cn

TS:   await resp.json()
来源：http://wm.asd995.cn


<!-- 参考信息 -->