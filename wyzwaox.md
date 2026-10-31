代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://qu.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rw.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://cp.chemitech.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://iq.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://lh.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://df.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zw.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yx.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cq.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uv.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uv.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://om.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ex.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pg.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cv.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cq.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hh.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://gm.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fh.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://da.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ji.panjiajie.cn

TS:   /error/gim
来源：http://tn.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eo.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oc.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://mk.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mo.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://qq.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dw.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wc.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kk.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kv.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gu.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ij.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pg.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vr.szxytkj.cn

================================================================================
来源：http://wv.colortex.cn

J. 日期与时间
来源：http://jk.9csxet.cn

================================================================================
来源：http://bd.bookmarksfly.cn

[J01] 获取当前时间
来源：http://ef.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ge.jctech888.com.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xt.lnxyls.cn

JS:   new Date();  Date.now()
来源：http://sg.9csxet.cn

TS:   new Date();  Date.now()
来源：http://kt.chemitech.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jc.521024.cn

Go:   time.Now()
来源：http://nq.nicolike.cn

Ruby: Time.now
来源：http://fx.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ba.521024.cn

[J02] 格式化输出
来源：http://fi.muxihuayi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vf.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dp.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ix.wgjwhj.cn

TS:   d.toISOString()
来源：http://sx.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mn.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ct.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://de.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lv.asd995.cn

[J03] 字符串解析为日期
来源：http://kn.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uv.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://de.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://ul.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://ho.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cn.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mb.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://yi.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mz.asd995.cn

[J04] 时间戳与日期互转
来源：http://fz.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hr.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hh.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fz.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lo.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yq.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wr.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://os.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vw.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://bs.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://um.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gn.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ff.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jw.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://fw.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fo.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://tg.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pa.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://gv.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://jj.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://by.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hk.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sz.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vl.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://rr.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://we.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://tl.shtwfgs.cn

[J07] 比较两个日期
来源：http://qa.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://jv.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yi.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yq.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nx.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ib.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tl.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://wg.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://zw.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rd.bookmarksfly.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vr.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wv.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gv.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://md.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gt.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zp.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hx.bookmarksfly.cn

[J09] 时区处理
来源：http://cc.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hg.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kc.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fg.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://po.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fo.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ce.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hx.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gq.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://nc.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lv.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sf.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bs.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dl.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lv.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yb.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fj.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tw.521024.cn

================================================================================
来源：http://yv.szxytkj.cn

K. JSON 与序列化
来源：http://tp.gzmigu.cn

================================================================================
来源：http://la.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://bc.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zy.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vo.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://dg.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://wj.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oy.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://cd.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sh.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nf.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://qu.9csxet.cn

Py:   json.loads(s)
来源：http://cl.huixiangedu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mp.gzmigu.cn

JS:   JSON.parse(s)
来源：http://zh.9csxet.cn

TS:   JSON.parse(s)
来源：http://mv.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gb.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://xm.colortex.cn

Ruby: JSON.parse(s)
来源：http://my.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pl.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://uc.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gs.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bt.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://or.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gt.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bj.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rw.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vk.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jm.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://av.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gn.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://om.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qh.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oo.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lq.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dp.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://je.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hn.wgjwhj.cn

[K05] 深拷贝对象
来源：http://jy.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://wo.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://up.shxzskj.cn

JS:   structuredClone(obj)
来源：http://or.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://ig.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mf.hnjuh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://br.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kc.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rv.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://vi.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://la.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ya.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ik.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hk.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ec.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hl.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jk.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://al.jctech888.com.cn

[K07] 进制转换
来源：http://uh.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fk.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qp.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ol.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uu.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kk.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://io.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mz.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zc.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://gn.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://wb.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sa.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://sv.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://xe.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vv.wgjwhj.cn

Go:   encoding/gob
来源：http://ty.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://hw.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pg.jctech888.com.cn

================================================================================
来源：http://bf.gzmigu.cn

L. 网络请求
来源：http://bh.521024.cn

================================================================================
来源：http://ju.huixinmuqiang.cn

[L01] 发送 GET 请求
来源：http://yg.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://co.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lc.newstarts.cn

JS:   await fetch(url)
来源：http://df.muxihuayi.cn

TS:   await fetch(url)
来源：http://az.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aa.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://fx.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mg.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gp.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://wh.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kp.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://od.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tc.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iq.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yh.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bm.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rq.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ln.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://nz.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cp.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://te.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fi.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pg.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bj.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gc.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oi.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nj.huanxung.cn

[L04] 设置超时
来源：http://ln.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://mw.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ro.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ka.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ao.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tp.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zr.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mq.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uy.hahajie.cn

[L05] 上传文件（multipart）
来源：http://hs.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ld.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tt.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qu.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hj.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ey.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wb.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vq.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://em.newstarts.cn

[L06] 解析响应为 JSON
来源：http://te.bjjhwx.cn

Py:   resp.json()
来源：http://bo.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://gw.yuexingan06.cn

JS:   await resp.json()
来源：http://at.9csxet.cn

TS:   await resp.json()
来源：http://oy.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://id.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hu.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://kr.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wq.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://ca.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qo.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aj.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://sw.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://zf.panjiajie.cn

Java: resp.statusCode()
来源：http://vo.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://oc.szsharing.cn

Ruby: resp.code.to_i
来源：http://fo.asd995.cn

C#:   (int)resp.StatusCode
来源：http://gx.huanxung.cn

[L08] 并发请求多个地址
来源：http://xs.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tr.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://jf.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://st.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bu.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zv.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ww.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fc.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vr.haigaiapp.cn

================================================================================
来源：http://wm.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://mf.shxzukj.cn

================================================================================
来源：http://eh.lnxyls.cn

[M01] 读取命令行参数
来源：http://kx.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://xy.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://lp.hahajie.cn

JS:   process.argv.slice(2)
来源：http://uj.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://zw.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://ke.haigaiapp.cn

Go:   os.Args[1:]
来源：http://ko.haigaiapp.cn

Ruby: ARGV
来源：http://mj.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://cg.asd995.cn

[M02] 读取环境变量
来源：http://iv.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://tq.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fq.nicolike.cn

JS:   process.env.HOME
来源：http://gw.wgjwhj.cn

TS:   process.env.HOME
来源：http://mm.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://rn.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://th.colortex.cn

Ruby: ENV["HOME"]
来源：http://vg.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wi.chemitech.net.cn

[M03] 执行外部命令
来源：http://zy.huixiangedu.cn


<!-- 参考信息 -->