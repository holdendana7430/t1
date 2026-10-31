代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://co.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wz.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://ys.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bd.haigaiapp.cn

[I02] 提取所有匹配
来源：http://uh.szsharing.cn

Py:   re.findall(r"\d+", s)
来源：http://pv.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ue.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mu.lnxyls.cn

TS:   s.match(/\d+/g)
来源：http://oo.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xl.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wy.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://jg.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pp.521024.cn

[I03] 提取捕获分组
来源：http://lo.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://in.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://um.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cm.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rd.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vr.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kt.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bv.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ky.bjjhwx.cn

[I04] 正则替换
来源：http://fa.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xq.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ut.521024.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cw.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bo.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pi.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vi.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uj.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gn.huanxung.cn

[I05] 按正则拆分
来源：http://dv.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xg.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sy.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://ag.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://ja.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://fp.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cc.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cl.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kp.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ft.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cv.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wq.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iz.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ye.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ie.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hv.haigaiapp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dm.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ai.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://nj.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nw.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://si.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pm.521024.cn

TS:   /error/gim
来源：http://wv.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zt.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oj.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://mf.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ds.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://yf.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wu.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wq.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kx.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hk.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gg.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qc.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ph.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tx.haigaiapp.cn

================================================================================
来源：http://nr.huixiangedu.cn

J. 日期与时间
来源：http://hd.colortex.cn

================================================================================
来源：http://bc.wgjwhj.cn

[J01] 获取当前时间
来源：http://iq.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://aw.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vd.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://xg.huanxung.cn

TS:   new Date();  Date.now()
来源：http://ih.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bm.szxytkj.cn

Go:   time.Now()
来源：http://as.panjiajie.cn

Ruby: Time.now
来源：http://np.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lx.shxzskj.cn

[J02] 格式化输出
来源：http://lz.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yo.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wt.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ou.nszjky.cn

TS:   d.toISOString()
来源：http://ln.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vt.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hu.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kj.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qh.gzmigu.cn

[J03] 字符串解析为日期
来源：http://fi.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ei.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rd.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://or.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://fg.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ob.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jz.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://ws.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jl.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://dr.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ym.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hy.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ji.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dw.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xm.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ac.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qc.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ck.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://lv.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://jc.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://eh.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oy.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fa.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://ge.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ly.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://hs.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qe.szsharing.cn

[J06] 计算两时间之差
来源：http://xl.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://um.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://lo.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pm.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hd.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ix.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://af.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://tf.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://ug.521024.cn

[J07] 比较两个日期
来源：http://zv.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://gm.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cu.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gq.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://oe.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fv.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iq.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zp.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://yl.hnjuh.cn

[J08] 提取年月日与星期
来源：http://is.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bj.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rw.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pa.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ad.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rl.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zh.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://en.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fr.jctech888.com.cn

[J09] 时区处理
来源：http://ht.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://av.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ed.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rq.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kr.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xm.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ly.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ul.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ym.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://sm.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vk.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zu.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yw.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ul.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xz.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ws.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tz.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wc.shtwfgs.cn

================================================================================
来源：http://ml.521024.cn

K. JSON 与序列化
来源：http://zh.bookmarksfly.cn

================================================================================
来源：http://hi.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://vl.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xq.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ma.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://ce.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://in.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mj.nszjky.cn

Go:   json.Marshal(obj)
来源：http://ft.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ax.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oy.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://hy.chemitech.net.cn

Py:   json.loads(s)
来源：http://pz.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tc.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://ph.newstarts.cn

TS:   JSON.parse(s)
来源：http://km.gzmigu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pe.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://oo.asd995.cn

Ruby: JSON.parse(s)
来源：http://ay.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lz.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://jb.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ju.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ot.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ld.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jy.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tg.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ct.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://er.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kw.9csxet.cn

[K04] 读取 JSON 文件
来源：http://et.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yf.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://au.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xf.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cz.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yd.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vg.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sz.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://px.huanxung.cn

[K05] 深拷贝对象
来源：http://bm.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://vg.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://pv.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://iq.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://ve.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://np.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ke.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wh.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gd.nicolike.cn

[K06] 解析 URL 查询串
来源：http://ie.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://di.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rg.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://md.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://as.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yy.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vt.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ks.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sw.9csxet.cn

[K07] 进制转换
来源：http://dd.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qb.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://di.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ae.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zf.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qa.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://in.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rg.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bz.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://fc.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://cp.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dq.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://aa.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://rh.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://li.shxzskj.cn

Go:   encoding/gob
来源：http://eq.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://pu.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lq.hahajie.cn

================================================================================
来源：http://ck.521024.cn

L. 网络请求
来源：http://op.yuexingan06.cn

================================================================================
来源：http://cg.huanxung.cn

[L01] 发送 GET 请求
来源：http://bh.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dc.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ot.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://bj.wgjwhj.cn

TS:   await fetch(url)
来源：http://ll.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ll.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://du.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ya.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pl.asd995.cn

[L02] 发送 POST JSON
来源：http://ic.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zb.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://or.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kr.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kt.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://im.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hf.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tg.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iv.newstarts.cn

[L03] 设置自定义请求头
来源：http://qg.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lw.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pp.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ze.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://an.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kl.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uh.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oo.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yf.huixinmuqiang.cn

[L04] 设置超时
来源：http://jy.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://gu.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rl.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jt.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oo.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ye.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ry.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bo.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bx.szsharing.cn

[L05] 上传文件（multipart）
来源：http://vw.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://if.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://if.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qr.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ya.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vq.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nx.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nj.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pg.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://dy.nszjky.cn

Py:   resp.json()
来源：http://nb.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://cn.newstarts.cn

JS:   await resp.json()
来源：http://pv.lnxyls.cn

TS:   await resp.json()
来源：http://hu.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cv.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ut.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://nf.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gk.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://qy.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://os.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gf.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://xk.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://al.asd995.cn

Java: resp.statusCode()
来源：http://ce.hnjuh.cn

Go:   resp.StatusCode
来源：http://ch.gzmigu.cn

Ruby: resp.code.to_i
来源：http://ee.521024.cn


<!-- 参考信息 -->