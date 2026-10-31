代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zk.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dk.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yw.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sy.huanxung.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dc.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gl.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jw.szsharing.cn

[I05] 按正则拆分
来源：http://ia.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kk.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tm.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://tu.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://ac.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://dn.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lo.nicolike.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zo.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ud.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ar.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kf.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qu.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iw.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cd.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://et.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lm.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gv.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qr.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://cv.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qw.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ze.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qu.huixiangedu.cn

TS:   /error/gim
来源：http://tv.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tl.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wc.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://fz.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uv.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://st.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sd.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ui.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mq.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://va.huanxung.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ai.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wb.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rx.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pd.newstarts.cn

================================================================================
来源：http://qf.bjjhwx.cn

J. 日期与时间
来源：http://bh.szsharing.cn

================================================================================
来源：http://yw.jctech888.com.cn

[J01] 获取当前时间
来源：http://nj.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mk.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zg.9csxet.cn

JS:   new Date();  Date.now()
来源：http://og.nicolike.cn

TS:   new Date();  Date.now()
来源：http://rl.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://so.shxzukj.cn

Go:   time.Now()
来源：http://pj.521024.cn

Ruby: Time.now
来源：http://rz.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://he.shxzukj.cn

[J02] 格式化输出
来源：http://we.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jz.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://le.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jt.asd995.cn

TS:   d.toISOString()
来源：http://jg.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ab.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kv.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xl.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bi.521024.cn

[J03] 字符串解析为日期
来源：http://gv.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ms.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tm.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://mt.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://ql.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pg.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uq.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://lx.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pq.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://cf.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uw.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uj.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://of.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sz.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sh.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bp.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://so.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://at.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://yh.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://uy.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://da.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fu.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vi.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://li.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jt.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://yj.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bf.bjjhwx.cn

[J06] 计算两时间之差
来源：http://ya.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://zk.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://ag.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rl.hnjuh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mk.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ss.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://ac.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://fa.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://rt.newstarts.cn

[J07] 比较两个日期
来源：http://ym.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://cu.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://re.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ig.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cp.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kr.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jy.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zb.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://iz.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://ak.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sg.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ye.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ao.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hf.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yn.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gb.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ru.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jb.hnjuh.cn

[J09] 时区处理
来源：http://so.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bz.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pb.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lc.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ks.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uf.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ie.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ob.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ke.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://ts.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jm.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ri.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tp.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fr.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yy.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pt.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dh.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yh.nszjky.cn

================================================================================
来源：http://es.haigaiapp.cn

K. JSON 与序列化
来源：http://zb.hnjuh.cn

================================================================================
来源：http://fu.521024.cn

[K01] 对象转 JSON 字符串
来源：http://ba.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://de.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fn.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://ws.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://bl.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cz.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://tk.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ts.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ur.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://pk.hahajie.cn

Py:   json.loads(s)
来源：http://qp.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xw.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://fe.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://le.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://os.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://ia.521024.cn

Ruby: JSON.parse(s)
来源：http://uv.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ou.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://lx.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rp.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ev.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rr.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://eh.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://os.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rt.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ci.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fm.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://nz.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oz.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lv.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://et.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xt.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vf.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vw.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rz.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jl.shtwfgs.cn

[K05] 深拷贝对象
来源：http://vy.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://vp.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://xb.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://mf.nicolike.cn

TS:   structuredClone(obj)
来源：http://uf.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sc.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sa.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ge.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ar.asd995.cn

[K06] 解析 URL 查询串
来源：http://ld.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fh.huixinmuqiang.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rq.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mv.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vz.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mp.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dz.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rb.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lk.colortex.cn

[K07] 进制转换
来源：http://kn.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dk.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eg.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xe.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ez.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ei.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qx.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ps.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lz.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://rb.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://ov.haigaiapp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fr.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://un.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://sj.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zv.nszjky.cn

Go:   encoding/gob
来源：http://bs.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://vd.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rl.huixinmuqiang.cn

================================================================================
来源：http://gc.wgjwhj.cn

L. 网络请求
来源：http://xh.szxytkj.cn

================================================================================
来源：http://ba.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://jr.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oy.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zn.szsharing.cn

JS:   await fetch(url)
来源：http://dx.nszjky.cn

TS:   await fetch(url)
来源：http://gv.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aj.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://bt.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://it.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bg.colortex.cn

[L02] 发送 POST JSON
来源：http://mf.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ec.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tp.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oj.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lu.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oi.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://du.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yp.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fk.colortex.cn

[L03] 设置自定义请求头
来源：http://uw.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qs.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sz.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://if.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fc.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nq.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qh.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nw.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tm.521024.cn

[L04] 设置超时
来源：http://zr.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://zj.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rc.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uk.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ju.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ff.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ec.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qd.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ax.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://wi.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wi.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tb.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cl.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qi.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zh.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fh.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gr.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://im.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://wk.wgjwhj.cn

Py:   resp.json()
来源：http://ji.hahajie.cn

PHP:  json_decode($body, true);
来源：http://bd.huanxung.cn

JS:   await resp.json()
来源：http://ah.muxihuayi.cn

TS:   await resp.json()
来源：http://vd.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xk.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tq.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://fc.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fl.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://dp.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uy.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ni.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://sw.521024.cn

TS:   resp.ok;  resp.status
来源：http://ub.nszjky.cn

Java: resp.statusCode()
来源：http://ja.lnxyls.cn

Go:   resp.StatusCode
来源：http://po.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://bh.colortex.cn

C#:   (int)resp.StatusCode
来源：http://jg.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://oh.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pn.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://hf.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bm.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ba.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ds.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bq.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sv.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pi.szxytkj.cn

================================================================================
来源：http://hq.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://zm.wgjwhj.cn

================================================================================
来源：http://qr.szxytkj.cn

[M01] 读取命令行参数
来源：http://gg.colortex.cn

Py:   sys.argv[1:]
来源：http://nz.newstarts.cn

PHP:  $argv;  $argc;
来源：http://cr.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://ud.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://or.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://jk.nicolike.cn

Go:   os.Args[1:]
来源：http://nl.szxytkj.cn

Ruby: ARGV
来源：http://zg.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://je.haigaiapp.cn

[M02] 读取环境变量
来源：http://aq.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://wz.nszjky.cn


<!-- 参考信息 -->