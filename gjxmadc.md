代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://lr.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://si.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wm.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uc.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jk.yuexingan06.cn

Go:   defer f.Close()
来源：http://gg.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cq.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://be.huixiangedu.cn

================================================================================
来源：http://mv.bookmarksfly.cn

I. 正则表达式
来源：http://vb.shxzukj.cn

================================================================================
来源：http://cq.newstarts.cn

[I01] 判断是否匹配
来源：http://gy.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dp.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ug.colortex.cn

JS:   /\d+/.test(s)
来源：http://jk.521024.cn

TS:   /\d+/.test(s)
来源：http://gm.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hg.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qg.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://eb.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vu.huanxung.cn

[I02] 提取所有匹配
来源：http://be.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://qm.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mn.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fg.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://iw.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gj.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gp.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://sp.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pr.colortex.cn

[I03] 提取捕获分组
来源：http://ci.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://na.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yz.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://du.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xz.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pb.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xl.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vr.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gl.colortex.cn

[I04] 正则替换
来源：http://cx.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cv.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xo.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rd.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jm.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wp.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pq.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fh.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ku.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://nj.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dr.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ca.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://wo.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://si.nicolike.cn

Java: s.split("\\s*,\\s*")
来源：http://uo.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fy.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vh.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fe.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://do.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sh.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qj.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ht.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dj.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vr.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://je.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dm.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nl.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://jy.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ye.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ee.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wp.521024.cn

TS:   /error/gim
来源：http://jx.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jm.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dj.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://of.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pr.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://dt.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gv.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pu.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mk.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qq.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vu.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uv.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://er.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ly.newstarts.cn

================================================================================
来源：http://rw.yuntaijiaju.cn

J. 日期与时间
来源：http://of.bjjhwx.cn

================================================================================
来源：http://hb.bjjhwx.cn

[J01] 获取当前时间
来源：http://ao.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xe.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xo.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://tv.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://mk.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://aq.huixinmuqiang.cn

Go:   time.Now()
来源：http://of.yuexingan06.cn

Ruby: Time.now
来源：http://av.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://io.wgjwhj.cn

[J02] 格式化输出
来源：http://tx.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fe.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gj.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jz.chemitech.net.cn

TS:   d.toISOString()
来源：http://zo.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ep.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fe.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kj.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uv.szsharing.cn

[J03] 字符串解析为日期
来源：http://wz.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zj.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ec.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://ax.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://iw.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://po.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wy.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://by.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ds.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://dq.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jx.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nh.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gx.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://at.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vm.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mr.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ru.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://po.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://lt.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://wl.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://eu.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dt.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bb.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://qq.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://us.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://su.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dv.shtwfgs.cn

[J06] 计算两时间之差
来源：http://kb.asd995.cn

Py:   (end - start).total_seconds()
来源：http://sc.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://id.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xh.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pk.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vq.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://to.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://yi.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://si.hnjuh.cn

[J07] 比较两个日期
来源：http://mt.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://we.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gw.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xo.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fs.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tq.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pn.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fs.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://yl.panjiajie.cn

[J08] 提取年月日与星期
来源：http://at.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mv.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://as.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://af.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gt.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fk.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lr.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ij.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ye.nszjky.cn

[J09] 时区处理
来源：http://bw.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gf.nicolike.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ee.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zs.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zi.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hh.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mr.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jw.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wk.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://xr.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bl.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bw.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hv.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vv.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pi.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ma.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cp.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vh.huanxung.cn

================================================================================
来源：http://ct.yuntaijiaju.cn

K. JSON 与序列化
来源：http://fe.jctech888.com.cn

================================================================================
来源：http://gv.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://mb.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gr.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hr.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://gb.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://ni.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bf.9csxet.cn

Go:   json.Marshal(obj)
来源：http://lx.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://md.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rz.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://rt.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://vf.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dc.nicolike.cn

JS:   JSON.parse(s)
来源：http://bx.panjiajie.cn

TS:   JSON.parse(s)
来源：http://qj.gzmigu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mm.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://hm.nszjky.cn

Ruby: JSON.parse(s)
来源：http://ga.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xv.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://st.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ul.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jn.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bx.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cs.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pt.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xj.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vd.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ga.newstarts.cn

[K04] 读取 JSON 文件
来源：http://sb.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mu.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bt.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ef.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cg.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yl.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gq.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dj.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tf.shxzukj.cn

[K05] 深拷贝对象
来源：http://mk.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://uu.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://de.shxzukj.cn

JS:   structuredClone(obj)
来源：http://kh.nicolike.cn

TS:   structuredClone(obj)
来源：http://do.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kp.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jl.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://no.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cy.szsharing.cn

[K06] 解析 URL 查询串
来源：http://sx.gzmigu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xi.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://df.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://va.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sb.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ns.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ai.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rl.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sc.muxihuayi.cn

[K07] 进制转换
来源：http://tm.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zo.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tv.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zp.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ki.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ck.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tw.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yq.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zk.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://ch.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://ss.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://iy.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://yy.hahajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://ba.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gn.hnjuh.cn

Go:   encoding/gob
来源：http://fy.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://rv.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://in.bookmarksfly.cn

================================================================================
来源：http://pk.shxzukj.cn

L. 网络请求
来源：http://mq.lnxyls.cn

================================================================================
来源：http://zi.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://tp.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nl.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oa.9csxet.cn

JS:   await fetch(url)
来源：http://hv.nszjky.cn

TS:   await fetch(url)
来源：http://eb.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xy.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://br.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dm.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jg.gzmigu.cn

[L02] 发送 POST JSON
来源：http://ng.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://og.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bv.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dp.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mh.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ah.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rk.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ub.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zr.9csxet.cn

[L03] 设置自定义请求头
来源：http://pg.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://px.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lc.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xe.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ix.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eb.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ea.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://te.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cb.9csxet.cn

[L04] 设置超时
来源：http://zl.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://cu.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rq.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jr.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ey.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xv.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hw.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bb.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kz.asd995.cn

[L05] 上传文件（multipart）
来源：http://bv.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vm.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zl.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cl.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hq.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sw.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hy.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lu.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hw.szsharing.cn

[L06] 解析响应为 JSON
来源：http://nr.huixiangedu.cn


<!-- 参考信息 -->