代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://zs.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://la.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rs.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yl.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zc.521024.cn

Go:   defer f.Close()
来源：http://nx.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qh.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wq.szxytkj.cn

================================================================================
来源：http://mg.jianghongdianzi.cn

I. 正则表达式
来源：http://sn.hahajie.cn

================================================================================
来源：http://cg.shtwfgs.cn

[I01] 判断是否匹配
来源：http://nh.huixiangedu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wu.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fh.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://mh.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://zs.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bx.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mc.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://gf.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bo.asd995.cn

[I02] 提取所有匹配
来源：http://gd.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://cr.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mu.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tv.bjjhwx.cn

TS:   s.match(/\d+/g)
来源：http://rn.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zq.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qg.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://kr.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rq.chemitech.net.cn

[I03] 提取捕获分组
来源：http://pq.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ym.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://se.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ls.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ao.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tp.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hp.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kn.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vn.hahajie.cn

[I04] 正则替换
来源：http://pf.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ke.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ak.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jg.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mn.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rd.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fm.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vs.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vn.szsharing.cn

[I05] 按正则拆分
来源：http://gk.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pu.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nw.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://pt.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://oe.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://xu.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tr.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nr.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wq.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ej.bookmarksfly.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rg.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hf.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cs.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uh.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jq.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xy.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://be.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ne.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://bj.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mv.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nv.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qo.huixiangedu.cn

TS:   /error/gim
来源：http://wt.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fy.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tn.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://rp.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kx.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://lg.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tq.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yu.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lo.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qk.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ri.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iz.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tv.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mr.huixinmuqiang.cn

================================================================================
来源：http://la.huixiangedu.cn

J. 日期与时间
来源：http://jl.huanxung.cn

================================================================================
来源：http://cb.gzmigu.cn

[J01] 获取当前时间
来源：http://ge.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rh.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mp.9csxet.cn

JS:   new Date();  Date.now()
来源：http://kp.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://ke.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ie.huixiangedu.cn

Go:   time.Now()
来源：http://mk.panjiajie.cn

Ruby: Time.now
来源：http://yl.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bq.chemitech.net.cn

[J02] 格式化输出
来源：http://xh.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://by.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tf.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ve.panjiajie.cn

TS:   d.toISOString()
来源：http://if.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fr.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mk.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ea.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oh.panjiajie.cn

[J03] 字符串解析为日期
来源：http://ci.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gm.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xd.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://kd.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://dq.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ja.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pp.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://li.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ci.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://na.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yh.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pz.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ja.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dk.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hr.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zq.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dh.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uj.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://wp.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://jg.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gx.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ad.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://en.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://ed.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dy.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://be.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ry.szsharing.cn

[J06] 计算两时间之差
来源：http://jb.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://st.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://fg.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vp.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ox.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ic.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://qt.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://dw.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://bk.huanxung.cn

[J07] 比较两个日期
来源：http://dg.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://ao.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bi.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uu.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ld.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ao.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oq.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ir.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://ay.szsharing.cn

[J08] 提取年月日与星期
来源：http://cz.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ha.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://er.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oz.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wh.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vc.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ay.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nt.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://in.huixiangedu.cn

[J09] 时区处理
来源：http://oj.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cq.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pw.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ps.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kf.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mo.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zk.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kh.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://br.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://xg.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://eq.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dw.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nm.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oa.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nh.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rt.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ix.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hx.panjiajie.cn

================================================================================
来源：http://vl.szsharing.cn

K. JSON 与序列化
来源：http://qo.hnjuh.cn

================================================================================
来源：http://lg.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://yu.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pe.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kc.asd995.cn

JS:   JSON.stringify(obj)
来源：http://ya.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://fk.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nc.nszjky.cn

Go:   json.Marshal(obj)
来源：http://kg.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://iw.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sf.asd995.cn

[K02] JSON 字符串转对象
来源：http://bv.asd995.cn

Py:   json.loads(s)
来源：http://pe.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lq.szsharing.cn

JS:   JSON.parse(s)
来源：http://xs.gzmigu.cn

TS:   JSON.parse(s)
来源：http://bf.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hc.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://nx.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://sk.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gx.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://ic.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://um.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uz.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ow.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ox.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zz.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dc.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ci.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://es.nicolike.cn

[K04] 读取 JSON 文件
来源：http://np.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lu.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dh.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mz.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sn.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kc.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rh.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zv.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eg.wgjwhj.cn

[K05] 深拷贝对象
来源：http://bj.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://wr.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://ln.szsharing.cn

JS:   structuredClone(obj)
来源：http://fn.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://zu.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qx.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gz.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zk.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uq.colortex.cn

[K06] 解析 URL 查询串
来源：http://cb.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ld.huixinmuqiang.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ax.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ip.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tc.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eg.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dk.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mv.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nl.szsharing.cn

[K07] 进制转换
来源：http://qi.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dp.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kr.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rt.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cx.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cc.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jg.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ka.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nd.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://qx.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://kl.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tn.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://rb.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://oe.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uy.colortex.cn

Go:   encoding/gob
来源：http://wp.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://wg.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tg.haigaiapp.cn

================================================================================
来源：http://oi.huixiangedu.cn

L. 网络请求
来源：http://xy.asd995.cn

================================================================================
来源：http://jk.huixinmuqiang.cn

[L01] 发送 GET 请求
来源：http://nr.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jt.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nq.szsharing.cn

JS:   await fetch(url)
来源：http://sh.shtwfgs.cn

TS:   await fetch(url)
来源：http://ns.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aw.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://rf.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://js.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://he.hahajie.cn

[L02] 发送 POST JSON
来源：http://de.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ns.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xm.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kc.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qi.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hm.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fl.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qx.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bd.szsharing.cn

[L03] 设置自定义请求头
来源：http://bj.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ib.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://db.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hg.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lt.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lb.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oh.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gf.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pm.szsharing.cn

[L04] 设置超时
来源：http://yp.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://ub.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qj.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rf.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nv.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qd.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xk.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sc.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ht.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://dm.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tl.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bb.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bn.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yq.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://po.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cs.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vb.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xz.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://ac.bookmarksfly.cn


<!-- 参考信息 -->