代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bk.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cw.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yi.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mv.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cx.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dq.hnjuh.cn

[I04] 正则替换
来源：http://tb.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pi.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nn.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kq.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vl.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qm.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kg.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ch.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dq.colortex.cn

[I05] 按正则拆分
来源：http://vk.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nx.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zm.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://ui.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://al.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://lr.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tj.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fl.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kq.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yd.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wz.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wn.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nx.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wz.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lk.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gb.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ck.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yi.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://gl.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oe.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xi.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jy.shxzukj.cn

TS:   /error/gim
来源：http://yv.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ae.521024.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wk.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://ir.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nw.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://yg.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jk.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rt.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iy.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sj.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bi.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xh.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ev.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zn.jctech888.com.cn

================================================================================
来源：http://ek.szsharing.cn

J. 日期与时间
来源：http://nt.chemitech.net.cn

================================================================================
来源：http://pm.lnxyls.cn

[J01] 获取当前时间
来源：http://rt.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://za.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qg.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://ey.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://xo.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ga.521024.cn

Go:   time.Now()
来源：http://oz.haigaiapp.cn

Ruby: Time.now
来源：http://gb.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oo.9csxet.cn

[J02] 格式化输出
来源：http://yd.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lh.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hq.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hp.huixiangedu.cn

TS:   d.toISOString()
来源：http://yk.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yw.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qt.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bz.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://od.hahajie.cn

[J03] 字符串解析为日期
来源：http://ky.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iw.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mt.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://rk.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://le.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://of.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qa.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://dg.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ti.9csxet.cn

[J04] 时间戳与日期互转
来源：http://sj.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://du.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fe.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ij.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fy.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fd.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ba.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pt.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://md.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://ob.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://fv.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hl.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ln.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bp.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://dd.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wv.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://uv.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xw.szxytkj.cn

[J06] 计算两时间之差
来源：http://hh.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://qt.521024.cn

PHP:  $end->diff($start)->days;
来源：http://xo.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qb.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vs.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xp.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://pu.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://bk.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://wh.nszjky.cn

[J07] 比较两个日期
来源：http://gl.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://sc.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mm.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ci.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ge.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://at.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zg.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lz.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://wo.szsharing.cn

[J08] 提取年月日与星期
来源：http://xe.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eg.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kx.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yz.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zq.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hs.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qz.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://so.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mx.hnjuh.cn

[J09] 时区处理
来源：http://wy.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uc.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dm.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fe.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vw.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xc.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ld.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://im.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zj.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://nh.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tp.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://so.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cf.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lg.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pm.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ft.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xg.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oq.hnjuh.cn

================================================================================
来源：http://pn.gzmigu.cn

K. JSON 与序列化
来源：http://jr.szsharing.cn

================================================================================
来源：http://ox.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://tr.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cg.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ty.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://ky.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://mp.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lj.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://if.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kc.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ds.nszjky.cn

[K02] JSON 字符串转对象
来源：http://pp.panjiajie.cn

Py:   json.loads(s)
来源：http://vs.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ur.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://ex.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://fn.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rc.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://oq.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://wn.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wz.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://xu.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jg.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ev.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hh.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dj.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://du.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ph.521024.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lq.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bz.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://xs.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://af.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://is.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cn.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gg.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jc.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wu.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ze.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ad.hahajie.cn

[K05] 深拷贝对象
来源：http://ka.521024.cn

Py:   copy.deepcopy(obj)
来源：http://ew.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://pm.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://vm.521024.cn

TS:   structuredClone(obj)
来源：http://oz.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://of.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yl.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ei.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wr.nicolike.cn

[K06] 解析 URL 查询串
来源：http://tx.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qp.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dd.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bj.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ij.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jx.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pl.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://is.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://db.shxzskj.cn

[K07] 进制转换
来源：http://kh.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ga.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xb.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zg.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vu.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ce.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uy.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gf.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jb.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://bs.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://yv.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ey.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://ja.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://zl.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yc.hnjuh.cn

Go:   encoding/gob
来源：http://tb.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://ld.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xo.huixiangedu.cn

================================================================================
来源：http://vp.muxihuayi.cn

L. 网络请求
来源：http://iz.nszjky.cn

================================================================================
来源：http://vi.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://uh.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pc.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ss.gzmigu.cn

JS:   await fetch(url)
来源：http://yz.nszjky.cn

TS:   await fetch(url)
来源：http://xt.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lv.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://bn.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eu.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uo.lnxyls.cn

[L02] 发送 POST JSON
来源：http://si.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fc.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ve.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rp.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tj.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cf.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://az.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wj.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yh.bjjhwx.cn

[L03] 设置自定义请求头
来源：http://fj.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gm.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://la.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://su.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fm.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fq.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sz.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eb.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ai.bjjhwx.cn

[L04] 设置超时
来源：http://ck.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://hs.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xl.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nu.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pk.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://st.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://es.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hf.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hu.hahajie.cn

[L05] 上传文件（multipart）
来源：http://ur.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ou.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qf.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ax.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://it.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ri.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kx.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wu.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ia.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://it.9csxet.cn

Py:   resp.json()
来源：http://uv.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://no.gzmigu.cn

JS:   await resp.json()
来源：http://jo.muxihuayi.cn

TS:   await resp.json()
来源：http://el.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oy.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qw.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://os.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sa.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://tv.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iz.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://af.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://ui.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://mr.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://df.huixiangedu.cn

Go:   resp.StatusCode
来源：http://vs.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://hz.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://og.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://qo.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://li.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://wh.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dk.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ur.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cj.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qv.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jv.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sv.haigaiapp.cn

================================================================================
来源：http://vq.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://na.jianghongdianzi.cn

================================================================================
来源：http://zp.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://fd.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://nk.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://gj.asd995.cn


<!-- 参考信息 -->