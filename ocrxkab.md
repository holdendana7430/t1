代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://em.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pc.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://vp.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://qt.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dg.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jx.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://pp.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sv.jctech888.com.cn

[I02] 提取所有匹配
来源：http://yb.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://br.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vl.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wm.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://jr.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ne.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ug.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://hr.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zp.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://gr.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ni.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qe.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pz.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xh.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gz.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lv.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yn.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kx.newstarts.cn

[I04] 正则替换
来源：http://qe.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ee.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ya.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://je.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ld.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://an.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yg.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pt.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xh.nicolike.cn

[I05] 按正则拆分
来源：http://gs.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bm.asd995.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ba.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://nu.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://jq.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://ez.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fg.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hz.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qw.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gs.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vq.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yl.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mn.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ch.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nm.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://te.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ka.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uo.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://ph.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wg.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ba.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mp.szxytkj.cn

TS:   /error/gim
来源：http://ju.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bl.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xw.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://uy.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ih.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://jg.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xd.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ff.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oj.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ol.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jh.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://li.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ua.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://it.9csxet.cn

================================================================================
来源：http://bs.hahajie.cn

J. 日期与时间
来源：http://fa.huixinmuqiang.cn

================================================================================
来源：http://vv.newstarts.cn

[J01] 获取当前时间
来源：http://ks.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://iu.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jz.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://rt.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://tt.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vk.haigaiapp.cn

Go:   time.Now()
来源：http://sy.szsharing.cn

Ruby: Time.now
来源：http://er.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ia.jianghongdianzi.cn

[J02] 格式化输出
来源：http://bb.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://of.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wo.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wl.shxzskj.cn

TS:   d.toISOString()
来源：http://dj.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wz.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hu.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mt.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ok.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://sp.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://es.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wf.colortex.cn

JS:   new Date("2024-01-02")
来源：http://md.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://le.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://es.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ge.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://sa.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yz.huanxung.cn

[J04] 时间戳与日期互转
来源：http://ws.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oa.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bw.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pi.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dl.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sp.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ja.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://st.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bs.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://rm.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://hl.jianghongdianzi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yg.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yo.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://it.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://ob.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nf.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://kp.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ip.szxytkj.cn

[J06] 计算两时间之差
来源：http://zn.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://ko.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://oz.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gi.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cu.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bh.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://wj.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://hs.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://mx.yuexingan06.cn

[J07] 比较两个日期
来源：http://yv.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://zh.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yf.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pj.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wg.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nf.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lk.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gu.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://bf.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://hm.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oj.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pa.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sn.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ti.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gz.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ta.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gj.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ao.521024.cn

[J09] 时区处理
来源：http://tp.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oh.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sv.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jg.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gd.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ki.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zx.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xy.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xh.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://ct.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hq.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cx.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ia.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bo.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xo.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pp.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iv.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mz.newstarts.cn

================================================================================
来源：http://za.asd995.cn

K. JSON 与序列化
来源：http://rw.gzmigu.cn

================================================================================
来源：http://uf.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://gr.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xc.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yi.asd995.cn

JS:   JSON.stringify(obj)
来源：http://ll.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://gy.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ua.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://su.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vf.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lv.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://sf.wgjwhj.cn

Py:   json.loads(s)
来源：http://ft.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eg.newstarts.cn

JS:   JSON.parse(s)
来源：http://mf.nicolike.cn

TS:   JSON.parse(s)
来源：http://tb.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uw.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://ap.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://wm.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ev.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://cv.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kb.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pk.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ha.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://md.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://de.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xf.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nz.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lj.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://co.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eo.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hs.szsharing.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ar.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xu.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mt.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://az.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zg.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ke.nicolike.cn

[K05] 深拷贝对象
来源：http://iu.521024.cn

Py:   copy.deepcopy(obj)
来源：http://hy.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://bp.nszjky.cn

JS:   structuredClone(obj)
来源：http://ez.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://ho.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lw.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lx.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rs.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ht.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://tn.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eo.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ox.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ku.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zf.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mt.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://df.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yn.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qh.chemitech.net.cn

[K07] 进制转换
来源：http://zt.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xx.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ny.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vo.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pj.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bs.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ke.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://og.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ai.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://nm.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://pc.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cr.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://cy.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://pn.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://js.gzmigu.cn

Go:   encoding/gob
来源：http://tc.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://bc.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lx.haigaiapp.cn

================================================================================
来源：http://fe.wgjwhj.cn

L. 网络请求
来源：http://au.huixiangedu.cn

================================================================================
来源：http://jg.521024.cn

[L01] 发送 GET 请求
来源：http://zs.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://np.yuexingan06.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nd.nicolike.cn

JS:   await fetch(url)
来源：http://qu.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://nj.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://no.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://cb.huixiangedu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://og.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wz.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://di.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://za.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yk.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mr.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ul.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tj.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xt.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rs.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nt.nicolike.cn

[L03] 设置自定义请求头
来源：http://pl.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jz.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zv.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hq.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bd.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kr.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cg.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pg.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://we.asd995.cn

[L04] 设置超时
来源：http://tw.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://pk.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ko.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vy.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ad.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pt.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://if.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iq.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nt.szsharing.cn

[L05] 上传文件（multipart）
来源：http://ug.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wf.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sg.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zk.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hg.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vr.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ft.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yq.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://as.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://rz.hnjuh.cn

Py:   resp.json()
来源：http://cm.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://xh.colortex.cn

JS:   await resp.json()
来源：http://lz.nicolike.cn

TS:   await resp.json()
来源：http://qn.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wv.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gf.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://rt.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mk.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://qw.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ea.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ui.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://bo.nszjky.cn


<!-- 参考信息 -->