代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gy.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dz.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://eh.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cm.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nj.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xr.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ti.jctech888.com.cn

[I05] 按正则拆分
来源：http://fq.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nv.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ch.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://rq.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://nq.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://zq.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ys.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uh.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qf.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ib.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bj.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rc.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pi.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xt.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wk.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jd.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nx.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yq.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://qc.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://en.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vo.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mx.newstarts.cn

TS:   /error/gim
来源：http://hn.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jb.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://re.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://aq.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kv.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://od.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vj.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sk.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wr.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sa.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gf.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pl.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wj.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pp.huixiangedu.cn

================================================================================
来源：http://sv.huixiangedu.cn

J. 日期与时间
来源：http://ze.hahajie.cn

================================================================================
来源：http://zk.521024.cn

[J01] 获取当前时间
来源：http://ii.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wj.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vp.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://fl.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://zy.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tj.szsharing.cn

Go:   time.Now()
来源：http://rj.shxzskj.cn

Ruby: Time.now
来源：http://ag.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xy.gzmigu.cn

[J02] 格式化输出
来源：http://rz.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ci.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fr.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ts.9csxet.cn

TS:   d.toISOString()
来源：http://ua.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hs.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jo.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hp.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xz.panjiajie.cn

[J03] 字符串解析为日期
来源：http://gv.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://za.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ra.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://vl.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://lm.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ok.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zx.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://oo.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rk.nicolike.cn

[J04] 时间戳与日期互转
来源：http://gf.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ot.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rb.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vr.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xd.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://we.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kr.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://te.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yx.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://nk.colortex.cn

Py:   now + timedelta(days=7)
来源：http://qn.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ne.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wu.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sd.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://yz.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uu.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://nq.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qm.szsharing.cn

[J06] 计算两时间之差
来源：http://jw.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://hx.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://py.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gk.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jm.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bo.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://ey.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://xp.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://gl.yuexingan06.cn

[J07] 比较两个日期
来源：http://bw.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://uj.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ee.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pj.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hl.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vw.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://di.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wm.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://gj.shxzukj.cn

[J08] 提取年月日与星期
来源：http://ea.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dv.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dm.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gg.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ei.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qm.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dr.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ry.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tl.wgjwhj.cn

[J09] 时区处理
来源：http://qg.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ag.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yp.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qc.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wx.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uo.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wa.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uz.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bf.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://nj.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mq.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://do.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yv.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ba.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xo.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ak.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://io.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ue.bjjhwx.cn

================================================================================
来源：http://jc.asd995.cn

K. JSON 与序列化
来源：http://sf.hnjuh.cn

================================================================================
来源：http://xi.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://as.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nb.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jz.colortex.cn

JS:   JSON.stringify(obj)
来源：http://ve.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://xu.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://to.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://zy.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bi.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mm.9csxet.cn

[K02] JSON 字符串转对象
来源：http://gq.haigaiapp.cn

Py:   json.loads(s)
来源：http://jn.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vv.lnxyls.cn

JS:   JSON.parse(s)
来源：http://qf.hahajie.cn

TS:   JSON.parse(s)
来源：http://ec.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zk.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://kx.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://dt.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qd.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://te.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pp.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://km.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jn.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tk.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://le.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ie.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vx.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wo.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://bi.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hf.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://az.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mb.gzmigu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ja.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fc.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ge.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zb.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cs.nicolike.cn

[K05] 深拷贝对象
来源：http://qy.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://qd.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://au.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://ps.hahajie.cn

TS:   structuredClone(obj)
来源：http://gu.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://md.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ng.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://me.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sc.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://qh.gzmigu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vc.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mw.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rw.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xr.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gi.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sx.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mf.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kw.521024.cn

[K07] 进制转换
来源：http://rz.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yb.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oq.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fb.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kj.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qy.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xk.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qb.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zz.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://sw.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://xc.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rz.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://hj.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://xg.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ux.shxzukj.cn

Go:   encoding/gob
来源：http://vz.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://co.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ks.wgjwhj.cn

================================================================================
来源：http://ln.hnjuh.cn

L. 网络请求
来源：http://pn.szsharing.cn

================================================================================
来源：http://ke.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://mn.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ad.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iz.colortex.cn

JS:   await fetch(url)
来源：http://bw.bookmarksfly.cn

TS:   await fetch(url)
来源：http://xc.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pb.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://jq.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://iq.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qf.9csxet.cn

[L02] 发送 POST JSON
来源：http://jz.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pw.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ge.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mm.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xg.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ai.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hd.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zs.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ks.521024.cn

[L03] 设置自定义请求头
来源：http://sx.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hx.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gj.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gc.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rg.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sw.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cq.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xh.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xh.chemitech.net.cn

[L04] 设置超时
来源：http://yt.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://dp.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ge.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sk.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wq.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fn.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uf.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kr.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hd.nicolike.cn

[L05] 上传文件（multipart）
来源：http://sb.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zh.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rp.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tk.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iw.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ht.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wh.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://if.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pc.521024.cn

[L06] 解析响应为 JSON
来源：http://au.szxytkj.cn

Py:   resp.json()
来源：http://io.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://ze.shxzukj.cn

JS:   await resp.json()
来源：http://ed.nicolike.cn

TS:   await resp.json()
来源：http://bc.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://da.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lo.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://rp.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zc.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://pu.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bu.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yk.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://bh.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://zt.jctech888.com.cn

Java: resp.statusCode()
来源：http://cx.chemitech.net.cn

Go:   resp.StatusCode
来源：http://kg.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://wj.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://nz.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://ce.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jj.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://py.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wj.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zg.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xd.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zs.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lb.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://te.szsharing.cn

================================================================================
来源：http://zo.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://rc.jianghongdianzi.cn

================================================================================
来源：http://um.gzmigu.cn

[M01] 读取命令行参数
来源：http://op.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://qh.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://mx.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://el.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://yv.colortex.cn

Java: args 数组（main 方法参数）
来源：http://cs.panjiajie.cn

Go:   os.Args[1:]
来源：http://yw.newstarts.cn

Ruby: ARGV
来源：http://qx.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://ed.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://pu.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://kw.gzmigu.cn


<!-- 参考信息 -->