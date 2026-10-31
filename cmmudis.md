代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ub.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ed.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://by.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jt.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qp.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dc.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vz.huixiangedu.cn

[I05] 按正则拆分
来源：http://hz.9csxet.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ot.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bf.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://lw.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://ik.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://if.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yt.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qg.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aa.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eq.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ew.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hb.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cy.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ew.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mm.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yw.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ya.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zz.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://dn.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ke.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rh.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fb.jianghongdianzi.cn

TS:   /error/gim
来源：http://hg.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dn.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ck.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://tr.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://at.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://ov.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pm.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yo.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hy.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tp.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ii.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tv.szxytkj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vz.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gy.wgjwhj.cn

================================================================================
来源：http://gk.huixiangedu.cn

J. 日期与时间
来源：http://gn.521024.cn

================================================================================
来源：http://hp.szsharing.cn

[J01] 获取当前时间
来源：http://hm.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qt.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pn.lnxyls.cn

JS:   new Date();  Date.now()
来源：http://va.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://fo.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gu.lnxyls.cn

Go:   time.Now()
来源：http://tt.jctech888.com.cn

Ruby: Time.now
来源：http://mo.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zj.gzmigu.cn

[J02] 格式化输出
来源：http://cw.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ki.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ni.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nk.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://ji.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xr.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lu.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://te.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tf.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://pv.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lq.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gc.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://qj.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://ld.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ga.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cq.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://jo.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lh.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://ct.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gx.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qk.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gx.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sv.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dl.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xt.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rs.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ab.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://fe.colortex.cn

Py:   now + timedelta(days=7)
来源：http://li.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bz.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nd.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kh.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://ku.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xw.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://bq.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jb.jctech888.com.cn

[J06] 计算两时间之差
来源：http://bj.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://vj.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://ol.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bk.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ld.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wv.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://jf.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://yu.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://jh.wgjwhj.cn

[J07] 比较两个日期
来源：http://bo.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://pq.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ll.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://it.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xf.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pb.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ov.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sb.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://qc.nszjky.cn

[J08] 提取年月日与星期
来源：http://vq.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://em.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vj.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nv.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://am.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bc.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nt.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bv.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fo.huixiangedu.cn

[J09] 时区处理
来源：http://cf.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ab.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vi.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lw.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ro.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uh.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ql.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kv.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://op.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://eb.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gs.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lt.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ck.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://as.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ci.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xt.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sb.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pp.wgjwhj.cn

================================================================================
来源：http://jr.huixinmuqiang.cn

K. JSON 与序列化
来源：http://dn.hnjuh.cn

================================================================================
来源：http://yp.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://yx.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://me.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rn.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://os.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://me.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://by.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://kp.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qm.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jk.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://im.huixiangedu.cn

Py:   json.loads(s)
来源：http://jd.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vf.nszjky.cn

JS:   JSON.parse(s)
来源：http://eq.9csxet.cn

TS:   JSON.parse(s)
来源：http://tc.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wk.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://sg.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://tl.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qy.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://hc.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ad.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nw.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://od.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ow.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pm.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://io.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gn.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qo.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://ls.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dk.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sa.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bp.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mp.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pt.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oi.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ib.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jb.gzmigu.cn

[K05] 深拷贝对象
来源：http://lh.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://ti.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://aq.521024.cn

JS:   structuredClone(obj)
来源：http://yy.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://zo.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sc.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qo.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fq.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zy.nicolike.cn

[K06] 解析 URL 查询串
来源：http://ge.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oj.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nx.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://du.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ml.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sm.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nf.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fg.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wj.szxytkj.cn

[K07] 进制转换
来源：http://gd.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sq.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ce.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jq.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hx.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wv.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nu.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jh.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yq.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://xy.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://ao.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ia.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://sa.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://rk.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hl.panjiajie.cn

Go:   encoding/gob
来源：http://qj.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://bd.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://is.huanxung.cn

================================================================================
来源：http://yv.9csxet.cn

L. 网络请求
来源：http://se.shtwfgs.cn

================================================================================
来源：http://ys.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://hh.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jl.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xn.haigaiapp.cn

JS:   await fetch(url)
来源：http://qa.bjjhwx.cn

TS:   await fetch(url)
来源：http://kj.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oi.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://qh.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pf.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qf.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://rt.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hw.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://so.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jw.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fb.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://th.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vn.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yu.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oc.shxzukj.cn

[L03] 设置自定义请求头
来源：http://tp.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vk.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hd.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rr.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vq.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xi.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cv.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yr.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xr.muxihuayi.cn

[L04] 设置超时
来源：http://qo.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://dm.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hu.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ox.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kw.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rm.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fu.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xz.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://co.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://ey.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dh.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bn.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qa.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ke.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kg.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ba.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uo.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wj.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://gq.shxzskj.cn

Py:   resp.json()
来源：http://uk.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://is.shxzskj.cn

JS:   await resp.json()
来源：http://ae.jctech888.com.cn

TS:   await resp.json()
来源：http://rq.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ec.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://it.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://sh.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ny.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://pu.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pp.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qb.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://dv.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://zb.shxzskj.cn

Java: resp.statusCode()
来源：http://gw.newstarts.cn

Go:   resp.StatusCode
来源：http://mi.9csxet.cn

Ruby: resp.code.to_i
来源：http://ms.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://du.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://nx.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lp.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://hq.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wy.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jb.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ki.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gh.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eq.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fc.yuexingan06.cn

================================================================================
来源：http://yy.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://td.9csxet.cn

================================================================================
来源：http://si.shtwfgs.cn

[M01] 读取命令行参数
来源：http://bz.gzmigu.cn

Py:   sys.argv[1:]
来源：http://ws.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://xk.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://wn.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://ts.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://zk.newstarts.cn

Go:   os.Args[1:]
来源：http://nz.asd995.cn

Ruby: ARGV
来源：http://tf.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://zf.panjiajie.cn

[M02] 读取环境变量
来源：http://ra.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://ya.huixinmuqiang.cn


<!-- 参考信息 -->