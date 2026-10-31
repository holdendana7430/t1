代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ld.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jc.szsharing.cn

[I04] 正则替换
来源：http://lf.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zs.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://if.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ce.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ku.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xw.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gt.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sg.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yx.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://wh.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cd.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ng.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://jz.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://cz.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://jj.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lp.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tc.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nq.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ai.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://be.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rw.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ev.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vj.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jr.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mz.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tk.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hk.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://xd.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kg.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ce.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://on.haigaiapp.cn

TS:   /error/gim
来源：http://qw.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lw.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ei.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://ol.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pr.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://fj.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cm.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jo.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qg.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://br.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qe.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mk.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://no.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mw.muxihuayi.cn

================================================================================
来源：http://ps.jianghongdianzi.cn

J. 日期与时间
来源：http://yq.9csxet.cn

================================================================================
来源：http://al.nszjky.cn

[J01] 获取当前时间
来源：http://cp.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rk.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kv.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://ty.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://iv.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ls.bjjhwx.cn

Go:   time.Now()
来源：http://ea.lnxyls.cn

Ruby: Time.now
来源：http://wr.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mf.jianghongdianzi.cn

[J02] 格式化输出
来源：http://xx.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wp.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vb.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ba.szxytkj.cn

TS:   d.toISOString()
来源：http://ck.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nr.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wl.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rf.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://io.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://nw.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oe.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eu.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://zq.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://ej.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nu.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yo.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://jc.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ew.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://uv.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bu.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nq.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oa.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mk.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tg.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://of.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gz.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nd.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://bd.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://gh.jianghongdianzi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ha.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qx.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qm.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://bg.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jk.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://zk.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fm.jctech888.com.cn

[J06] 计算两时间之差
来源：http://nz.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://qu.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://fh.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xa.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eo.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hd.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://ga.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://dz.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://sm.shtwfgs.cn

[J07] 比较两个日期
来源：http://qf.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://fm.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uj.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ls.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ou.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uk.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yz.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://eo.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://ku.hahajie.cn

[J08] 提取年月日与星期
来源：http://qb.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vy.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eb.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lt.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ay.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hn.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rp.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://os.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://op.chemitech.net.cn

[J09] 时区处理
来源：http://oy.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://te.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jl.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ei.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nb.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://so.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aa.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://im.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hw.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://gb.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tu.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yt.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ek.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hq.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pd.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ah.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ar.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vi.shtwfgs.cn

================================================================================
来源：http://ve.newstarts.cn

K. JSON 与序列化
来源：http://yi.asd995.cn

================================================================================
来源：http://hw.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://za.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aw.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dj.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://rr.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://iu.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ny.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://ma.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mo.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dq.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://xj.huixiangedu.cn

Py:   json.loads(s)
来源：http://sg.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sr.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://jx.521024.cn

TS:   JSON.parse(s)
来源：http://tu.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://re.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://dv.nszjky.cn

Ruby: JSON.parse(s)
来源：http://vv.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zq.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://pq.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bd.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qo.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hp.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://le.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dr.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wt.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tr.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zk.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://ic.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ea.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bv.szsharing.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fq.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cu.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yk.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sv.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nq.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rj.hnjuh.cn

[K05] 深拷贝对象
来源：http://gy.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://dm.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://ut.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://te.hnjuh.cn

TS:   structuredClone(obj)
来源：http://nc.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nh.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qe.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vn.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bv.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://oh.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lw.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jx.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ha.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ny.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ig.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cd.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dr.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jy.jianghongdianzi.cn

[K07] 进制转换
来源：http://ud.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wk.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cn.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vh.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jb.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ta.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ac.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qu.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ac.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://xq.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://fq.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://aw.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://am.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://im.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qe.jctech888.com.cn

Go:   encoding/gob
来源：http://vu.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://nw.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mz.colortex.cn

================================================================================
来源：http://ak.bookmarksfly.cn

L. 网络请求
来源：http://lf.gzmigu.cn

================================================================================
来源：http://eb.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://hn.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dd.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ha.newstarts.cn

JS:   await fetch(url)
来源：http://ag.newstarts.cn

TS:   await fetch(url)
来源：http://ll.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hx.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://bd.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dw.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hn.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://fw.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qv.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jm.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://km.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://km.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tr.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eh.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fc.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://le.lnxyls.cn

[L03] 设置自定义请求头
来源：http://ax.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ze.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://er.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ah.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sy.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ih.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ds.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ii.bjjhwx.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kv.huixiangedu.cn

[L04] 设置超时
来源：http://ux.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://el.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yv.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wt.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jq.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ax.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ax.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ib.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://go.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://yo.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ye.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ih.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sy.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://is.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ly.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wj.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qc.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pg.nszjky.cn

[L06] 解析响应为 JSON
来源：http://mt.gzmigu.cn

Py:   resp.json()
来源：http://fc.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://mj.yuexingan06.cn

JS:   await resp.json()
来源：http://cl.chemitech.net.cn

TS:   await resp.json()
来源：http://nx.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://je.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ca.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://tm.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fy.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://wa.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://je.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rz.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://mq.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://qs.chemitech.net.cn

Java: resp.statusCode()
来源：http://qq.hahajie.cn

Go:   resp.StatusCode
来源：http://ic.gzmigu.cn

Ruby: resp.code.to_i
来源：http://ic.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://wd.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://gx.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ef.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://jc.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pa.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rp.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ex.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dh.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zy.hahajie.cn

================================================================================
来源：http://di.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://pj.gzmigu.cn

================================================================================
来源：http://oi.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://ng.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://ho.szsharing.cn

PHP:  $argv;  $argc;
来源：http://up.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://rj.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://ht.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://ud.jctech888.com.cn

Go:   os.Args[1:]
来源：http://eg.yuexingan06.cn


<!-- 参考信息 -->