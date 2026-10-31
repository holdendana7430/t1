代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rj.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://ud.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eq.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fi.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qn.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bh.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zq.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ql.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sv.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://at.hahajie.cn

[I04] 正则替换
来源：http://ls.yuexingan06.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cr.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://an.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ga.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pr.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uz.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zq.chemitech.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cw.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tx.panjiajie.cn

[I05] 按正则拆分
来源：http://ws.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tt.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kd.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://jk.hahajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://dl.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://fp.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eh.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hs.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pw.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qt.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zf.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fu.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jj.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lm.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ol.hahajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zi.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ta.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fp.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://mk.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://va.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xi.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pw.lnxyls.cn

TS:   /error/gim
来源：http://mv.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qu.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ua.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://tt.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nz.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://mk.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uh.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sb.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tb.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kd.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fq.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zh.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ng.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sa.shxzukj.cn

================================================================================
来源：http://th.yuexingan06.cn

J. 日期与时间
来源：http://ov.shxzskj.cn

================================================================================
来源：http://ph.jctech888.com.cn

[J01] 获取当前时间
来源：http://dm.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://em.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dz.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://gl.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://ie.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shxzukj.cn

Go:   time.Now()
来源：http://fo.haigaiapp.cn

Ruby: Time.now
来源：http://dw.newstarts.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ja.gzmigu.cn

[J02] 格式化输出
来源：http://qf.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vg.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fi.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pe.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://oz.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xi.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pa.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aj.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tp.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://na.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bd.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ku.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://pt.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://ja.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kq.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xd.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://hv.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mt.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://yj.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lh.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yp.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rh.lnxyls.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pt.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oh.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iy.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dr.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ja.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://vo.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://ng.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jb.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://no.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zv.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://iz.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dk.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://th.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jx.yuexingan06.cn

[J06] 计算两时间之差
来源：http://bt.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://md.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://ha.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iu.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ye.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lz.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://sp.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://wy.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://ub.chemitech.net.cn

[J07] 比较两个日期
来源：http://mv.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://xu.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wk.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://le.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mn.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zc.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lr.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lb.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://kb.nszjky.cn

[J08] 提取年月日与星期
来源：http://qc.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vx.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://by.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ul.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cp.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xj.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uc.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vh.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rs.hahajie.cn

[J09] 时区处理
来源：http://yk.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cq.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qf.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hq.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ir.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gg.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zo.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sl.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hk.521024.cn

[J10] 取今天 / 本月第一天
来源：http://al.gzmigu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vs.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rr.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zv.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qw.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qq.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mg.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yy.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jy.nicolike.cn

================================================================================
来源：http://qw.huixinmuqiang.cn

K. JSON 与序列化
来源：http://zf.panjiajie.cn

================================================================================
来源：http://xr.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://wb.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sp.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://md.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://wo.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://ul.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gl.asd995.cn

Go:   json.Marshal(obj)
来源：http://yl.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pa.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ed.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://he.muxihuayi.cn

Py:   json.loads(s)
来源：http://ov.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gx.nszjky.cn

JS:   JSON.parse(s)
来源：http://kn.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://dg.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://co.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://qm.521024.cn

Ruby: JSON.parse(s)
来源：http://ac.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dl.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://cl.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ue.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wv.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ct.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vp.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yf.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kx.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kz.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lj.huanxung.cn

[K04] 读取 JSON 文件
来源：http://jv.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lu.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ca.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ts.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pr.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gh.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yt.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qj.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kc.shtwfgs.cn

[K05] 深拷贝对象
来源：http://we.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://ti.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://qs.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://cq.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://uq.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xc.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vy.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://io.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yj.nszjky.cn

[K06] 解析 URL 查询串
来源：http://bj.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gj.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mo.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bk.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ip.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lx.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dl.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dz.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lf.szxytkj.cn

[K07] 进制转换
来源：http://ea.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zf.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bp.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wo.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ue.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tp.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mp.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nb.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qn.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ts.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://sm.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bp.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://dp.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://xw.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kp.newstarts.cn

Go:   encoding/gob
来源：http://gf.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://so.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ki.nicolike.cn

================================================================================
来源：http://uo.shtwfgs.cn

L. 网络请求
来源：http://fs.colortex.cn

================================================================================
来源：http://ym.szsharing.cn

[L01] 发送 GET 请求
来源：http://iq.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://la.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nh.nicolike.cn

JS:   await fetch(url)
来源：http://qz.szsharing.cn

TS:   await fetch(url)
来源：http://nf.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qu.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://be.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nn.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ah.521024.cn

[L02] 发送 POST JSON
来源：http://sm.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ub.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qz.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kv.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sm.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pm.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rl.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sv.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bi.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://rj.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yr.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mu.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pm.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tw.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fi.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rc.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oz.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yn.shxzskj.cn

[L04] 设置超时
来源：http://xx.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://gr.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sd.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mg.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://om.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lq.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bd.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dt.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ur.521024.cn

[L05] 上传文件（multipart）
来源：http://vy.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jx.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zy.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aw.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aq.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kt.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xj.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zo.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cy.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://ua.asd995.cn

Py:   resp.json()
来源：http://tv.nszjky.cn

PHP:  json_decode($body, true);
来源：http://bo.hahajie.cn

JS:   await resp.json()
来源：http://ka.nszjky.cn

TS:   await resp.json()
来源：http://mk.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ia.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vw.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://sr.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yo.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://bw.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wc.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ct.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://cf.colortex.cn

TS:   resp.ok;  resp.status
来源：http://ia.yuexingan06.cn

Java: resp.statusCode()
来源：http://or.chemitech.net.cn

Go:   resp.StatusCode
来源：http://cb.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://qc.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://et.szxytkj.cn

[L08] 并发请求多个地址
来源：http://xy.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zf.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://ny.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ya.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wt.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dl.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vz.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ki.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gp.huanxung.cn

================================================================================
来源：http://uz.521024.cn

M. 命令行 / 进程 / 环境
来源：http://dj.gzmigu.cn


<!-- 参考信息 -->