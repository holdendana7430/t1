代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fw.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pb.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ml.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nz.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cx.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qk.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wu.newstarts.cn

[I05] 按正则拆分
来源：http://bc.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cc.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yv.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://mj.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://qn.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://lc.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zc.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ph.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kg.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mv.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ca.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bp.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zm.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dv.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ab.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ao.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zd.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yk.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://jq.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ri.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pw.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dg.wgjwhj.cn

TS:   /error/gim
来源：http://jm.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pn.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cv.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://ka.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://og.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://ip.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ed.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hb.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cl.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qi.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gf.nszjky.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cg.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oi.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ou.huixiangedu.cn

================================================================================
来源：http://hp.chemitech.net.cn

J. 日期与时间
来源：http://va.nicolike.cn

================================================================================
来源：http://aw.muxihuayi.cn

[J01] 获取当前时间
来源：http://oi.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zu.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://as.colortex.cn

JS:   new Date();  Date.now()
来源：http://hf.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://wr.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ge.asd995.cn

Go:   time.Now()
来源：http://bk.lnxyls.cn

Ruby: Time.now
来源：http://xi.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ye.hnjuh.cn

[J02] 格式化输出
来源：http://ze.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gw.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mg.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lu.shxzskj.cn

TS:   d.toISOString()
来源：http://rp.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iq.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pi.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jd.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qn.asd995.cn

[J03] 字符串解析为日期
来源：http://tf.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oj.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rx.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://ag.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://ll.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hb.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://em.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://we.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vo.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://jo.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://im.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pa.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wk.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yw.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uk.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://of.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jn.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ii.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://ty.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://vl.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nj.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zm.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ab.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://xc.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dg.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://oa.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rf.shxzskj.cn

[J06] 计算两时间之差
来源：http://ko.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://ww.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://db.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ax.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qb.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zs.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://wc.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://eg.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://sn.nicolike.cn

[J07] 比较两个日期
来源：http://od.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://sb.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ku.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://te.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pq.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jx.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://in.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mm.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ke.panjiajie.cn

[J08] 提取年月日与星期
来源：http://ue.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ma.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oh.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hp.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bi.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ii.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sv.huixiangedu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oe.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tx.asd995.cn

[J09] 时区处理
来源：http://kh.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://js.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://al.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gs.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dl.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pu.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lx.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mn.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ss.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://si.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rd.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gz.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ax.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fi.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pc.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ih.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wx.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tb.lnxyls.cn

================================================================================
来源：http://uj.hnjuh.cn

K. JSON 与序列化
来源：http://jn.jctech888.com.cn

================================================================================
来源：http://dw.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://eo.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ob.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yq.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://nu.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://pd.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jx.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://gh.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qk.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gq.9csxet.cn

[K02] JSON 字符串转对象
来源：http://cj.lnxyls.cn

Py:   json.loads(s)
来源：http://bm.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yd.gzmigu.cn

JS:   JSON.parse(s)
来源：http://jm.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://yw.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cx.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://ok.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://ht.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qt.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://bu.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yp.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vc.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mj.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ba.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ay.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://su.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gf.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hu.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://lb.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eb.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jf.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gh.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jp.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fo.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sp.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lw.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fy.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://vm.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://yc.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://we.szsharing.cn

JS:   structuredClone(obj)
来源：http://mh.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://ui.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zv.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bm.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tl.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ii.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://vd.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gp.huixinmuqiang.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qd.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://io.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jy.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ha.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ys.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://np.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ka.nszjky.cn

[K07] 进制转换
来源：http://lo.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uf.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kb.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cn.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nf.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tx.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ze.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kt.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bz.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://ha.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://so.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rh.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://es.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://lk.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nw.lnxyls.cn

Go:   encoding/gob
来源：http://sl.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://ve.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ca.asd995.cn

================================================================================
来源：http://vi.gzmigu.cn

L. 网络请求
来源：http://bv.chemitech.net.cn

================================================================================
来源：http://hp.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://mp.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kc.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bm.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://lc.haigaiapp.cn

TS:   await fetch(url)
来源：http://pf.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xq.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://dl.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://av.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ch.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://yv.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uc.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://da.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pq.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mu.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fr.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ma.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://og.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vi.panjiajie.cn

[L03] 设置自定义请求头
来源：http://iw.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xr.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wh.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hj.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dk.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ob.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kn.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nm.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sb.colortex.cn

[L04] 设置超时
来源：http://wj.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://aa.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wa.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bb.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qe.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gw.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wi.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ob.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mn.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://om.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nm.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xv.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fj.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cy.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sb.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ow.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wx.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mm.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://yk.wgjwhj.cn

Py:   resp.json()
来源：http://ea.9csxet.cn

PHP:  json_decode($body, true);
来源：http://jw.gzmigu.cn

JS:   await resp.json()
来源：http://nk.yuntaijiaju.cn

TS:   await resp.json()
来源：http://cw.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gz.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ny.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://lf.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hl.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://wp.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ph.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yz.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://zs.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://hj.gzmigu.cn

Java: resp.statusCode()
来源：http://jy.gzmigu.cn

Go:   resp.StatusCode
来源：http://gn.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://gh.colortex.cn

C#:   (int)resp.StatusCode
来源：http://fm.hahajie.cn

[L08] 并发请求多个地址
来源：http://iv.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ea.521024.cn

PHP:  curl_multi_init() 系列
来源：http://cg.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tl.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zv.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kk.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zg.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mk.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jj.huixinmuqiang.cn

================================================================================
来源：http://ez.521024.cn

M. 命令行 / 进程 / 环境
来源：http://cv.colortex.cn

================================================================================
来源：http://df.chemitech.net.cn

[M01] 读取命令行参数
来源：http://ni.nszjky.cn

Py:   sys.argv[1:]
来源：http://ps.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://wa.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://vq.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://ky.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://iq.jctech888.com.cn

Go:   os.Args[1:]
来源：http://fa.lnxyls.cn

Ruby: ARGV
来源：http://so.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://py.shtwfgs.cn

[M02] 读取环境变量
来源：http://kq.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://ru.bjjhwx.cn


<!-- 参考信息 -->