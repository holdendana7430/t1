代发 wailian999

[I02] 提取所有匹配
来源：http://mq.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://kl.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xk.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ss.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://dv.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fs.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oi.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://qf.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nc.wgjwhj.cn

[I03] 提取捕获分组
来源：http://pi.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ah.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mn.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fb.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tt.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ke.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tz.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wj.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ci.lnxyls.cn

[I04] 正则替换
来源：http://ed.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xy.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rc.muxihuayi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zn.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cy.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ez.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xq.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jg.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sp.shtwfgs.cn

[I05] 按正则拆分
来源：http://jl.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ix.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vw.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://ny.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://xd.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://ng.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ag.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mn.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wm.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yo.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gy.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yz.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gc.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dh.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ey.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cz.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://he.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hy.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://bg.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hs.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ze.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mj.521024.cn

TS:   /error/gim
来源：http://ds.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pm.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://om.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://iu.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vd.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://lr.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ou.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dd.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jm.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oi.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xh.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kr.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rd.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iw.shtwfgs.cn

================================================================================
来源：http://uj.asd995.cn

J. 日期与时间
来源：http://ww.bjjhwx.cn

================================================================================
来源：http://qx.asd995.cn

[J01] 获取当前时间
来源：http://mu.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bq.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mu.asd995.cn

JS:   new Date();  Date.now()
来源：http://qt.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://sh.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qz.nicolike.cn

Go:   time.Now()
来源：http://cs.wgjwhj.cn

Ruby: Time.now
来源：http://ji.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pf.muxihuayi.cn

[J02] 格式化输出
来源：http://iu.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zc.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pv.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vw.wgjwhj.cn

TS:   d.toISOString()
来源：http://qe.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nn.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ou.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xe.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ox.asd995.cn

[J03] 字符串解析为日期
来源：http://mw.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ia.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qx.asd995.cn

JS:   new Date("2024-01-02")
来源：http://ye.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://oe.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uj.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://re.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://ub.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eq.huanxung.cn

[J04] 时间戳与日期互转
来源：http://xs.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qq.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hy.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gp.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ph.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://br.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nk.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wr.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bb.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://tg.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://zs.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xm.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ex.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ll.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://sp.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dz.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://qe.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://if.yuexingan06.cn

[J06] 计算两时间之差
来源：http://mc.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://lz.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://rw.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tk.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bz.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zz.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://vw.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://np.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://ae.nicolike.cn

[J07] 比较两个日期
来源：http://ua.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://cy.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ps.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tn.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ug.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ut.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gy.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uo.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://mr.shxzskj.cn

[J08] 提取年月日与星期
来源：http://fu.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://de.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mq.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lf.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ob.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sp.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zu.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ql.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ct.jianghongdianzi.cn

[J09] 时区处理
来源：http://an.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bd.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eo.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xy.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qh.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wm.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://an.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://po.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yo.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://dy.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bn.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ie.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hd.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ew.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pn.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zv.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://po.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ce.huixinmuqiang.cn

================================================================================
来源：http://th.wgjwhj.cn

K. JSON 与序列化
来源：http://ww.huixiangedu.cn

================================================================================
来源：http://ub.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://xk.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fp.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yx.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://dn.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://au.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rt.newstarts.cn

Go:   json.Marshal(obj)
来源：http://cd.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ty.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gn.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://oi.asd995.cn

Py:   json.loads(s)
来源：http://dv.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://at.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://qz.szsharing.cn

TS:   JSON.parse(s)
来源：http://hw.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://op.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://bi.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://eb.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rm.bookmarksfly.cn

[K03] JSON 美化输出（带缩进）
来源：http://hp.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mo.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nq.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wg.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ti.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ed.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kd.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tr.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ni.szsharing.cn

[K04] 读取 JSON 文件
来源：http://cw.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eg.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fn.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ds.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ya.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ht.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iy.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://eu.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aj.colortex.cn

[K05] 深拷贝对象
来源：http://zd.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://sx.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://rf.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://qy.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://bb.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oj.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ce.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ay.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://iu.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://rk.huixinmuqiang.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ko.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ry.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dp.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ah.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xs.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bn.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://er.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ba.bjjhwx.cn

[K07] 进制转换
来源：http://xp.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nu.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ne.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nf.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ta.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://at.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vb.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kw.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bw.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://ok.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://eq.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xu.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://hu.yuexingan06.cn

TS:   v8.serialize(obj)        // Node
来源：http://ew.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dr.yuexingan06.cn

Go:   encoding/gob
来源：http://ac.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://wc.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wi.wgjwhj.cn

================================================================================
来源：http://ne.9csxet.cn

L. 网络请求
来源：http://gx.chemitech.net.cn

================================================================================
来源：http://gs.asd995.cn

[L01] 发送 GET 请求
来源：http://zg.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jh.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wd.wgjwhj.cn

JS:   await fetch(url)
来源：http://jb.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://rh.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qu.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://qc.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kq.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pi.gzmigu.cn

[L02] 发送 POST JSON
来源：http://ej.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ts.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://me.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uu.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qk.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://if.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jz.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rd.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rr.hnjuh.cn

[L03] 设置自定义请求头
来源：http://mx.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ci.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hf.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nj.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ck.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yb.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ot.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nc.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yh.yuntaijiaju.cn

[L04] 设置超时
来源：http://ht.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://ca.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dw.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qa.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zm.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xo.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fm.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bw.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ay.9csxet.cn

[L05] 上传文件（multipart）
来源：http://ph.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wl.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tk.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uz.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sm.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vi.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kf.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://db.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://um.newstarts.cn

[L06] 解析响应为 JSON
来源：http://js.521024.cn

Py:   resp.json()
来源：http://dc.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://pq.gzmigu.cn

JS:   await resp.json()
来源：http://wd.hahajie.cn

TS:   await resp.json()
来源：http://zs.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rh.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://od.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://kf.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://we.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://oq.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tt.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rj.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://ea.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://ev.nicolike.cn

Java: resp.statusCode()
来源：http://ks.lnxyls.cn

Go:   resp.StatusCode
来源：http://sh.nicolike.cn

Ruby: resp.code.to_i
来源：http://hi.asd995.cn

C#:   (int)resp.StatusCode
来源：http://kf.hnjuh.cn

[L08] 并发请求多个地址
来源：http://we.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dn.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://nb.nszjky.cn


<!-- 参考信息 -->