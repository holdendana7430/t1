代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://kj.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://th.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://am.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://dk.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://uq.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://em.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://um.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ez.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qz.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ml.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ng.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ho.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ab.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fz.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vb.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uf.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vz.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://fz.szxytkj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sw.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://al.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ad.nszjky.cn

TS:   /error/gim
来源：http://mk.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gg.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bv.jctech888.com.cn

Ruby: s.scan(/error/i)
来源：http://ro.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gb.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://bx.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://os.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vd.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tm.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yr.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tk.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pd.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yd.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ov.jianghongdianzi.cn

================================================================================
来源：http://fk.521024.cn

J. 日期与时间
来源：http://fw.bjjhwx.cn

================================================================================
来源：http://wl.lnxyls.cn

[J01] 获取当前时间
来源：http://ql.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ig.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wa.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://zi.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://be.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pu.shxzskj.cn

Go:   time.Now()
来源：http://ub.wgjwhj.cn

Ruby: Time.now
来源：http://bx.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://va.shxzskj.cn

[J02] 格式化输出
来源：http://ls.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bx.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qn.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nc.yuexingan06.cn

TS:   d.toISOString()
来源：http://dt.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fw.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://un.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vd.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vi.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://po.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cm.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ll.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://ld.521024.cn

TS:   new Date("2024-01-02")
来源：http://kq.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zt.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qz.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://pp.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cx.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://fe.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yl.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kk.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qp.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rl.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pp.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wr.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gk.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gv.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://is.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://ok.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vq.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vp.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dz.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://nw.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xt.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://iq.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cn.hnjuh.cn

[J06] 计算两时间之差
来源：http://rk.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://qu.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://tn.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oj.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rm.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tg.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://dc.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://dt.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://yk.szxytkj.cn

[J07] 比较两个日期
来源：http://yo.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://mw.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zy.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://om.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jn.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zb.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pc.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zy.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://qn.asd995.cn

[J08] 提取年月日与星期
来源：http://wf.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bj.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vm.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mj.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fn.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cy.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ra.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qv.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jj.yuntaijiaju.cn

[J09] 时区处理
来源：http://wv.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yc.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pg.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://su.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vz.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fy.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zx.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ft.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bh.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://hk.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ys.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ng.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ia.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fm.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ea.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sv.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jv.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cr.lnxyls.cn

================================================================================
来源：http://di.nszjky.cn

K. JSON 与序列化
来源：http://ik.shtwfgs.cn

================================================================================
来源：http://zu.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://vc.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ep.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hc.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://wc.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://py.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ma.colortex.cn

Go:   json.Marshal(obj)
来源：http://af.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fv.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qc.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://cw.shxzukj.cn

Py:   json.loads(s)
来源：http://iq.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jh.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://vt.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://ns.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xm.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://jl.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://xn.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wb.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://cn.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ts.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://er.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nf.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jb.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dg.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wb.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wp.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jm.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://rs.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://re.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ud.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ff.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ez.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pb.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ir.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tf.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://az.huixiangedu.cn

[K05] 深拷贝对象
来源：http://tk.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://rv.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://kb.521024.cn

JS:   structuredClone(obj)
来源：http://df.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://ca.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hq.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pi.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nm.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fd.szsharing.cn

[K06] 解析 URL 查询串
来源：http://uc.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://io.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ji.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tu.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wn.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cr.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wd.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bo.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gc.yuexingan06.cn

[K07] 进制转换
来源：http://jw.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://la.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zb.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ym.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wv.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://df.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nv.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vc.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pv.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://cv.asd995.cn

Py:   pickle.dumps(obj)
来源：http://yq.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zw.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://pr.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://ri.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dz.hahajie.cn

Go:   encoding/gob
来源：http://ob.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://ij.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jk.bookmarksfly.cn

================================================================================
来源：http://nx.yuntaijiaju.cn

L. 网络请求
来源：http://ck.yuexingan06.cn

================================================================================
来源：http://gv.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://pu.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tq.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qy.yuexingan06.cn

JS:   await fetch(url)
来源：http://sk.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://ku.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hw.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://xi.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oy.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hi.hnjuh.cn

[L02] 发送 POST JSON
来源：http://rb.colortex.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ej.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ym.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ro.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gl.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nz.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qk.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uh.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bi.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://om.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qb.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nt.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aj.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xd.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nb.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://za.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://od.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lr.wgjwhj.cn

[L04] 设置超时
来源：http://kd.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://pa.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cr.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dz.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ki.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yy.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nn.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yv.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nf.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://nv.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lf.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mq.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gk.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://of.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aq.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nc.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uo.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ks.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://wq.muxihuayi.cn

Py:   resp.json()
来源：http://wz.nicolike.cn

PHP:  json_decode($body, true);
来源：http://sw.yuexingan06.cn

JS:   await resp.json()
来源：http://oq.colortex.cn

TS:   await resp.json()
来源：http://wc.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ia.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://if.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://lq.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dx.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://nq.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://de.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bq.asd995.cn

JS:   resp.ok;  resp.status
来源：http://bq.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://qo.huanxung.cn

Java: resp.statusCode()
来源：http://ot.wgjwhj.cn

Go:   resp.StatusCode
来源：http://cl.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://in.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://qf.szxytkj.cn

[L08] 并发请求多个地址
来源：http://pv.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wy.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://dp.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://te.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fu.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rd.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://im.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lp.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bu.nszjky.cn

================================================================================
来源：http://bp.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://bh.jctech888.com.cn

================================================================================
来源：http://is.chemitech.net.cn

[M01] 读取命令行参数
来源：http://wg.nicolike.cn

Py:   sys.argv[1:]
来源：http://jk.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://oo.hahajie.cn

JS:   process.argv.slice(2)
来源：http://iz.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://rt.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://fu.panjiajie.cn

Go:   os.Args[1:]
来源：http://ki.szxytkj.cn

Ruby: ARGV
来源：http://oz.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://rb.hahajie.cn

[M02] 读取环境变量
来源：http://sf.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://bi.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ge.521024.cn

JS:   process.env.HOME
来源：http://lt.shtwfgs.cn

TS:   process.env.HOME
来源：http://wm.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://ya.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://he.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://zx.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mt.shxzukj.cn

[M03] 执行外部命令
来源：http://ow.521024.cn


<!-- 参考信息 -->