代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uz.hahajie.cn

[I03] 提取捕获分组
来源：http://od.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tc.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xk.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://em.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rm.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wj.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ps.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vw.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rk.nicolike.cn

[I04] 正则替换
来源：http://ae.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kh.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lw.muxihuayi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://on.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sc.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xw.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fk.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bu.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ro.9csxet.cn

[I05] 按正则拆分
来源：http://zr.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qp.asd995.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qu.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://mv.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://ph.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://ko.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ed.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yk.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gv.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zy.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rk.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ql.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lo.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ap.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://td.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ml.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qx.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://is.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://kz.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vg.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oq.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fs.huixinmuqiang.cn

TS:   /error/gim
来源：http://zm.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gd.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jh.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://xx.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nw.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://ix.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jb.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://td.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qx.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://it.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://il.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pe.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ul.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ni.haigaiapp.cn

================================================================================
来源：http://nx.yuexingan06.cn

J. 日期与时间
来源：http://wn.wgjwhj.cn

================================================================================
来源：http://nr.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://cg.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://db.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cg.nszjky.cn

JS:   new Date();  Date.now()
来源：http://ca.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://fa.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://un.hnjuh.cn

Go:   time.Now()
来源：http://nb.jctech888.com.cn

Ruby: Time.now
来源：http://kq.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://be.huixiangedu.cn

[J02] 格式化输出
来源：http://yg.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wn.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wo.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nx.muxihuayi.cn

TS:   d.toISOString()
来源：http://rr.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://he.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ej.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pv.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ol.521024.cn

[J03] 字符串解析为日期
来源：http://oz.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rj.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hr.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://bi.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://of.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dj.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cr.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://xu.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mc.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://rw.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xq.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xe.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jp.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gr.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lc.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bp.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lz.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://et.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://ka.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://oa.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mj.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tt.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qs.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://mt.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ib.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://ma.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hj.muxihuayi.cn

[J06] 计算两时间之差
来源：http://dr.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://lg.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://xw.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kv.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sf.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://me.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://yq.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://yl.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://dd.hahajie.cn

[J07] 比较两个日期
来源：http://fr.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://kh.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ql.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://es.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kb.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ba.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ix.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bz.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://ho.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://iu.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lg.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wg.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fi.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ac.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jf.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zb.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wq.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zv.yuntaijiaju.cn

[J09] 时区处理
来源：http://cx.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gq.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tq.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ye.jctech888.com.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uf.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://od.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kq.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rw.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fz.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://yq.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wk.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://er.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ug.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rv.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jj.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ji.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://na.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ic.yuntaijiaju.cn

================================================================================
来源：http://ox.521024.cn

K. JSON 与序列化
来源：http://rt.nszjky.cn

================================================================================
来源：http://ef.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://xp.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rc.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gu.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://ga.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://cn.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zn.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://bp.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yh.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lu.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://fi.chemitech.net.cn

Py:   json.loads(s)
来源：http://rn.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iq.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://zu.panjiajie.cn

TS:   JSON.parse(s)
来源：http://cr.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fm.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://ay.9csxet.cn

Ruby: JSON.parse(s)
来源：http://dl.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uy.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://pg.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://td.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hk.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sy.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yb.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zr.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ko.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lq.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cq.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://kl.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dx.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iz.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xp.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lm.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://df.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ch.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kx.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lo.asd995.cn

[K05] 深拷贝对象
来源：http://mt.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://gp.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://lb.nszjky.cn

JS:   structuredClone(obj)
来源：http://jo.nszjky.cn

TS:   structuredClone(obj)
来源：http://ys.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wq.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xl.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wc.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hp.newstarts.cn

[K06] 解析 URL 查询串
来源：http://jc.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eg.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wx.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ob.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yb.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ia.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tk.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lf.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ns.huixiangedu.cn

[K07] 进制转换
来源：http://ts.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hj.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mi.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vr.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wv.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zz.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eh.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jf.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sn.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://rd.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://wi.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yx.szsharing.cn

JS:   v8.serialize(obj)        // Node
来源：http://ac.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://jn.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ia.shxzskj.cn

Go:   encoding/gob
来源：http://bo.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://ld.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://im.gzmigu.cn

================================================================================
来源：http://ch.yuexingan06.cn

L. 网络请求
来源：http://be.shtwfgs.cn

================================================================================
来源：http://hv.panjiajie.cn

[L01] 发送 GET 请求
来源：http://nv.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gc.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://md.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://yg.asd995.cn

TS:   await fetch(url)
来源：http://nz.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kk.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://xd.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ew.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eu.521024.cn

[L02] 发送 POST JSON
来源：http://je.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mf.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vi.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ks.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yt.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jh.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zi.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pv.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mp.shxzskj.cn

[L03] 设置自定义请求头
来源：http://dl.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uk.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zs.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vw.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dd.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ab.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fp.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qz.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vl.shxzukj.cn

[L04] 设置超时
来源：http://uk.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://os.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jk.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ad.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ul.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jk.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dd.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fr.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aq.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://eq.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ek.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jx.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ew.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hb.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uf.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hf.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://du.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ll.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://hj.szxytkj.cn

Py:   resp.json()
来源：http://yk.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://ac.bjjhwx.cn

JS:   await resp.json()
来源：http://tg.haigaiapp.cn

TS:   await resp.json()
来源：http://cb.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qo.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vz.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://sc.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gh.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://rq.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vl.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cx.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://gz.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://ny.colortex.cn

Java: resp.statusCode()
来源：http://ug.9csxet.cn

Go:   resp.StatusCode
来源：http://ie.colortex.cn

Ruby: resp.code.to_i
来源：http://cv.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://oh.nszjky.cn

[L08] 并发请求多个地址
来源：http://hz.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bo.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://bk.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bv.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ii.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dy.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ut.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zo.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ad.newstarts.cn

================================================================================
来源：http://am.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://ta.szsharing.cn


<!-- 参考信息 -->