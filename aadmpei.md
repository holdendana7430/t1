代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://ji.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qy.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xw.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ak.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uc.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dh.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bg.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jn.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lc.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yb.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wm.haigaiapp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ys.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ni.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://ij.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yt.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kj.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xz.gzmigu.cn

TS:   /error/gim
来源：http://bi.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jt.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://st.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://fe.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nb.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://un.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ys.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dw.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lh.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xi.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oz.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pw.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yz.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tk.nicolike.cn

================================================================================
来源：http://ah.chemitech.net.cn

J. 日期与时间
来源：http://cv.shtwfgs.cn

================================================================================
来源：http://ur.hahajie.cn

[J01] 获取当前时间
来源：http://xb.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dx.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zo.nszjky.cn

JS:   new Date();  Date.now()
来源：http://ah.521024.cn

TS:   new Date();  Date.now()
来源：http://nu.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fj.jctech888.com.cn

Go:   time.Now()
来源：http://ys.wgjwhj.cn

Ruby: Time.now
来源：http://cg.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yq.asd995.cn

[J02] 格式化输出
来源：http://sn.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ug.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ka.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://es.asd995.cn

TS:   d.toISOString()
来源：http://ue.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sa.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pw.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xg.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tq.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://pw.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gn.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://po.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://uu.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://ye.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zs.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xa.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://nj.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fp.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://yj.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uq.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zm.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fk.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kx.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rs.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tf.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sn.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://du.521024.cn

[J05] 时间加减（加 7 天）
来源：http://qz.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://jh.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zj.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://he.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ia.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://oz.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ww.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://fv.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pm.huanxung.cn

[J06] 计算两时间之差
来源：http://pv.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://az.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://fy.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pp.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sr.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qs.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://mr.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://xj.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://yo.521024.cn

[J07] 比较两个日期
来源：http://ym.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://ze.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oo.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fq.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mh.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ni.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hw.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vc.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://xg.lnxyls.cn

[J08] 提取年月日与星期
来源：http://mm.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gv.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wd.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://up.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pc.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vi.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zh.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://os.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fr.jianghongdianzi.cn

[J09] 时区处理
来源：http://ln.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nr.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ih.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uv.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gz.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uy.nicolike.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jk.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kv.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rj.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://wo.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lf.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yq.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yc.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://td.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pe.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kq.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qr.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fd.asd995.cn

================================================================================
来源：http://cs.shtwfgs.cn

K. JSON 与序列化
来源：http://td.szsharing.cn

================================================================================
来源：http://mk.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://ts.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uw.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fm.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://ew.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://wp.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gu.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://mv.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oj.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xp.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://mf.521024.cn

Py:   json.loads(s)
来源：http://rm.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oj.hnjuh.cn

JS:   JSON.parse(s)
来源：http://ze.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://lk.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jt.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://ud.nicolike.cn

Ruby: JSON.parse(s)
来源：http://ep.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://la.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://ke.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nw.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ey.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cf.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kg.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wp.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nq.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oa.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://am.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://qr.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ld.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://in.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iy.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wn.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hb.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wd.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ya.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://py.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://nv.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://yx.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://yn.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://sz.gzmigu.cn

TS:   structuredClone(obj)
来源：http://pq.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ec.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gf.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qb.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bb.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://cy.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qy.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://er.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://as.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lg.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pv.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cq.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jv.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jg.muxihuayi.cn

[K07] 进制转换
来源：http://vl.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yn.chemitech.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rx.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sp.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kw.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gi.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pm.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://en.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rb.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://ci.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://bj.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vw.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://vm.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://ro.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eh.wgjwhj.cn

Go:   encoding/gob
来源：http://te.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://ng.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bn.yuntaijiaju.cn

================================================================================
来源：http://mv.haigaiapp.cn

L. 网络请求
来源：http://ca.shxzskj.cn

================================================================================
来源：http://sj.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://es.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://np.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://re.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://hm.huixiangedu.cn

TS:   await fetch(url)
来源：http://iz.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gj.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://kv.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://of.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lh.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://ua.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://be.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vx.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vg.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://re.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fy.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jv.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://te.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jd.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://rn.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cs.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lx.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yc.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uv.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wo.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eo.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vy.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zk.huixinmuqiang.cn

[L04] 设置超时
来源：http://yh.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://fg.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oh.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sv.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vj.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fi.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fm.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ru.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ss.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://sm.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://id.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pk.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lj.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kw.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tk.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qg.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jg.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jh.nicolike.cn

[L06] 解析响应为 JSON
来源：http://eu.haigaiapp.cn

Py:   resp.json()
来源：http://pm.huanxung.cn

PHP:  json_decode($body, true);
来源：http://pa.asd995.cn

JS:   await resp.json()
来源：http://ew.shxzukj.cn

TS:   await resp.json()
来源：http://oi.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dd.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bo.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://an.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qe.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://cz.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jz.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nm.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://dt.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://ez.9csxet.cn

Java: resp.statusCode()
来源：http://bu.newstarts.cn

Go:   resp.StatusCode
来源：http://hi.9csxet.cn

Ruby: resp.code.to_i
来源：http://aq.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://wl.9csxet.cn

[L08] 并发请求多个地址
来源：http://mt.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tq.huixinmuqiang.cn

PHP:  curl_multi_init() 系列
来源：http://if.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pw.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ze.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://it.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lr.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xq.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pj.lnxyls.cn

================================================================================
来源：http://xa.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://ar.asd995.cn

================================================================================
来源：http://mt.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://rc.nszjky.cn

Py:   sys.argv[1:]
来源：http://hu.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://ey.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://yh.nszjky.cn

TS:   process.argv.slice(2)
来源：http://hg.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://bp.lnxyls.cn

Go:   os.Args[1:]
来源：http://vc.haigaiapp.cn

Ruby: ARGV
来源：http://vb.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://lv.shtwfgs.cn

[M02] 读取环境变量
来源：http://zj.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://mx.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gh.yuexingan06.cn

JS:   process.env.HOME
来源：http://pp.lnxyls.cn

TS:   process.env.HOME
来源：http://tf.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://lo.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qk.nszjky.cn

Ruby: ENV["HOME"]
来源：http://fl.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ez.colortex.cn

[M03] 执行外部命令
来源：http://eg.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hu.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wg.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://eg.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qk.newstarts.cn


<!-- 参考信息 -->