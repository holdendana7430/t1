代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sc.huanxung.cn

[I03] 提取捕获分组
来源：http://ec.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jj.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vh.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vp.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kt.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tj.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vh.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eo.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uz.wgjwhj.cn

[I04] 正则替换
来源：http://ng.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lk.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jk.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sn.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mn.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sz.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ki.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jd.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zk.newstarts.cn

[I05] 按正则拆分
来源：http://yt.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fk.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ye.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ox.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://nt.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://it.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rd.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mb.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://af.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://df.asd995.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zc.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ov.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qx.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nv.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wq.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pc.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rf.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zm.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://jp.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tv.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://az.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zy.panjiajie.cn

TS:   /error/gim
来源：http://ym.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ni.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zw.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://hl.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hi.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://bi.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pz.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cv.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wb.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zd.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ww.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tg.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kg.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://br.nszjky.cn

================================================================================
来源：http://de.szsharing.cn

J. 日期与时间
来源：http://pv.newstarts.cn

================================================================================
来源：http://yg.colortex.cn

[J01] 获取当前时间
来源：http://rf.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gt.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gm.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://ja.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://ri.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yn.nicolike.cn

Go:   time.Now()
来源：http://hj.nicolike.cn

Ruby: Time.now
来源：http://wy.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lu.hahajie.cn

[J02] 格式化输出
来源：http://oh.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oa.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fn.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jt.jctech888.com.cn

TS:   d.toISOString()
来源：http://ys.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sd.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://la.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wt.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hu.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://kh.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sh.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fq.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://cj.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://rq.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pq.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bu.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://is.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xo.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://gs.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pi.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sp.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sl.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xx.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gg.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cp.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://up.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://em.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://lf.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://dd.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gh.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yd.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xl.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://qu.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://re.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://hq.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kl.shxzukj.cn

[J06] 计算两时间之差
来源：http://vm.521024.cn

Py:   (end - start).total_seconds()
来源：http://el.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://nw.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://av.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zu.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ft.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://so.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://qr.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://hz.szxytkj.cn

[J07] 比较两个日期
来源：http://ry.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://mj.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://py.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ij.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kk.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cg.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bn.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cg.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://ar.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://ko.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ca.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ha.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://su.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ab.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ri.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sf.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qu.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vi.9csxet.cn

[J09] 时区处理
来源：http://ed.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pg.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zq.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xi.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rn.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zo.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pj.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uu.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lv.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://uv.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vu.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yo.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ci.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zx.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qx.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mr.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ws.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bu.bookmarksfly.cn

================================================================================
来源：http://zx.newstarts.cn

K. JSON 与序列化
来源：http://ut.haigaiapp.cn

================================================================================
来源：http://jx.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://rj.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://td.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lc.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://bq.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://vf.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hs.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://kx.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ye.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ri.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://im.wgjwhj.cn

Py:   json.loads(s)
来源：http://kh.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lz.gzmigu.cn

JS:   JSON.parse(s)
来源：http://ys.hnjuh.cn

TS:   JSON.parse(s)
来源：http://mc.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dp.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://tq.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://mk.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ax.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://ce.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lx.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bg.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oe.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kv.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oy.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ro.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://iy.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jk.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://zy.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fl.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hs.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ad.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qy.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vp.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://re.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kj.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://io.szxytkj.cn

[K05] 深拷贝对象
来源：http://wa.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://ub.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://ez.lnxyls.cn

JS:   structuredClone(obj)
来源：http://pv.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://mw.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ns.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uh.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lc.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sq.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://ap.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oa.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tc.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ws.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lg.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fq.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://so.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pb.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nt.huanxung.cn

[K07] 进制转换
来源：http://vc.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cz.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ti.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mn.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qv.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xu.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ey.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://om.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qf.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://rc.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://sp.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zp.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://ec.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://ph.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yk.9csxet.cn

Go:   encoding/gob
来源：http://ss.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://dt.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kt.haigaiapp.cn

================================================================================
来源：http://qj.gzmigu.cn

L. 网络请求
来源：http://jv.9csxet.cn

================================================================================
来源：http://jm.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://tj.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ru.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ct.huanxung.cn

JS:   await fetch(url)
来源：http://zz.9csxet.cn

TS:   await fetch(url)
来源：http://re.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dc.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://ye.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://td.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eh.newstarts.cn

[L02] 发送 POST JSON
来源：http://vy.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wj.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bn.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bg.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wr.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ju.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ti.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ul.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ad.huanxung.cn

[L03] 设置自定义请求头
来源：http://vi.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ww.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tt.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cz.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bs.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kd.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wv.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hi.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qo.huanxung.cn

[L04] 设置超时
来源：http://fl.jianghongdianzi.cn

Py:   requests.get(url, timeout=5)
来源：http://he.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cm.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sh.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bx.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://te.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ge.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lb.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ax.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://xn.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pc.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ss.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rs.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uh.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qq.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gg.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xg.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gu.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://yt.panjiajie.cn

Py:   resp.json()
来源：http://bu.nszjky.cn

PHP:  json_decode($body, true);
来源：http://qt.wgjwhj.cn

JS:   await resp.json()
来源：http://qb.hnjuh.cn

TS:   await resp.json()
来源：http://ln.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lu.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gm.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://wm.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ib.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://ut.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vn.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wp.asd995.cn

JS:   resp.ok;  resp.status
来源：http://oh.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://no.hahajie.cn

Java: resp.statusCode()
来源：http://xq.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://fh.szsharing.cn

Ruby: resp.code.to_i
来源：http://vm.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://pg.hnjuh.cn

[L08] 并发请求多个地址
来源：http://ig.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mu.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://fl.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://te.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qd.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://te.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vq.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dk.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pf.muxihuayi.cn

================================================================================
来源：http://bf.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://pf.shxzskj.cn


<!-- 参考信息 -->