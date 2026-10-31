代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dq.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wj.nicolike.cn

JS:   /\d+/.test(s)
来源：http://oy.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://dv.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ze.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ze.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://mr.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wf.asd995.cn

[I02] 提取所有匹配
来源：http://al.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://jp.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ha.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xg.bjjhwx.cn

TS:   s.match(/\d+/g)
来源：http://ih.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wo.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ed.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://qw.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ei.bjjhwx.cn

[I03] 提取捕获分组
来源：http://ux.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ju.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yu.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xr.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fn.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tx.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dq.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ih.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xa.hahajie.cn

[I04] 正则替换
来源：http://bl.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xx.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wz.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hc.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wp.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kw.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xb.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rr.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qp.asd995.cn

[I05] 按正则拆分
来源：http://rw.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gd.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ea.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://rq.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://yc.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://mi.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ot.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dc.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://if.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vt.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eq.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jm.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dv.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gt.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tq.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kd.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yj.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://me.szxytkj.cn

[I07] 忽略大小写与多行模式
来源：http://nz.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uz.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sv.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://si.hahajie.cn

TS:   /error/gim
来源：http://wu.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://im.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ba.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://fi.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nd.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://yv.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ja.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://km.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://si.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wc.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kq.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://me.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://to.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qi.szxytkj.cn

================================================================================
来源：http://wx.hahajie.cn

J. 日期与时间
来源：http://me.hnjuh.cn

================================================================================
来源：http://af.bjjhwx.cn

[J01] 获取当前时间
来源：http://nh.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ii.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jf.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://kx.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://xu.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tr.yuexingan06.cn

Go:   time.Now()
来源：http://ae.chemitech.net.cn

Ruby: Time.now
来源：http://al.newstarts.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kn.hahajie.cn

[J02] 格式化输出
来源：http://kq.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dx.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lh.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ab.asd995.cn

TS:   d.toISOString()
来源：http://pm.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tg.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xg.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cx.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mx.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://pk.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://di.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kt.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://vi.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://kt.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qh.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://et.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://ug.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cx.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://un.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dy.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ao.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uw.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://en.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://se.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bw.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ha.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ol.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://sh.asd995.cn

Py:   now + timedelta(days=7)
来源：http://rm.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qs.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://py.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xn.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://tb.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zh.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://lb.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dn.lnxyls.cn

[J06] 计算两时间之差
来源：http://kb.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://rp.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://vr.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iu.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pk.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kt.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://wn.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://re.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://zz.bjjhwx.cn

[J07] 比较两个日期
来源：http://kb.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://yj.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://df.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ad.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jr.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xw.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://di.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xo.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://um.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://pp.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ci.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fc.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hm.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aq.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qz.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yg.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wc.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lq.shtwfgs.cn

[J09] 时区处理
来源：http://xj.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xj.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oe.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cr.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uz.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uf.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vs.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nj.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://lp.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hg.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sx.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jh.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lf.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://in.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cn.shxzukj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xb.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ub.jianghongdianzi.cn

================================================================================
来源：http://gd.szxytkj.cn

K. JSON 与序列化
来源：http://zh.huanxung.cn

================================================================================
来源：http://ea.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://cd.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rg.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zj.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://uv.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://vc.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fg.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://gt.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yp.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kq.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://bg.9csxet.cn

Py:   json.loads(s)
来源：http://sr.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qx.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://oz.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://mr.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ot.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://ex.newstarts.cn

Ruby: JSON.parse(s)
来源：http://jq.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yf.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://jg.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://we.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hg.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://es.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mu.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eg.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lo.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vc.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dk.nicolike.cn

[K04] 读取 JSON 文件
来源：http://ji.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mc.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ar.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ad.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yg.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dr.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ir.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hf.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cg.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://xp.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://nx.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://ay.panjiajie.cn

JS:   structuredClone(obj)
来源：http://ec.panjiajie.cn

TS:   structuredClone(obj)
来源：http://af.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hl.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ni.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oz.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://np.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://sw.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dg.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ao.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ly.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dp.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fm.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://te.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wb.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cf.jctech888.com.cn

[K07] 进制转换
来源：http://qn.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jb.chemitech.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bg.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hh.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xs.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://er.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hm.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pp.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bi.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://bh.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://zu.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ov.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://qw.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://mh.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://or.muxihuayi.cn

Go:   encoding/gob
来源：http://ui.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://bz.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ng.yuexingan06.cn

================================================================================
来源：http://az.nszjky.cn

L. 网络请求
来源：http://ne.shtwfgs.cn

================================================================================
来源：http://tz.szxytkj.cn

[L01] 发送 GET 请求
来源：http://ao.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xq.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bt.shtwfgs.cn

JS:   await fetch(url)
来源：http://rz.chemitech.net.cn

TS:   await fetch(url)
来源：http://xz.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hk.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://ak.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://as.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fb.gzmigu.cn

[L02] 发送 POST JSON
来源：http://bn.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cv.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vd.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aj.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tk.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mk.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oq.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ax.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ap.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://gk.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vr.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wu.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ui.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qd.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://im.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qr.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wu.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xk.shxzukj.cn

[L04] 设置超时
来源：http://yw.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://wb.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qn.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ya.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mp.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bh.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bl.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gx.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qm.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://dy.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uo.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ot.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fu.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aj.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pf.szxytkj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hd.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fs.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kq.szsharing.cn

[L06] 解析响应为 JSON
来源：http://ek.huanxung.cn

Py:   resp.json()
来源：http://wh.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://dx.jctech888.com.cn

JS:   await resp.json()
来源：http://yf.colortex.cn

TS:   await resp.json()
来源：http://iy.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ro.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://du.yuexingan06.cn

Ruby: JSON.parse(resp.body)
来源：http://yt.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://en.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://ym.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yk.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jr.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://fo.chemitech.net.cn


<!-- 参考信息 -->