代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ei.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sk.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xp.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ok.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hv.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://me.huanxung.cn

[I04] 正则替换
来源：http://bn.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fn.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cp.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hy.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wh.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mg.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vs.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gn.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yk.shxzskj.cn

[I05] 按正则拆分
来源：http://tj.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fa.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wc.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://be.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://lj.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://dd.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ps.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ck.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xj.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cw.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xd.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pr.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fv.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bm.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fy.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wm.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rm.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nj.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://vy.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yj.bookmarksfly.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lv.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aa.hnjuh.cn

TS:   /error/gim
来源：http://hw.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fa.colortex.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gx.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://qh.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hu.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://mg.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ki.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ek.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jm.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xb.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vh.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qk.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cp.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xd.yuntaijiaju.cn

================================================================================
来源：http://ca.huanxung.cn

J. 日期与时间
来源：http://hp.szsharing.cn

================================================================================
来源：http://xq.shtwfgs.cn

[J01] 获取当前时间
来源：http://tk.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sh.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yv.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://aa.szsharing.cn

TS:   new Date();  Date.now()
来源：http://lh.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bk.jianghongdianzi.cn

Go:   time.Now()
来源：http://hi.yuexingan06.cn

Ruby: Time.now
来源：http://vb.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nh.chemitech.net.cn

[J02] 格式化输出
来源：http://pz.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://an.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://br.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nu.hahajie.cn

TS:   d.toISOString()
来源：http://vl.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zu.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mz.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://su.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zg.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://qg.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ks.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wh.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://jn.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://rk.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xa.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nf.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://qc.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wt.hahajie.cn

[J04] 时间戳与日期互转
来源：http://gn.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ik.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jq.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rg.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hf.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nm.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://db.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aq.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ny.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://ep.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://nl.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lw.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ar.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://je.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://mw.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rd.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://wy.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://as.chemitech.net.cn

[J06] 计算两时间之差
来源：http://jy.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://dm.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://zt.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ap.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cs.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rp.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://hx.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://ff.521024.cn

C#:   (end - start).TotalSeconds
来源：http://bw.bookmarksfly.cn

[J07] 比较两个日期
来源：http://do.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://oz.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zj.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hw.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ft.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zl.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://py.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gl.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://mg.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://yh.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oc.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ff.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ak.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pb.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ug.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gl.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sz.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fl.yuexingan06.cn

[J09] 时区处理
来源：http://hk.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tr.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mg.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jk.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vy.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rz.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ak.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mm.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ca.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://lh.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fc.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xq.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ym.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sd.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zs.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lv.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oz.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pe.wgjwhj.cn

================================================================================
来源：http://nb.521024.cn

K. JSON 与序列化
来源：http://qp.nicolike.cn

================================================================================
来源：http://nz.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://xc.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mu.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nm.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://ip.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://wo.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dd.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://wf.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xy.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jr.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://mj.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://qx.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jp.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://ai.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://tu.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zd.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://wh.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://tw.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qq.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://qn.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://if.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wd.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jh.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ce.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fw.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dm.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mu.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fj.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://qc.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gy.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gk.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vq.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fd.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zx.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ms.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yy.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kb.521024.cn

[K05] 深拷贝对象
来源：http://ed.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://nb.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://qh.szxytkj.cn

JS:   structuredClone(obj)
来源：http://kx.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://tj.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xm.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ds.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fs.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pj.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://wx.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ri.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sn.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pl.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aj.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bz.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ie.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qr.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mh.shxzskj.cn

[K07] 进制转换
来源：http://gh.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qj.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://by.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jo.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pf.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rg.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gt.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qq.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zp.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://tm.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://fx.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ay.521024.cn

JS:   v8.serialize(obj)        // Node
来源：http://mg.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://st.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://or.hahajie.cn

Go:   encoding/gob
来源：http://ze.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://zw.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ip.asd995.cn

================================================================================
来源：http://ni.shtwfgs.cn

L. 网络请求
来源：http://pu.haigaiapp.cn

================================================================================
来源：http://qb.szxytkj.cn

[L01] 发送 GET 请求
来源：http://ta.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bm.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bv.yuexingan06.cn

JS:   await fetch(url)
来源：http://pf.wgjwhj.cn

TS:   await fetch(url)
来源：http://fm.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://in.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://si.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bx.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tv.9csxet.cn

[L02] 发送 POST JSON
来源：http://ia.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bp.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mr.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ri.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ez.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vw.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mx.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rv.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dk.hahajie.cn

[L03] 设置自定义请求头
来源：http://jv.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uh.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://az.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sf.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qg.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wg.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ey.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ug.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jb.nszjky.cn

[L04] 设置超时
来源：http://zx.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://mu.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rc.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hu.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://da.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qr.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tb.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qn.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cz.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://xv.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kj.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wi.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ty.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qe.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nv.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vy.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://to.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://el.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://kc.hahajie.cn

Py:   resp.json()
来源：http://ha.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://ru.jctech888.com.cn

JS:   await resp.json()
来源：http://wa.521024.cn

TS:   await resp.json()
来源：http://xl.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vn.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ps.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://bo.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ra.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://ra.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vl.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hc.huanxung.cn

JS:   resp.ok;  resp.status
来源：http://pa.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://ae.shxzskj.cn

Java: resp.statusCode()
来源：http://sw.wgjwhj.cn

Go:   resp.StatusCode
来源：http://cb.newstarts.cn

Ruby: resp.code.to_i
来源：http://gi.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://kt.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://yu.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ji.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://ex.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://so.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://js.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yu.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zb.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uk.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ct.hnjuh.cn

================================================================================
来源：http://rr.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://kq.bjjhwx.cn

================================================================================
来源：http://ug.haigaiapp.cn

[M01] 读取命令行参数
来源：http://vv.szxytkj.cn

Py:   sys.argv[1:]
来源：http://jw.hahajie.cn

PHP:  $argv;  $argc;
来源：http://qe.chemitech.net.cn


<!-- 参考信息 -->