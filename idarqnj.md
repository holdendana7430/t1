代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ed.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rq.huanxung.cn

JS:   /\d+/.test(s)
来源：http://vp.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://dq.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iy.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://co.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://cm.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fn.asd995.cn

[I02] 提取所有匹配
来源：http://lp.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://ov.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vh.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hq.bjjhwx.cn

TS:   s.match(/\d+/g)
来源：http://gv.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zr.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uo.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://gv.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://us.jctech888.com.cn

[I03] 提取捕获分组
来源：http://rb.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://im.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://aq.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fe.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tf.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qa.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fv.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zn.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cv.muxihuayi.cn

[I04] 正则替换
来源：http://tu.gzmigu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fa.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zq.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rg.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mc.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wu.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pv.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://co.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iq.colortex.cn

[I05] 按正则拆分
来源：http://mq.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wn.colortex.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wi.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://zw.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://av.bookmarksfly.cn

Java: s.split("\\s*,\\s*")
来源：http://uj.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wj.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://od.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ns.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://si.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hh.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iy.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xl.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ta.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ka.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ql.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ju.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tv.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://qe.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://df.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gk.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sf.panjiajie.cn

TS:   /error/gim
来源：http://ed.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oh.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rd.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://pq.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rg.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://io.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ju.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ee.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sa.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ly.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ey.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nz.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kz.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fs.asd995.cn

================================================================================
来源：http://at.panjiajie.cn

J. 日期与时间
来源：http://qq.gzmigu.cn

================================================================================
来源：http://sz.hnjuh.cn

[J01] 获取当前时间
来源：http://le.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yo.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qr.szsharing.cn

JS:   new Date();  Date.now()
来源：http://jg.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://bg.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vt.bookmarksfly.cn

Go:   time.Now()
来源：http://qq.asd995.cn

Ruby: Time.now
来源：http://qx.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lv.lnxyls.cn

[J02] 格式化输出
来源：http://su.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mp.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vm.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://no.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://vq.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xg.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://te.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://no.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://da.lnxyls.cn

[J03] 字符串解析为日期
来源：http://ac.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oq.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fg.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://fg.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://uu.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://il.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gk.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://mi.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://td.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://gz.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ck.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qd.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zh.gzmigu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uh.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lr.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sw.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vf.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vx.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://ag.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://wp.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wj.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nh.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pm.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://lw.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fp.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://ly.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tj.jctech888.com.cn

[J06] 计算两时间之差
来源：http://pd.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://qu.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://ru.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vc.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bx.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hi.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://hx.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://gf.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://kc.szsharing.cn

[J07] 比较两个日期
来源：http://ed.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://kr.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://md.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hv.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jq.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ij.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ip.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gu.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://qj.newstarts.cn

[J08] 提取年月日与星期
来源：http://zj.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vj.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://in.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kg.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cv.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xo.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://eo.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nt.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ph.muxihuayi.cn

[J09] 时区处理
来源：http://py.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://az.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://so.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sz.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wt.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ud.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nh.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zp.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zp.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://ga.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oj.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hj.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://le.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fi.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xm.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lc.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gf.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gx.muxihuayi.cn

================================================================================
来源：http://td.bookmarksfly.cn

K. JSON 与序列化
来源：http://kx.colortex.cn

================================================================================
来源：http://as.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://qk.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wv.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zo.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://lh.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://lc.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mq.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://nl.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fu.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ez.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://sb.wgjwhj.cn

Py:   json.loads(s)
来源：http://uu.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lc.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://sf.panjiajie.cn

TS:   JSON.parse(s)
来源：http://nq.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hv.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://fu.newstarts.cn

Ruby: JSON.parse(s)
来源：http://qf.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yx.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://ut.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cs.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sh.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vl.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wc.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ok.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mt.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gd.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jd.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://xu.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zl.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qa.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cx.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://he.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wy.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bu.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yd.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bu.9csxet.cn

[K05] 深拷贝对象
来源：http://fl.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://ip.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://yv.9csxet.cn

JS:   structuredClone(obj)
来源：http://mo.szxytkj.cn

TS:   structuredClone(obj)
来源：http://tc.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jj.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nf.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yf.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nx.521024.cn

[K06] 解析 URL 查询串
来源：http://ab.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sx.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ku.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://im.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qp.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://al.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://op.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://se.shxzukj.cn

[K07] 进制转换
来源：http://ny.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oj.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jy.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xp.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://px.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gi.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uy.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zg.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nh.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://nk.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://mu.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://su.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://vr.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://oe.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hr.newstarts.cn

Go:   encoding/gob
来源：http://ql.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://zn.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qb.haigaiapp.cn

================================================================================
来源：http://gq.newstarts.cn

L. 网络请求
来源：http://ch.shxzskj.cn

================================================================================
来源：http://gy.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://sk.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zu.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ro.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://gl.hnjuh.cn

TS:   await fetch(url)
来源：http://bv.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bs.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://yu.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://an.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fr.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://zs.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hg.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://px.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://de.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yw.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gi.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://by.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cg.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cx.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://kb.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://et.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yz.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sf.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://el.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sg.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ah.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fe.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gh.szxytkj.cn

[L04] 设置超时
来源：http://aq.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://gj.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ue.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kr.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ng.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kh.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wl.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xu.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cy.colortex.cn

[L05] 上传文件（multipart）
来源：http://vo.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sg.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tb.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ci.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://so.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wd.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tm.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ki.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sm.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://py.shtwfgs.cn

Py:   resp.json()
来源：http://sp.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://hk.yuexingan06.cn

JS:   await resp.json()
来源：http://rw.colortex.cn

TS:   await resp.json()
来源：http://lp.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tv.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cu.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://nn.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ei.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://ou.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gy.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hv.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://wp.yuexingan06.cn


<!-- 参考信息 -->