代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://de.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://yv.hnjuh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tx.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nz.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eb.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kq.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rt.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pa.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ni.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rg.jianghongdianzi.cn

[I04] 正则替换
来源：http://ws.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hg.huanxung.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ne.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ke.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ir.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ne.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ex.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nj.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vu.bookmarksfly.cn

[I05] 按正则拆分
来源：http://by.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ug.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pf.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://in.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://ao.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://ld.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nu.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uh.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://np.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sg.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vl.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nc.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://db.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ws.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ft.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dm.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gs.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ab.521024.cn

[I07] 忽略大小写与多行模式
来源：http://ik.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ly.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bq.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ol.szxytkj.cn

TS:   /error/gim
来源：http://pa.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ri.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ek.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://ci.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ut.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://al.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xn.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ha.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fw.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://be.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://je.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://om.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xv.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mm.panjiajie.cn

================================================================================
来源：http://ur.bookmarksfly.cn

J. 日期与时间
来源：http://ur.bjjhwx.cn

================================================================================
来源：http://xr.panjiajie.cn

[J01] 获取当前时间
来源：http://ix.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tb.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ny.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://xd.nszjky.cn

TS:   new Date();  Date.now()
来源：http://nm.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bn.shxzskj.cn

Go:   time.Now()
来源：http://gx.shtwfgs.cn

Ruby: Time.now
来源：http://jl.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lr.chemitech.net.cn

[J02] 格式化输出
来源：http://ie.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hm.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ns.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ey.bookmarksfly.cn

TS:   d.toISOString()
来源：http://kt.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://su.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sw.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cu.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qx.panjiajie.cn

[J03] 字符串解析为日期
来源：http://ts.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fp.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wz.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://pe.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://gu.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://np.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nf.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://ob.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yf.9csxet.cn

[J04] 时间戳与日期互转
来源：http://ah.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vu.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xi.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://af.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tc.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ah.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lu.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qr.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dv.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://lp.colortex.cn

Py:   now + timedelta(days=7)
来源：http://uj.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bl.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sl.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fn.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://sz.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cw.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://ps.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jb.colortex.cn

[J06] 计算两时间之差
来源：http://py.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://fv.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://sy.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jn.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eb.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sn.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://fv.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://eu.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://tg.szxytkj.cn

[J07] 比较两个日期
来源：http://ck.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://fx.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ll.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kh.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uo.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ga.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://it.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://ze.hnjuh.cn

[J08] 提取年月日与星期
来源：http://od.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qs.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ax.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ho.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qz.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ai.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ye.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uc.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ix.9csxet.cn

[J09] 时区处理
来源：http://wo.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ww.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jc.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ub.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://du.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kh.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bu.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dj.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pl.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://cx.gzmigu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ol.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ae.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gs.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ab.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ky.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ak.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nv.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sb.9csxet.cn

================================================================================
来源：http://nz.panjiajie.cn

K. JSON 与序列化
来源：http://ls.huixinmuqiang.cn

================================================================================
来源：http://qf.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://ix.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oh.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ph.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://oe.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://zw.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://py.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://xa.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ec.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sy.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://nc.panjiajie.cn

Py:   json.loads(s)
来源：http://rg.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lv.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://al.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://ry.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eu.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://wc.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://ik.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wm.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://nz.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xq.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ji.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pk.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vh.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zz.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ps.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wm.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kg.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://az.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nm.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://un.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pn.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xk.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zn.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wk.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yh.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nd.shxzskj.cn

[K05] 深拷贝对象
来源：http://io.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://wj.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://uv.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://mx.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://sb.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bz.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wz.9csxet.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ki.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://up.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://zy.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bv.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ps.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ch.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://va.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cr.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zp.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jk.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://go.jianghongdianzi.cn

[K07] 进制转换
来源：http://ww.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hm.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://py.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bp.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cu.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qn.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vx.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sc.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://un.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://bg.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://fc.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nz.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://hw.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://yc.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sh.shtwfgs.cn

Go:   encoding/gob
来源：http://dv.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://hs.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qd.szxytkj.cn

================================================================================
来源：http://nn.haigaiapp.cn

L. 网络请求
来源：http://rz.szsharing.cn

================================================================================
来源：http://rp.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://ra.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bg.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ji.haigaiapp.cn

JS:   await fetch(url)
来源：http://eb.lnxyls.cn

TS:   await fetch(url)
来源：http://gu.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zo.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://hs.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kq.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://na.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://vj.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xa.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ld.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sa.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nm.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hv.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bv.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gn.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kj.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://xz.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mc.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oi.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mu.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kf.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://te.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ap.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jx.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hi.shxzukj.cn

[L04] 设置超时
来源：http://cj.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://oo.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jq.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hn.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mq.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tu.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pf.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ug.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gw.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://uy.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ib.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dh.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jt.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dt.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uw.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nh.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lv.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gi.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://qp.bookmarksfly.cn

Py:   resp.json()
来源：http://yl.nszjky.cn

PHP:  json_decode($body, true);
来源：http://nh.asd995.cn

JS:   await resp.json()
来源：http://rc.jctech888.com.cn

TS:   await resp.json()
来源：http://by.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qf.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sq.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://ne.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ed.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://ur.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ct.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://di.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://fj.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://ws.colortex.cn

Java: resp.statusCode()
来源：http://ye.szxytkj.cn

Go:   resp.StatusCode
来源：http://qf.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://ok.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://sd.nicolike.cn

[L08] 并发请求多个地址
来源：http://zj.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eo.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://th.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qx.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ov.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://to.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jw.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fp.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hi.shxzskj.cn

================================================================================
来源：http://jn.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://os.huixiangedu.cn


<!-- 参考信息 -->