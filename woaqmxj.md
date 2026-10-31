代发 wailian999

TS:   s.match(/\d+/g)
来源：http://nf.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ha.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yi.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://yq.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vc.huixiangedu.cn

[I03] 提取捕获分组
来源：http://sg.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sc.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://os.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://si.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://is.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wg.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hj.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sv.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oa.yuntaijiaju.cn

[I04] 正则替换
来源：http://ay.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zz.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mc.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cs.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sp.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://as.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rw.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ol.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nx.yuexingan06.cn

[I05] 按正则拆分
来源：http://sl.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://of.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kk.colortex.cn

JS:   s.split(/\s*,\s*/)
来源：http://nx.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://kh.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://rq.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ru.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ik.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nw.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ff.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rc.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tn.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zb.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ls.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dz.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iq.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qr.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tl.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://ft.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pr.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hd.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ez.wgjwhj.cn

TS:   /error/gim
来源：http://nv.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jt.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pf.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://yy.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qz.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://oj.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pd.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ls.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ib.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ux.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xj.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://th.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xr.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rs.szsharing.cn

================================================================================
来源：http://qs.jctech888.com.cn

J. 日期与时间
来源：http://tm.chemitech.net.cn

================================================================================
来源：http://nz.haigaiapp.cn

[J01] 获取当前时间
来源：http://my.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hu.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ud.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://yw.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://ye.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ec.haigaiapp.cn

Go:   time.Now()
来源：http://dv.9csxet.cn

Ruby: Time.now
来源：http://uw.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mu.wgjwhj.cn

[J02] 格式化输出
来源：http://qt.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yd.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ci.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ph.nicolike.cn

TS:   d.toISOString()
来源：http://nt.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yh.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lp.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tt.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://za.lnxyls.cn

[J03] 字符串解析为日期
来源：http://hy.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ck.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qn.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://fj.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://ly.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vn.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yl.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://xc.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://va.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://bl.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wl.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bh.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ah.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tw.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://of.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nd.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lt.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nm.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://sg.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://mr.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ie.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ws.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hw.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://qi.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iv.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://ej.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ys.szxytkj.cn

[J06] 计算两时间之差
来源：http://ij.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://mi.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://mu.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mo.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nz.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nz.521024.cn

Go:   end.Sub(start).Hours()
来源：http://jt.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://ld.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://vy.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://gc.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://ab.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jv.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bw.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hv.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fe.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mc.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ib.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://az.nicolike.cn

[J08] 提取年月日与星期
来源：http://nm.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eg.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rx.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sq.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://in.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lk.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gj.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dd.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sl.9csxet.cn

[J09] 时区处理
来源：http://wz.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wk.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jc.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://en.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kc.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://am.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wl.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wh.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ll.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://xd.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cb.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fj.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yv.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fv.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xn.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yk.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pd.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hu.huixinmuqiang.cn

================================================================================
来源：http://di.bjjhwx.cn

K. JSON 与序列化
来源：http://mm.nszjky.cn

================================================================================
来源：http://ho.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://uw.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wk.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ub.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://xg.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://bc.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sv.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://az.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://iq.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cd.hahajie.cn

[K02] JSON 字符串转对象
来源：http://ld.panjiajie.cn

Py:   json.loads(s)
来源：http://mb.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dc.hnjuh.cn

JS:   JSON.parse(s)
来源：http://xo.panjiajie.cn

TS:   JSON.parse(s)
来源：http://qr.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yt.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://bt.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://ma.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lg.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://zt.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ux.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sb.jianghongdianzi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ab.szxytkj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cz.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tw.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xv.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dq.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ph.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://by.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ke.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wh.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ck.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rd.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tm.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mx.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dh.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wr.yuexingan06.cn

[K05] 深拷贝对象
来源：http://kj.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://wf.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://fo.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://dw.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://wl.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ob.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xw.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gm.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dm.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://mf.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uo.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dq.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ix.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jn.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vl.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mf.huixiangedu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vf.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kq.newstarts.cn

[K07] 进制转换
来源：http://gj.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yr.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sd.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ui.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ij.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uw.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ty.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yh.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://or.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://cu.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://au.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uf.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://zr.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://iu.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yn.shxzukj.cn

Go:   encoding/gob
来源：http://lu.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://hw.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kh.bjjhwx.cn

================================================================================
来源：http://wm.colortex.cn

L. 网络请求
来源：http://da.9csxet.cn

================================================================================
来源：http://ft.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://oe.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://il.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lh.huanxung.cn

JS:   await fetch(url)
来源：http://aa.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://pz.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vb.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://ej.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lg.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nl.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://oh.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tc.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uu.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vv.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://me.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vn.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ux.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iu.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vi.nszjky.cn

[L03] 设置自定义请求头
来源：http://iy.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lo.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wy.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vq.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ab.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wr.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nv.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xm.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zy.muxihuayi.cn

[L04] 设置超时
来源：http://ra.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://fq.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xg.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xn.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eh.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://be.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ee.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kd.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gg.nszjky.cn

[L05] 上传文件（multipart）
来源：http://hk.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fo.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://an.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ag.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pv.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ir.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tr.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oz.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sd.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://ds.lnxyls.cn

Py:   resp.json()
来源：http://kh.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://cc.shtwfgs.cn

JS:   await resp.json()
来源：http://rd.chemitech.net.cn

TS:   await resp.json()
来源：http://qg.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sj.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jd.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://dy.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jc.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://ij.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://il.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gi.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://od.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://ac.colortex.cn

Java: resp.statusCode()
来源：http://zg.nszjky.cn

Go:   resp.StatusCode
来源：http://zd.hahajie.cn

Ruby: resp.code.to_i
来源：http://hl.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://mm.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://hm.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dt.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://sz.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jz.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qn.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rm.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ud.wgjwhj.cn


<!-- 参考信息 -->