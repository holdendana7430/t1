代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vu.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mo.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://db.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vm.yuntaijiaju.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://je.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zx.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mh.haigaiapp.cn

[I05] 按正则拆分
来源：http://hg.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gq.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tk.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://vl.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://gm.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://jx.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oc.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jh.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zm.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qi.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wt.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bl.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ss.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bi.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fm.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rs.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pv.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ea.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://ys.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wr.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://of.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zz.hahajie.cn

TS:   /error/gim
来源：http://tf.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zg.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qn.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://at.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mi.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://wd.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ga.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wt.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yq.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nk.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rs.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nc.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bd.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cn.asd995.cn

================================================================================
来源：http://ft.bookmarksfly.cn

J. 日期与时间
来源：http://uu.szxytkj.cn

================================================================================
来源：http://ff.nicolike.cn

[J01] 获取当前时间
来源：http://yl.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jj.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pa.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://ws.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://or.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sk.asd995.cn

Go:   time.Now()
来源：http://zl.huanxung.cn

Ruby: Time.now
来源：http://nx.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yy.newstarts.cn

[J02] 格式化输出
来源：http://rd.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bw.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ol.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qe.521024.cn

TS:   d.toISOString()
来源：http://dd.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xp.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jp.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jv.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yr.9csxet.cn

[J03] 字符串解析为日期
来源：http://gw.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hl.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iz.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://jh.asd995.cn

TS:   new Date("2024-01-02")
来源：http://ta.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ni.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cd.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://rn.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jx.hahajie.cn

[J04] 时间戳与日期互转
来源：http://kw.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sp.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jy.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://la.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ud.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qt.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://be.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ue.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mt.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://az.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://ig.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iw.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rs.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ed.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://zt.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yr.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://xh.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mo.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://yw.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://lz.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://wp.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sc.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://iv.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mh.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://ay.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://cm.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://ji.nicolike.cn

[J07] 比较两个日期
来源：http://kh.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://wc.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hd.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zw.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yy.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mv.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mb.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cx.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://zb.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://ma.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bc.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hp.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jv.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iz.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pq.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zm.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://la.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wv.colortex.cn

[J09] 时区处理
来源：http://le.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vi.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uf.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ms.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sp.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pt.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://go.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qr.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bb.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://td.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ed.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qu.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yl.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://df.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hi.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ve.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dz.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kw.haigaiapp.cn

================================================================================
来源：http://vy.bookmarksfly.cn

K. JSON 与序列化
来源：http://tk.newstarts.cn

================================================================================
来源：http://sd.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://cn.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lc.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://th.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://uy.521024.cn

TS:   JSON.stringify(obj)
来源：http://ep.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mj.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://fd.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pc.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dx.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://jq.shxzukj.cn

Py:   json.loads(s)
来源：http://wb.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qx.colortex.cn

JS:   JSON.parse(s)
来源：http://dz.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://it.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ha.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://lh.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://ac.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aw.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ul.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ja.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yf.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://il.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pc.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qb.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ch.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zf.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vn.9csxet.cn

[K04] 读取 JSON 文件
来源：http://yb.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yf.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ag.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zg.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ge.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xt.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ms.shtwfgs.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ib.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uj.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://rh.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://yc.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://pc.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://fk.asd995.cn

TS:   structuredClone(obj)
来源：http://if.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sm.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://br.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rt.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ml.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://rw.huixinmuqiang.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zi.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xf.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xd.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iq.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ix.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rg.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ij.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mp.huixinmuqiang.cn

[K07] 进制转换
来源：http://gt.panjiajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hh.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://em.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kl.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://di.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rx.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kx.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vq.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rv.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ks.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://jc.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qe.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ge.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://vc.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tm.jianghongdianzi.cn

Go:   encoding/gob
来源：http://nm.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://om.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qr.muxihuayi.cn

================================================================================
来源：http://go.haigaiapp.cn

L. 网络请求
来源：http://xo.bookmarksfly.cn

================================================================================
来源：http://mo.hahajie.cn

[L01] 发送 GET 请求
来源：http://hv.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ov.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yy.shtwfgs.cn

JS:   await fetch(url)
来源：http://yl.huixiangedu.cn

TS:   await fetch(url)
来源：http://om.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qh.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://kn.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ez.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ck.newstarts.cn

[L02] 发送 POST JSON
来源：http://qa.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nv.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ir.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wn.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ho.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fz.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ul.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wb.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gv.colortex.cn

[L03] 设置自定义请求头
来源：http://qc.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jp.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://le.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nk.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://um.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://et.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://py.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fq.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zs.hahajie.cn

[L04] 设置超时
来源：http://yw.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://cd.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yf.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uz.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://da.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ib.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ey.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qz.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ju.hahajie.cn

[L05] 上传文件（multipart）
来源：http://fb.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sk.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://at.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yg.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nn.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tb.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dr.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jv.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rk.nszjky.cn

[L06] 解析响应为 JSON
来源：http://uy.huixiangedu.cn

Py:   resp.json()
来源：http://wz.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://ii.nszjky.cn

JS:   await resp.json()
来源：http://xb.asd995.cn

TS:   await resp.json()
来源：http://ea.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ty.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cs.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://yp.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rx.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://kj.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gb.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ud.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://px.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://tv.haigaiapp.cn

Java: resp.statusCode()
来源：http://gb.wgjwhj.cn

Go:   resp.StatusCode
来源：http://bv.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://gs.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://yx.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://tq.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zr.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://ex.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jj.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mp.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ck.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rc.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zs.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ch.521024.cn

================================================================================
来源：http://yw.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://ks.nicolike.cn

================================================================================
来源：http://sj.asd995.cn

[M01] 读取命令行参数
来源：http://vz.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://qn.nszjky.cn

PHP:  $argv;  $argc;
来源：http://ko.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://bc.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://hj.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://fn.haigaiapp.cn

Go:   os.Args[1:]
来源：http://ol.asd995.cn

Ruby: ARGV
来源：http://dz.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://vl.newstarts.cn

[M02] 读取环境变量
来源：http://vl.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://hy.muxihuayi.cn


<!-- 参考信息 -->