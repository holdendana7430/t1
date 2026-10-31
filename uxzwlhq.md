代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://fa.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gg.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lz.chemitech.net.cn

[I05] 按正则拆分
来源：http://kh.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qe.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ot.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://uz.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://yw.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://xr.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yi.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ex.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://if.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uq.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vb.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nd.hahajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cd.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ma.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xl.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qy.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://es.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wt.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://xo.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kk.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://la.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://om.9csxet.cn

TS:   /error/gim
来源：http://xg.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oa.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jm.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://ve.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ta.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://px.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://db.huixiangedu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lr.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uh.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eo.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ss.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fo.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xx.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tp.yuntaijiaju.cn

================================================================================
来源：http://wg.chemitech.net.cn

J. 日期与时间
来源：http://rq.szxytkj.cn

================================================================================
来源：http://ub.shtwfgs.cn

[J01] 获取当前时间
来源：http://ks.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xy.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mz.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://mp.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://df.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tw.lnxyls.cn

Go:   time.Now()
来源：http://tv.521024.cn

Ruby: Time.now
来源：http://uf.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lp.szsharing.cn

[J02] 格式化输出
来源：http://wy.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nn.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kr.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sy.shtwfgs.cn

TS:   d.toISOString()
来源：http://ae.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eo.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ek.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rs.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gz.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://dp.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://je.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tm.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://jx.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://wy.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zw.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ys.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://fr.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://og.hahajie.cn

[J04] 时间戳与日期互转
来源：http://fh.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cs.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://id.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ay.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yz.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ku.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xt.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vx.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hy.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://zw.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://xv.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lp.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tt.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zj.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://ub.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fi.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://kf.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ou.colortex.cn

[J06] 计算两时间之差
来源：http://yd.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://ts.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://ys.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sz.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bo.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hs.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://sw.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://jy.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://gn.chemitech.net.cn

[J07] 比较两个日期
来源：http://ay.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://vv.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eb.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pi.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vb.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gz.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jt.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gr.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://fa.9csxet.cn

[J08] 提取年月日与星期
来源：http://hr.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gh.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yi.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ez.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rq.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qd.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pb.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lu.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fc.newstarts.cn

[J09] 时区处理
来源：http://aj.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pg.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xl.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qr.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ri.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xc.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cq.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pn.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rb.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://iu.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://os.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://we.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yc.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wu.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wn.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bg.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gf.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uy.chemitech.net.cn

================================================================================
来源：http://rj.9csxet.cn

K. JSON 与序列化
来源：http://em.bjjhwx.cn

================================================================================
来源：http://vy.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://ft.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tj.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fk.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://hb.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://fr.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tr.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://yv.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fj.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://db.nszjky.cn

[K02] JSON 字符串转对象
来源：http://rs.nszjky.cn

Py:   json.loads(s)
来源：http://kh.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nx.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://rl.521024.cn

TS:   JSON.parse(s)
来源：http://ru.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wi.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://jx.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://du.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fe.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://dm.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://za.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nh.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fh.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ia.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://og.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ce.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wg.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qp.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://ru.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yo.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://be.szsharing.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vu.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hg.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zp.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fv.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yg.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dx.nicolike.cn

[K05] 深拷贝对象
来源：http://so.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://hq.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://zg.shxzukj.cn

JS:   structuredClone(obj)
来源：http://rg.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://su.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ez.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ps.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uf.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uv.nszjky.cn

[K06] 解析 URL 查询串
来源：http://my.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fw.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pd.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pz.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mr.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://io.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zu.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fa.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nx.yuexingan06.cn

[K07] 进制转换
来源：http://an.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ss.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mo.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fz.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mo.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pm.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wq.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qm.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zv.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://lu.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://lb.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xk.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://pg.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://bg.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gi.shtwfgs.cn

Go:   encoding/gob
来源：http://ch.521024.cn

Ruby: Marshal.dump(obj)
来源：http://cc.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ol.yuntaijiaju.cn

================================================================================
来源：http://pd.yuntaijiaju.cn

L. 网络请求
来源：http://bw.bjjhwx.cn

================================================================================
来源：http://ir.nicolike.cn

[L01] 发送 GET 请求
来源：http://lh.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://un.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://we.hnjuh.cn

JS:   await fetch(url)
来源：http://us.lnxyls.cn

TS:   await fetch(url)
来源：http://bw.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zx.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://qn.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gd.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nv.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://sd.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ox.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://la.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cg.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ko.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ym.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://es.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yg.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dv.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://xt.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qh.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yi.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ss.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ra.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nn.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rh.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ki.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fr.newstarts.cn

[L04] 设置超时
来源：http://po.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://io.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://te.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tz.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zw.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://at.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://so.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://px.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hh.szsharing.cn

[L05] 上传文件（multipart）
来源：http://zo.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xa.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kd.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://su.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rs.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rw.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vr.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pw.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://os.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://nw.nicolike.cn

Py:   resp.json()
来源：http://yq.newstarts.cn

PHP:  json_decode($body, true);
来源：http://vk.muxihuayi.cn

JS:   await resp.json()
来源：http://ej.jianghongdianzi.cn

TS:   await resp.json()
来源：http://yi.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ia.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hi.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://ey.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eg.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://vg.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://az.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jw.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://my.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://pz.gzmigu.cn

Java: resp.statusCode()
来源：http://sf.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://db.hahajie.cn

Ruby: resp.code.to_i
来源：http://wm.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://wl.szxytkj.cn

[L08] 并发请求多个地址
来源：http://iz.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ku.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://av.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gh.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ok.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ao.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ne.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kn.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mr.asd995.cn

================================================================================
来源：http://wa.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://qw.bjjhwx.cn

================================================================================
来源：http://no.yuexingan06.cn

[M01] 读取命令行参数
来源：http://gc.521024.cn

Py:   sys.argv[1:]
来源：http://av.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://yu.colortex.cn

JS:   process.argv.slice(2)
来源：http://vn.nicolike.cn

TS:   process.argv.slice(2)
来源：http://bc.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://xi.shtwfgs.cn

Go:   os.Args[1:]
来源：http://rx.lnxyls.cn

Ruby: ARGV
来源：http://tj.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://vf.yuexingan06.cn

[M02] 读取环境变量
来源：http://es.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://mv.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ot.hahajie.cn

JS:   process.env.HOME
来源：http://xo.hahajie.cn

TS:   process.env.HOME
来源：http://xf.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://vy.muxihuayi.cn


<!-- 参考信息 -->