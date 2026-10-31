代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ts.huixiangedu.cn

Go:   defer f.Close()
来源：http://ge.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pw.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nf.colortex.cn

================================================================================
来源：http://nb.asd995.cn

I. 正则表达式
来源：http://mq.chemitech.net.cn

================================================================================
来源：http://kb.panjiajie.cn

[I01] 判断是否匹配
来源：http://rc.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kn.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kk.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://oa.newstarts.cn

TS:   /\d+/.test(s)
来源：http://dk.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pb.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gy.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://dk.9csxet.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sq.521024.cn

[I02] 提取所有匹配
来源：http://ze.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://ee.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rs.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vs.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://xi.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ts.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cg.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://or.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://me.colortex.cn

[I03] 提取捕获分组
来源：http://ps.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lz.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sj.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zj.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vp.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wp.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ut.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mr.muxihuayi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mj.hahajie.cn

[I04] 正则替换
来源：http://zd.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bf.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rq.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fb.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xi.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sw.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zi.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gv.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vk.shxzukj.cn

[I05] 按正则拆分
来源：http://gl.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fn.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ux.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://fh.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://eb.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://uw.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vt.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ub.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xh.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://of.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xu.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uz.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sc.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ip.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qq.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vp.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kp.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ar.521024.cn

[I07] 忽略大小写与多行模式
来源：http://vg.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fr.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qc.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://db.9csxet.cn

TS:   /error/gim
来源：http://gi.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://al.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sa.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://hl.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vi.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://jn.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bc.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://no.shxzukj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dk.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zg.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qv.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lf.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sj.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wk.nicolike.cn

================================================================================
来源：http://xk.shtwfgs.cn

J. 日期与时间
来源：http://ce.haigaiapp.cn

================================================================================
来源：http://yf.haigaiapp.cn

[J01] 获取当前时间
来源：http://zy.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mk.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ct.521024.cn

JS:   new Date();  Date.now()
来源：http://ry.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://ud.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vt.bookmarksfly.cn

Go:   time.Now()
来源：http://ts.haigaiapp.cn

Ruby: Time.now
来源：http://mu.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://up.shxzukj.cn

[J02] 格式化输出
来源：http://ua.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qr.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zx.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aw.szxytkj.cn

TS:   d.toISOString()
来源：http://va.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://km.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fe.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wr.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rg.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://fm.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rd.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yv.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://lp.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://hh.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rb.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vo.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ks.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nx.521024.cn

[J04] 时间戳与日期互转
来源：http://wj.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ht.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hy.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tz.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://em.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iq.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yo.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ha.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pm.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://zl.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://ws.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uz.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hd.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ul.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://mk.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://un.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://ui.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hc.wgjwhj.cn

[J06] 计算两时间之差
来源：http://nb.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://ig.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://vo.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ku.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xq.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://at.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://xp.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://xj.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://bx.nicolike.cn

[J07] 比较两个日期
来源：http://kj.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://pe.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pi.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yy.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ei.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lh.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fp.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://td.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://us.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://gy.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yb.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zf.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rv.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fe.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fy.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ve.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vm.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jl.szsharing.cn

[J09] 时区处理
来源：http://go.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ix.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nf.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vr.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qf.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ns.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jm.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fg.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ho.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://uf.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zj.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://db.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cs.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ie.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dh.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vn.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hl.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kk.shxzukj.cn

================================================================================
来源：http://mk.gzmigu.cn

K. JSON 与序列化
来源：http://mh.bjjhwx.cn

================================================================================
来源：http://lw.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://ra.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aq.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eu.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://wq.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://cw.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zy.szsharing.cn

Go:   json.Marshal(obj)
来源：http://wp.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mu.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fe.nszjky.cn

[K02] JSON 字符串转对象
来源：http://cl.chemitech.net.cn

Py:   json.loads(s)
来源：http://io.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vs.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://ak.521024.cn

TS:   JSON.parse(s)
来源：http://wq.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ao.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://bd.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://ls.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yp.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://iw.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gq.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bs.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://eo.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dx.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gz.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fm.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zi.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aa.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://ts.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bw.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bb.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qz.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nz.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qo.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bs.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lu.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://di.nszjky.cn

[K05] 深拷贝对象
来源：http://im.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://kt.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://dc.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://jg.hahajie.cn

TS:   structuredClone(obj)
来源：http://ao.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cm.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ko.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bw.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ha.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://ps.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ex.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ew.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bu.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://as.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bm.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ao.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hm.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dp.yuntaijiaju.cn

[K07] 进制转换
来源：http://gf.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lj.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://et.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jj.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jd.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://du.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mw.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ib.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qj.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://ir.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://jn.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ex.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://on.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://ie.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zs.bjjhwx.cn

Go:   encoding/gob
来源：http://wg.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://ib.9csxet.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yc.nszjky.cn

================================================================================
来源：http://yp.521024.cn

L. 网络请求
来源：http://kb.huixinmuqiang.cn

================================================================================
来源：http://mr.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://sj.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ml.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vc.shtwfgs.cn

JS:   await fetch(url)
来源：http://sc.521024.cn

TS:   await fetch(url)
来源：http://qr.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yk.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://oy.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vx.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hw.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://ys.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vf.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ov.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sm.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gn.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sl.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wh.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tp.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kk.lnxyls.cn

[L03] 设置自定义请求头
来源：http://nt.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://co.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zu.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bk.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cn.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zg.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rm.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ak.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jt.chemitech.net.cn

[L04] 设置超时
来源：http://bb.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://jy.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xh.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vc.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ny.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ha.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qh.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://je.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pe.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://vm.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uj.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bg.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pi.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qr.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yo.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ra.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://br.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sd.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://ks.colortex.cn

Py:   resp.json()
来源：http://je.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://mb.nszjky.cn

JS:   await resp.json()
来源：http://zf.yuexingan06.cn

TS:   await resp.json()
来源：http://ei.9csxet.cn


<!-- 参考信息 -->