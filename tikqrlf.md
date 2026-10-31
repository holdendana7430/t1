代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://et.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iq.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fy.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hi.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zw.yuexingan06.cn

Go:   defer f.Close()
来源：http://gw.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ik.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wt.szxytkj.cn

================================================================================
来源：http://xj.bookmarksfly.cn

I. 正则表达式
来源：http://ro.huixiangedu.cn

================================================================================
来源：http://sb.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://sf.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zk.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rp.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://uz.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://vp.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vv.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ry.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://ay.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bp.yuexingan06.cn

[I02] 提取所有匹配
来源：http://ob.szsharing.cn

Py:   re.findall(r"\d+", s)
来源：http://np.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mc.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://np.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://ym.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gh.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wj.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://pf.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fs.hnjuh.cn

[I03] 提取捕获分组
来源：http://kl.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vo.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hj.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://al.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lr.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oc.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://de.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://st.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oa.panjiajie.cn

[I04] 正则替换
来源：http://my.szxytkj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ag.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ot.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pm.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kg.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hh.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://em.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ei.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xs.szxytkj.cn

[I05] 按正则拆分
来源：http://fi.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pr.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xp.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://ll.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://oj.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://gw.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gf.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sy.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ah.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yl.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ty.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pz.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yw.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ep.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vc.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gx.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xe.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zw.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://mz.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tf.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ia.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rn.bookmarksfly.cn

TS:   /error/gim
来源：http://zg.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ut.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fr.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://nr.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bq.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://ye.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uq.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pi.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ft.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mi.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bh.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zy.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sj.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oi.jctech888.com.cn

================================================================================
来源：http://ud.huixiangedu.cn

J. 日期与时间
来源：http://cv.521024.cn

================================================================================
来源：http://of.huanxung.cn

[J01] 获取当前时间
来源：http://on.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lg.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://az.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://se.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://cf.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ky.bjjhwx.cn

Go:   time.Now()
来源：http://op.shxzskj.cn

Ruby: Time.now
来源：http://jc.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sg.bjjhwx.cn

[J02] 格式化输出
来源：http://ud.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kf.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://du.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lh.nicolike.cn

TS:   d.toISOString()
来源：http://ra.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dv.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xx.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ad.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://en.colortex.cn

[J03] 字符串解析为日期
来源：http://xd.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yn.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wh.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://yo.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://og.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lc.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rw.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://dz.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rv.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://ds.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vf.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vk.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ia.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pq.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pt.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ld.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ul.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zl.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://kn.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://xk.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ks.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yc.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ff.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://cf.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qm.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://bo.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tj.gzmigu.cn

[J06] 计算两时间之差
来源：http://ur.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://ko.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://hf.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gd.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nj.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xc.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://dz.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://yg.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://ue.newstarts.cn

[J07] 比较两个日期
来源：http://fm.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://uc.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hg.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uc.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rw.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rb.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cv.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tl.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://nd.9csxet.cn

[J08] 提取年月日与星期
来源：http://ys.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vc.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ib.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hb.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kd.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eq.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wk.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cb.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ao.asd995.cn

[J09] 时区处理
来源：http://im.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vz.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://za.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mq.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tu.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://am.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fr.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vx.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uv.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://eq.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wh.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vb.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://em.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://so.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yy.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eg.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://up.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dk.9csxet.cn

================================================================================
来源：http://pd.shxzukj.cn

K. JSON 与序列化
来源：http://fl.yuexingan06.cn

================================================================================
来源：http://ud.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://dr.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bf.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://go.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://oo.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://kk.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bw.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://oj.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jk.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wj.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://au.shtwfgs.cn

Py:   json.loads(s)
来源：http://be.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sp.hnjuh.cn

JS:   JSON.parse(s)
来源：http://hr.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://ny.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qh.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://oz.newstarts.cn

Ruby: JSON.parse(s)
来源：http://ny.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nq.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://he.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nd.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aj.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jk.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yi.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://he.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wa.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hm.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bt.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://yo.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gp.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rr.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zp.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dk.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://so.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://he.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wu.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wu.shtwfgs.cn

[K05] 深拷贝对象
来源：http://fr.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://br.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://jh.gzmigu.cn

JS:   structuredClone(obj)
来源：http://uh.colortex.cn

TS:   structuredClone(obj)
来源：http://lz.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ig.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nk.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zk.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://eu.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://rc.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kk.huixinmuqiang.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://or.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dm.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ci.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dm.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fw.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ul.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zd.jianghongdianzi.cn

[K07] 进制转换
来源：http://al.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lz.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wt.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yv.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nw.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pk.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bh.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ze.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qb.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://yn.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://oi.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://eo.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://tp.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://xw.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dv.gzmigu.cn

Go:   encoding/gob
来源：http://fz.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://fz.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ig.lnxyls.cn

================================================================================
来源：http://zg.jctech888.com.cn

L. 网络请求
来源：http://kk.wgjwhj.cn

================================================================================
来源：http://gi.newstarts.cn

[L01] 发送 GET 请求
来源：http://jy.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ih.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ef.hnjuh.cn

JS:   await fetch(url)
来源：http://nn.newstarts.cn

TS:   await fetch(url)
来源：http://dt.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cr.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://co.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dc.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iz.newstarts.cn

[L02] 发送 POST JSON
来源：http://qa.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vd.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uc.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iq.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dk.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qs.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qy.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://au.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gb.szxytkj.cn

[L03] 设置自定义请求头
来源：http://gl.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zd.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tk.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rr.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lb.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hr.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ek.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ti.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wh.shxzskj.cn

[L04] 设置超时
来源：http://mx.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://dx.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ef.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ap.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dn.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cw.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hd.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pb.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pt.nszjky.cn

[L05] 上传文件（multipart）
来源：http://mx.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://da.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://al.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bn.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gu.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wi.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yr.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hn.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ff.huanxung.cn

[L06] 解析响应为 JSON
来源：http://uy.yuntaijiaju.cn


<!-- 参考信息 -->