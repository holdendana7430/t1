代发 wailian999

TS:   s.match(/\d+/g)
来源：http://xi.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://in.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bt.521024.cn

Ruby: s.scan(/\d+/)
来源：http://gx.bjjhwx.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fg.wgjwhj.cn

[I03] 提取捕获分组
来源：http://je.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vi.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wo.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lo.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xv.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kn.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dh.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hq.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tm.bjjhwx.cn

[I04] 正则替换
来源：http://dz.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vx.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tm.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lf.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wv.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yo.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sq.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ft.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pi.colortex.cn

[I05] 按正则拆分
来源：http://ll.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tn.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tx.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://xi.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://bt.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://hn.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aa.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tm.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ah.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pa.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ry.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ry.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hd.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dm.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xi.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ee.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yd.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hn.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://it.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cd.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bt.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zp.muxihuayi.cn

TS:   /error/gim
来源：http://ii.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zl.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fk.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://ey.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vr.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://jy.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qz.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vf.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://za.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ui.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pd.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zb.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://na.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tu.haigaiapp.cn

================================================================================
来源：http://qr.huanxung.cn

J. 日期与时间
来源：http://lg.jianghongdianzi.cn

================================================================================
来源：http://gm.nicolike.cn

[J01] 获取当前时间
来源：http://sw.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xs.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sc.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://qa.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://az.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ls.colortex.cn

Go:   time.Now()
来源：http://ie.hnjuh.cn

Ruby: Time.now
来源：http://di.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://en.shxzskj.cn

[J02] 格式化输出
来源：http://qw.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ok.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xo.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://on.9csxet.cn

TS:   d.toISOString()
来源：http://si.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tn.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oz.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uv.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ip.521024.cn

[J03] 字符串解析为日期
来源：http://pr.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fe.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zw.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://lh.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://yu.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tq.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://um.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://kr.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rv.huanxung.cn

[J04] 时间戳与日期互转
来源：http://nx.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ju.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fj.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rl.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fr.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vb.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qq.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jt.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lo.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://vs.521024.cn

Py:   now + timedelta(days=7)
来源：http://wl.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sf.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wx.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gi.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://zc.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://we.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://ga.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bc.9csxet.cn

[J06] 计算两时间之差
来源：http://yh.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://sa.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://ph.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kp.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pv.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fj.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://nh.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://pf.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://fz.chemitech.net.cn

[J07] 比较两个日期
来源：http://zw.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://at.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gg.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vh.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xs.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eh.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bf.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fs.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://mc.nszjky.cn

[J08] 提取年月日与星期
来源：http://bf.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yt.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mh.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://az.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wk.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zk.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ax.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xn.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hw.huixiangedu.cn

[J09] 时区处理
来源：http://km.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oe.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ga.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sh.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ry.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ht.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rm.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ga.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://su.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://qi.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wo.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vx.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tk.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://so.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mf.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fw.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uq.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ns.bookmarksfly.cn

================================================================================
来源：http://nn.jctech888.com.cn

K. JSON 与序列化
来源：http://dv.newstarts.cn

================================================================================
来源：http://ne.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://zw.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://og.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qs.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://fw.colortex.cn

TS:   JSON.stringify(obj)
来源：http://bi.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://md.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://tx.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sw.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yx.hahajie.cn

[K02] JSON 字符串转对象
来源：http://tk.panjiajie.cn

Py:   json.loads(s)
来源：http://oo.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wv.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://co.9csxet.cn

TS:   JSON.parse(s)
来源：http://xv.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nz.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://ys.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://gz.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://po.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ob.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xd.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qr.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bo.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lw.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gs.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hh.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wk.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qb.9csxet.cn

[K04] 读取 JSON 文件
来源：http://vs.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ug.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cz.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ad.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sq.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://np.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cq.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yx.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mg.newstarts.cn

[K05] 深拷贝对象
来源：http://pm.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://ur.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://oj.szsharing.cn

JS:   structuredClone(obj)
来源：http://ot.szsharing.cn

TS:   structuredClone(obj)
来源：http://pl.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gq.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qc.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pn.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sg.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://yr.huixinmuqiang.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ad.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oz.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qf.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cc.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://se.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ez.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rn.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yw.jianghongdianzi.cn

[K07] 进制转换
来源：http://xa.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://re.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://as.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hs.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kb.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mq.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://de.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bp.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wa.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://wc.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://kr.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://se.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://tj.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://aw.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nl.yuexingan06.cn

Go:   encoding/gob
来源：http://ov.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://nu.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iq.gzmigu.cn

================================================================================
来源：http://rz.newstarts.cn

L. 网络请求
来源：http://az.muxihuayi.cn

================================================================================
来源：http://xg.lnxyls.cn

[L01] 发送 GET 请求
来源：http://pg.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bf.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xg.gzmigu.cn

JS:   await fetch(url)
来源：http://oi.asd995.cn

TS:   await fetch(url)
来源：http://ms.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ka.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://mw.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lo.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xj.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://wr.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://js.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ne.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oe.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qb.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bz.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gj.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sp.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dx.panjiajie.cn

[L03] 设置自定义请求头
来源：http://lb.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qh.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ub.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eh.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rd.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ti.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uf.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fw.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kw.huanxung.cn

[L04] 设置超时
来源：http://km.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://jr.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vr.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dz.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ak.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gl.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pn.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yk.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jz.szsharing.cn

[L05] 上传文件（multipart）
来源：http://xd.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xc.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rq.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wt.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pz.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ia.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nh.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ne.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sh.9csxet.cn

[L06] 解析响应为 JSON
来源：http://uj.9csxet.cn

Py:   resp.json()
来源：http://hp.nicolike.cn

PHP:  json_decode($body, true);
来源：http://kg.huixinmuqiang.cn

JS:   await resp.json()
来源：http://kw.szsharing.cn

TS:   await resp.json()
来源：http://za.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kv.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lw.yuexingan06.cn

Ruby: JSON.parse(resp.body)
来源：http://ou.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fb.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://rj.newstarts.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://at.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vi.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://ak.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://zg.muxihuayi.cn

Java: resp.statusCode()
来源：http://dd.jctech888.com.cn

Go:   resp.StatusCode
来源：http://bf.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://jm.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://ai.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://aj.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sq.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://gd.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vt.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://et.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gr.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nl.wgjwhj.cn


<!-- 参考信息 -->