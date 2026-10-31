代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zc.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://oe.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://od.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wx.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lr.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oz.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cn.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zk.nszjky.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://us.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yu.muxihuayi.cn

[I04] 正则替换
来源：http://ak.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bv.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://it.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yw.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tk.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://am.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://au.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hy.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xm.gzmigu.cn

[I05] 按正则拆分
来源：http://ex.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://we.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rq.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://kg.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://qz.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://ji.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://al.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://eg.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qx.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uo.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://li.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://un.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://of.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://us.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lc.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cg.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xp.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mg.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://hq.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ct.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qx.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ri.yuntaijiaju.cn

TS:   /error/gim
来源：http://cn.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://df.521024.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iz.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://co.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://my.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://je.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gs.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ym.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nl.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jq.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ih.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pp.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cf.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lc.jianghongdianzi.cn

================================================================================
来源：http://hy.asd995.cn

J. 日期与时间
来源：http://dt.gzmigu.cn

================================================================================
来源：http://hx.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://am.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cm.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jn.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://td.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://kv.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yx.huixiangedu.cn

Go:   time.Now()
来源：http://zs.gzmigu.cn

Ruby: Time.now
来源：http://ye.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rf.huixiangedu.cn

[J02] 格式化输出
来源：http://kv.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vm.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ro.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ap.jctech888.com.cn

TS:   d.toISOString()
来源：http://bf.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pz.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nv.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qj.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nx.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://tc.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cp.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://et.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://tp.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://ad.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bm.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jp.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://th.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nu.nicolike.cn

[J04] 时间戳与日期互转
来源：http://cy.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ww.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mt.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ng.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ri.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zb.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://me.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pr.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bx.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://wz.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://hm.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qd.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cm.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ql.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://sq.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vb.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://ax.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vt.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://zo.asd995.cn

Py:   (end - start).total_seconds()
来源：http://fx.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://qn.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pn.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zy.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zi.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://do.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://ep.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://aj.9csxet.cn

[J07] 比较两个日期
来源：http://fc.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://tu.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ne.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://aa.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ey.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wy.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ze.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vd.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://ig.colortex.cn

[J08] 提取年月日与星期
来源：http://ym.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yg.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cl.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wh.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uu.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://av.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ok.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hi.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dn.hnjuh.cn

[J09] 时区处理
来源：http://la.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qz.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fp.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uz.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aq.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oi.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bk.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kr.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://va.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://jn.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://to.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sg.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qs.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nv.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yq.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tt.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gp.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nw.newstarts.cn

================================================================================
来源：http://tz.wgjwhj.cn

K. JSON 与序列化
来源：http://lg.gzmigu.cn

================================================================================
来源：http://uz.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://ga.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uy.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oi.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://sv.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://qy.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mn.hahajie.cn

Go:   json.Marshal(obj)
来源：http://wm.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pg.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gk.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://zj.huanxung.cn

Py:   json.loads(s)
来源：http://ly.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qr.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://vk.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://ob.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dg.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://we.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://uc.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pl.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://da.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wi.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iy.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bn.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bz.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eq.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ov.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dd.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nz.9csxet.cn

[K04] 读取 JSON 文件
来源：http://gp.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bs.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fk.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qg.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wf.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mu.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://da.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vq.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gs.szsharing.cn

[K05] 深拷贝对象
来源：http://wv.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://lf.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://uz.hahajie.cn

JS:   structuredClone(obj)
来源：http://bb.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://rh.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cf.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ht.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kv.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://af.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://fd.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aa.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fw.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://px.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://td.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zp.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ym.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cv.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qn.muxihuayi.cn

[K07] 进制转换
来源：http://nq.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yl.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ll.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bi.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xn.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sz.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mv.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wc.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wo.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://dm.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://tt.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ej.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://ls.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://au.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cn.asd995.cn

Go:   encoding/gob
来源：http://qs.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://fr.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://je.gzmigu.cn

================================================================================
来源：http://mi.huixinmuqiang.cn

L. 网络请求
来源：http://dp.521024.cn

================================================================================
来源：http://qf.521024.cn

[L01] 发送 GET 请求
来源：http://uw.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jx.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yo.shxzskj.cn

JS:   await fetch(url)
来源：http://kg.newstarts.cn

TS:   await fetch(url)
来源：http://am.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nc.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://da.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lk.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://du.huanxung.cn

[L02] 发送 POST JSON
来源：http://ma.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://az.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dk.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jn.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aa.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mj.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qo.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tb.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pp.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://ow.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qx.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dt.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ho.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qp.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xp.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pd.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://he.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ax.huixinmuqiang.cn

[L04] 设置超时
来源：http://sl.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://di.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dl.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dc.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gj.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sj.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ej.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hc.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pk.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://tb.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ve.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jp.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ul.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xh.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nn.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tp.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vh.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sm.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://in.yuexingan06.cn

Py:   resp.json()
来源：http://pp.colortex.cn

PHP:  json_decode($body, true);
来源：http://ro.szxytkj.cn

JS:   await resp.json()
来源：http://wu.asd995.cn

TS:   await resp.json()
来源：http://qw.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ac.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ql.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://kh.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kp.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://ku.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mn.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oy.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://nt.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://tj.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://sn.newstarts.cn

Go:   resp.StatusCode
来源：http://il.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://sd.asd995.cn

C#:   (int)resp.StatusCode
来源：http://cq.gzmigu.cn

[L08] 并发请求多个地址
来源：http://yl.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xr.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://nj.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gr.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://es.nicolike.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yx.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eq.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hy.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xb.wgjwhj.cn

================================================================================
来源：http://jx.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://fz.huixiangedu.cn


<!-- 参考信息 -->