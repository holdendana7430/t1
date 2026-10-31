代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://gs.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vw.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hc.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://aa.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ui.shtwfgs.cn

Go:   defer f.Close()
来源：http://ls.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fi.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jm.nszjky.cn

================================================================================
来源：http://hp.jianghongdianzi.cn

I. 正则表达式
来源：http://on.lnxyls.cn

================================================================================
来源：http://py.muxihuayi.cn

[I01] 判断是否匹配
来源：http://vy.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eg.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zo.shtwfgs.cn

JS:   /\d+/.test(s)
来源：http://om.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://vl.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dc.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bn.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://pb.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mr.bjjhwx.cn

[I02] 提取所有匹配
来源：http://aa.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://xr.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dx.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cp.lnxyls.cn

TS:   s.match(/\d+/g)
来源：http://gz.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vt.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://he.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://gf.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cw.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://xr.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yq.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xf.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://si.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kd.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://of.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oe.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oq.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ks.haigaiapp.cn

[I04] 正则替换
来源：http://nf.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wq.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yv.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uc.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xi.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ea.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zo.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yv.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xq.colortex.cn

[I05] 按正则拆分
来源：http://tb.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xv.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fs.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://pq.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://cx.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://mb.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ee.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cy.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bc.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uj.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hv.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gw.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bi.521024.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wp.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mu.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wm.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://np.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fg.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://yh.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dk.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://op.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ls.9csxet.cn

TS:   /error/gim
来源：http://bg.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zt.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ji.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://wd.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kp.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://qz.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://za.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ax.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lf.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gv.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ii.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uw.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hg.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lv.hahajie.cn

================================================================================
来源：http://pr.shxzukj.cn

J. 日期与时间
来源：http://jp.521024.cn

================================================================================
来源：http://uw.shxzskj.cn

[J01] 获取当前时间
来源：http://mi.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hj.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sp.lnxyls.cn

JS:   new Date();  Date.now()
来源：http://ml.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://fu.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hl.haigaiapp.cn

Go:   time.Now()
来源：http://yv.wgjwhj.cn

Ruby: Time.now
来源：http://kz.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yp.hnjuh.cn

[J02] 格式化输出
来源：http://ak.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wn.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ty.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jk.nszjky.cn

TS:   d.toISOString()
来源：http://ic.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://da.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://md.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hs.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pi.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://xw.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hj.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pr.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://fc.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://vq.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gn.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dh.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://hx.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hk.9csxet.cn

[J04] 时间戳与日期互转
来源：http://nv.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mx.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://km.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sb.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://aj.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qz.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qg.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eb.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yp.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://gh.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://em.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rz.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lr.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sx.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://lx.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sq.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://iy.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xb.szxytkj.cn

[J06] 计算两时间之差
来源：http://qh.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://hu.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://vw.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jb.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jg.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nw.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://tj.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://af.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://wa.jctech888.com.cn

[J07] 比较两个日期
来源：http://ng.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://wl.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gz.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uf.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xn.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jk.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zb.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ir.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ou.9csxet.cn

[J08] 提取年月日与星期
来源：http://pj.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hw.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qm.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ms.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://la.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ai.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ma.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rl.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fz.wgjwhj.cn

[J09] 时区处理
来源：http://jd.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qj.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hw.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wx.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qo.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vs.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ly.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sy.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yc.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://tw.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wa.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nl.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ck.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mj.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://or.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hr.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xu.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ri.colortex.cn

================================================================================
来源：http://ci.shxzskj.cn

K. JSON 与序列化
来源：http://hl.panjiajie.cn

================================================================================
来源：http://wp.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://ga.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xf.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sc.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://mh.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://rw.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dq.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://vr.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lm.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dp.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://xs.gzmigu.cn

Py:   json.loads(s)
来源：http://iv.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://il.shxzukj.cn

JS:   JSON.parse(s)
来源：http://yw.lnxyls.cn

TS:   JSON.parse(s)
来源：http://wv.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://um.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://rr.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://zc.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nn.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://en.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ji.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hp.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jb.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ps.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ln.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gh.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fq.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://br.szsharing.cn

[K04] 读取 JSON 文件
来源：http://tx.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yg.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xf.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wz.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wp.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gk.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rh.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gh.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ad.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://sn.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://vw.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://cy.shxzskj.cn

JS:   structuredClone(obj)
来源：http://ow.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://dj.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nr.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qn.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ii.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zw.colortex.cn

[K06] 解析 URL 查询串
来源：http://kc.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ak.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eh.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ss.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vl.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dn.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://eo.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vv.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kt.huanxung.cn

[K07] 进制转换
来源：http://vz.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sy.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kt.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wv.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rk.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://en.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qn.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cb.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://mp.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://qb.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ax.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://sn.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://tb.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lb.nicolike.cn

Go:   encoding/gob
来源：http://js.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://un.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ud.9csxet.cn

================================================================================
来源：http://tj.szsharing.cn

L. 网络请求
来源：http://lv.521024.cn

================================================================================
来源：http://ry.nszjky.cn

[L01] 发送 GET 请求
来源：http://ka.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lm.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ff.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://em.yuexingan06.cn

TS:   await fetch(url)
来源：http://gu.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jq.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://lt.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wd.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://re.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://tz.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sa.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hj.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bd.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iv.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uv.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hv.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://za.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cu.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://md.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tg.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mo.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ul.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ut.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://on.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mc.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kw.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dn.asd995.cn

[L04] 设置超时
来源：http://bt.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://ce.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mn.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iz.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qq.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dj.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zu.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wt.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ou.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://mt.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ym.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fz.nszjky.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mt.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ki.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qi.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dn.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ll.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://al.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://lj.jctech888.com.cn


<!-- 参考信息 -->