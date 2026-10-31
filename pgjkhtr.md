代发 wailian999

================================================================================
来源：http://rn.hahajie.cn

I. 正则表达式
来源：http://vw.gzmigu.cn

================================================================================
来源：http://bq.9csxet.cn

[I01] 判断是否匹配
来源：http://sa.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ok.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gi.asd995.cn

JS:   /\d+/.test(s)
来源：http://kj.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://bi.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uc.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jf.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://jv.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nc.nicolike.cn

[I02] 提取所有匹配
来源：http://oy.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://dd.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ga.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jt.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://ug.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yq.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vk.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://lg.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aw.wgjwhj.cn

[I03] 提取捕获分组
来源：http://mr.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://og.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zg.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ko.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vb.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hc.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ym.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://md.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zu.newstarts.cn

[I04] 正则替换
来源：http://uq.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kc.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sv.szxytkj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jv.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xz.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fi.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fi.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uc.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rc.huixiangedu.cn

[I05] 按正则拆分
来源：http://se.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zk.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://du.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://ad.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://mg.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://dd.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xv.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uz.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xh.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nw.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mb.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vn.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ys.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ff.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://of.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mz.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xh.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dz.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://ua.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://le.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fy.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vc.panjiajie.cn

TS:   /error/gim
来源：http://hn.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lv.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nb.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://tm.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qm.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://sq.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rc.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pr.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mi.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://la.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zt.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ot.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rx.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aa.bjjhwx.cn

================================================================================
来源：http://ob.bookmarksfly.cn

J. 日期与时间
来源：http://lq.gzmigu.cn

================================================================================
来源：http://bb.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://el.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qp.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rd.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://dc.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://ms.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pj.shxzskj.cn

Go:   time.Now()
来源：http://cg.jianghongdianzi.cn

Ruby: Time.now
来源：http://bg.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xr.huixinmuqiang.cn

[J02] 格式化输出
来源：http://fl.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pi.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hv.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ly.wgjwhj.cn

TS:   d.toISOString()
来源：http://ks.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lb.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://on.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jv.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sl.colortex.cn

[J03] 字符串解析为日期
来源：http://lj.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yl.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nn.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://ld.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://cm.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ni.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kq.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://dn.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ad.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://qq.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yw.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mi.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tb.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gq.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iv.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hl.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://at.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tl.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://nq.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://sz.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qh.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fp.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uv.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://gs.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ol.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://sl.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dv.chemitech.net.cn

[J06] 计算两时间之差
来源：http://sk.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://wv.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://pt.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nd.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qs.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mr.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://cl.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://oa.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://hj.muxihuayi.cn

[J07] 比较两个日期
来源：http://dg.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://sx.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hb.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zk.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ct.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iu.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vd.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ou.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://ks.lnxyls.cn

[J08] 提取年月日与星期
来源：http://la.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sr.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wa.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ur.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wh.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zb.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ba.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xa.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hy.asd995.cn

[J09] 时区处理
来源：http://cj.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ak.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ey.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lr.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sl.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gu.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yd.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hu.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://po.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://yq.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://db.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hm.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ze.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ka.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nz.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ov.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dz.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cq.chemitech.net.cn

================================================================================
来源：http://vk.newstarts.cn

K. JSON 与序列化
来源：http://tl.muxihuayi.cn

================================================================================
来源：http://oa.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://gb.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oa.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vv.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://fx.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://ap.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sf.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://xd.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nf.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mw.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://yn.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://rp.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bv.shxzskj.cn

JS:   JSON.parse(s)
来源：http://nu.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://qe.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vn.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://gi.521024.cn

Ruby: JSON.parse(s)
来源：http://jy.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ul.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://cv.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://px.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fc.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ej.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vq.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nu.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tu.521024.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zn.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fv.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://gy.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yf.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cc.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hf.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zv.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gb.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wq.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ir.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://se.lnxyls.cn

[K05] 深拷贝对象
来源：http://xc.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://as.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://fj.szsharing.cn

JS:   structuredClone(obj)
来源：http://kx.nicolike.cn

TS:   structuredClone(obj)
来源：http://tl.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rl.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sb.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cs.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pp.bjjhwx.cn

[K06] 解析 URL 查询串
来源：http://us.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gf.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aj.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jg.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ya.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yz.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ar.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nf.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sf.huixinmuqiang.cn

[K07] 进制转换
来源：http://nh.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mn.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pz.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oc.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dd.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rs.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nw.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qk.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yq.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://tx.521024.cn

Py:   pickle.dumps(obj)
来源：http://lp.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rz.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://hq.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://jw.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mo.huixiangedu.cn

Go:   encoding/gob
来源：http://pc.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://qe.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ic.chemitech.net.cn

================================================================================
来源：http://nj.bookmarksfly.cn

L. 网络请求
来源：http://pv.huixinmuqiang.cn

================================================================================
来源：http://ke.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://of.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fn.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gz.9csxet.cn

JS:   await fetch(url)
来源：http://bq.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://ag.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bo.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://jp.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mr.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aw.newstarts.cn

[L02] 发送 POST JSON
来源：http://sn.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://db.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fr.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jv.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sf.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jr.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xk.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://do.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ii.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://hu.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dd.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bf.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dl.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://um.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ku.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lc.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ah.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xi.521024.cn

[L04] 设置超时
来源：http://hy.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://sa.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kq.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ao.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kp.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://he.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://py.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oj.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qg.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://id.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ma.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zw.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wt.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vd.nszjky.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vm.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hy.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ed.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dm.newstarts.cn

[L06] 解析响应为 JSON
来源：http://lv.szxytkj.cn

Py:   resp.json()
来源：http://ib.hahajie.cn

PHP:  json_decode($body, true);
来源：http://cr.newstarts.cn

JS:   await resp.json()
来源：http://na.bjjhwx.cn

TS:   await resp.json()
来源：http://gz.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vv.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ag.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://qk.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ro.haigaiapp.cn


<!-- 参考信息 -->