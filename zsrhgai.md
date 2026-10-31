代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://rc.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vx.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://th.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://xe.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://ej.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ic.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qy.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qq.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://we.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vb.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://if.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dc.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pg.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sy.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zj.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zj.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sc.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://uk.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yz.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lr.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://op.huanxung.cn

TS:   /error/gim
来源：http://on.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dq.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://um.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://bk.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oa.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://qn.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wi.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qm.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hq.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fi.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uf.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xv.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ol.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kl.jctech888.com.cn

================================================================================
来源：http://xv.muxihuayi.cn

J. 日期与时间
来源：http://mh.521024.cn

================================================================================
来源：http://rf.nszjky.cn

[J01] 获取当前时间
来源：http://ho.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hw.jctech888.com.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iv.hahajie.cn

JS:   new Date();  Date.now()
来源：http://ba.szsharing.cn

TS:   new Date();  Date.now()
来源：http://bv.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yu.nicolike.cn

Go:   time.Now()
来源：http://jw.huixiangedu.cn

Ruby: Time.now
来源：http://gg.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bg.gzmigu.cn

[J02] 格式化输出
来源：http://tk.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ba.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jy.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://an.shxzukj.cn

TS:   d.toISOString()
来源：http://kw.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tp.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xr.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bv.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://db.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://tm.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eq.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ka.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://qb.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://zo.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ti.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rt.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://lw.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aq.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://kx.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iz.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mv.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bt.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ka.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wi.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bc.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oj.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uf.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://jl.wgjwhj.cn

Py:   now + timedelta(days=7)
来源：http://oo.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zn.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tq.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pb.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://nr.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uz.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://yn.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dh.huixiangedu.cn

[J06] 计算两时间之差
来源：http://dz.521024.cn

Py:   (end - start).total_seconds()
来源：http://ww.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://ua.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ic.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ld.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dp.521024.cn

Go:   end.Sub(start).Hours()
来源：http://pz.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://gh.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://xu.panjiajie.cn

[J07] 比较两个日期
来源：http://xv.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://tg.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vv.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xt.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fr.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jy.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xx.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mu.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://kt.panjiajie.cn

[J08] 提取年月日与星期
来源：http://qh.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zd.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fe.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mi.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vf.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cx.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yr.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dw.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dm.muxihuayi.cn

[J09] 时区处理
来源：http://lm.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gt.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hg.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zw.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gk.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ub.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yi.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vk.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://on.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://ov.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tx.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://il.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yo.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zk.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zf.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ci.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://as.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ek.lnxyls.cn

================================================================================
来源：http://bm.hahajie.cn

K. JSON 与序列化
来源：http://wz.yuntaijiaju.cn

================================================================================
来源：http://wy.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://wj.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ao.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uo.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://nl.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://uw.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rl.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://cm.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jl.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ou.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://ca.wgjwhj.cn

Py:   json.loads(s)
来源：http://jf.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jw.hahajie.cn

JS:   JSON.parse(s)
来源：http://vb.asd995.cn

TS:   JSON.parse(s)
来源：http://cg.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dz.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://te.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://mn.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nn.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://bc.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oh.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sb.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://du.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ih.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bg.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cl.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pn.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wg.hahajie.cn

[K04] 读取 JSON 文件
来源：http://kc.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ka.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pd.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zg.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ha.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pj.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bf.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zs.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oo.bjjhwx.cn

[K05] 深拷贝对象
来源：http://qu.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://fp.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://xv.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://pe.nszjky.cn

TS:   structuredClone(obj)
来源：http://sp.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wo.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ld.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cf.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oe.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://oc.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yq.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zo.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xh.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ze.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fv.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zn.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vj.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tl.panjiajie.cn

[K07] 进制转换
来源：http://pa.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pu.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://co.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vz.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ba.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vh.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qx.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://su.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ll.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://ra.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://wh.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sc.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://xd.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://ex.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cl.panjiajie.cn

Go:   encoding/gob
来源：http://tf.bookmarksfly.cn

Ruby: Marshal.dump(obj)
来源：http://ow.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dg.wgjwhj.cn

================================================================================
来源：http://zs.shtwfgs.cn

L. 网络请求
来源：http://qh.hnjuh.cn

================================================================================
来源：http://cl.szsharing.cn

[L01] 发送 GET 请求
来源：http://el.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://es.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ol.9csxet.cn

JS:   await fetch(url)
来源：http://vf.lnxyls.cn

TS:   await fetch(url)
来源：http://ni.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sb.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://qu.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wv.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ey.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://cu.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://la.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lo.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dp.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://af.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ll.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://du.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://op.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dp.colortex.cn

[L03] 设置自定义请求头
来源：http://yz.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jg.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rs.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bs.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vc.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://js.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gh.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dc.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mi.newstarts.cn

[L04] 设置超时
来源：http://zy.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://yp.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cz.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://js.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jf.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ph.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hk.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eq.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wa.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://bg.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pe.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://za.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zt.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dn.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gy.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://su.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mq.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mz.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://eu.bjjhwx.cn

Py:   resp.json()
来源：http://xl.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://im.szxytkj.cn

JS:   await resp.json()
来源：http://rh.gzmigu.cn

TS:   await resp.json()
来源：http://uf.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ro.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://do.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://fh.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pl.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://bz.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pm.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://az.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://bf.asd995.cn

TS:   resp.ok;  resp.status
来源：http://ry.muxihuayi.cn

Java: resp.statusCode()
来源：http://cd.panjiajie.cn

Go:   resp.StatusCode
来源：http://ol.shxzukj.cn

Ruby: resp.code.to_i
来源：http://yh.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://pr.newstarts.cn

[L08] 并发请求多个地址
来源：http://pg.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ai.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://mq.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kw.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yh.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kw.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dd.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rs.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ep.yuntaijiaju.cn

================================================================================
来源：http://nl.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://hn.newstarts.cn

================================================================================
来源：http://tc.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://fi.colortex.cn

Py:   sys.argv[1:]
来源：http://oi.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://qr.nszjky.cn

JS:   process.argv.slice(2)
来源：http://rr.szsharing.cn

TS:   process.argv.slice(2)
来源：http://wi.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://un.yuexingan06.cn

Go:   os.Args[1:]
来源：http://rw.huixinmuqiang.cn

Ruby: ARGV
来源：http://ap.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://vc.nicolike.cn

[M02] 读取环境变量
来源：http://ng.colortex.cn

Py:   os.environ.get("HOME")
来源：http://ba.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xz.lnxyls.cn

JS:   process.env.HOME
来源：http://rb.9csxet.cn

TS:   process.env.HOME
来源：http://gn.shxzukj.cn

Java: System.getenv("HOME")
来源：http://uf.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xb.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://qp.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gw.panjiajie.cn

[M03] 执行外部命令
来源：http://xm.bookmarksfly.cn


<!-- 参考信息 -->