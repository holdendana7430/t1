代发 wailian999

TS:   s.match(/\d+/g)
来源：http://wd.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cu.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ic.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://hh.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pw.shtwfgs.cn

[I03] 提取捕获分组
来源：http://ru.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tj.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yv.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dc.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tn.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wc.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wi.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://be.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cr.shtwfgs.cn

[I04] 正则替换
来源：http://te.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://av.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gk.lnxyls.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jc.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dc.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://du.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dv.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bv.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ty.huixiangedu.cn

[I05] 按正则拆分
来源：http://tt.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gj.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pm.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://dk.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://qs.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://bo.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hk.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zy.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rb.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dc.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ct.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jx.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rh.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ek.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bo.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ek.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gp.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iz.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://er.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ir.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qm.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://go.wgjwhj.cn

TS:   /error/gim
来源：http://tr.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zl.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://ed.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pz.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://ei.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hg.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ey.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ub.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hw.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nn.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tg.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lw.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hw.newstarts.cn

================================================================================
来源：http://fw.colortex.cn

J. 日期与时间
来源：http://pp.bjjhwx.cn

================================================================================
来源：http://kj.yuexingan06.cn

[J01] 获取当前时间
来源：http://gh.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://re.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zc.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://as.newstarts.cn

TS:   new Date();  Date.now()
来源：http://iz.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jy.bjjhwx.cn

Go:   time.Now()
来源：http://wh.shxzskj.cn

Ruby: Time.now
来源：http://pk.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dz.bjjhwx.cn

[J02] 格式化输出
来源：http://as.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dg.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ar.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ma.colortex.cn

TS:   d.toISOString()
来源：http://my.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xn.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bd.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://po.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eb.szxytkj.cn

[J03] 字符串解析为日期
来源：http://ak.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ia.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fc.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://bl.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://zu.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ts.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ze.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://ay.521024.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cf.colortex.cn

[J04] 时间戳与日期互转
来源：http://kc.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lp.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yu.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yf.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ah.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ww.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://px.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lx.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wj.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://pl.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://qw.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://db.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ts.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wn.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://eq.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tk.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://qs.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uv.chemitech.net.cn

[J06] 计算两时间之差
来源：http://fy.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://al.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://gk.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vj.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dh.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zc.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://dk.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://bt.521024.cn

C#:   (end - start).TotalSeconds
来源：http://aa.hnjuh.cn

[J07] 比较两个日期
来源：http://bk.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://kt.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ji.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xn.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hb.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kx.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hr.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wv.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://zd.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://hg.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vz.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yo.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hi.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gh.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wj.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ss.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wp.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uc.jctech888.com.cn

[J09] 时区处理
来源：http://oa.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zc.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qw.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ti.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dp.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ts.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://va.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tn.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://st.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://bs.gzmigu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mx.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://al.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fy.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yv.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rt.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wu.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bu.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zm.huixinmuqiang.cn

================================================================================
来源：http://uv.bjjhwx.cn

K. JSON 与序列化
来源：http://bh.9csxet.cn

================================================================================
来源：http://ab.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://le.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xp.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bc.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://dv.521024.cn

TS:   JSON.stringify(obj)
来源：http://iw.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qo.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://se.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ef.lnxyls.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bm.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://lv.yuexingan06.cn

Py:   json.loads(s)
来源：http://lb.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ky.shxzskj.cn

JS:   JSON.parse(s)
来源：http://hj.nicolike.cn

TS:   JSON.parse(s)
来源：http://ou.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ji.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://nv.hahajie.cn

Ruby: JSON.parse(s)
来源：http://zm.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dr.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://dt.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eq.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jx.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cr.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xv.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ha.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ea.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xa.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cm.9csxet.cn

[K04] 读取 JSON 文件
来源：http://dm.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yc.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ft.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gw.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ti.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zh.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://le.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://io.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://et.yuexingan06.cn

[K05] 深拷贝对象
来源：http://cf.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://ko.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://fz.nicolike.cn

JS:   structuredClone(obj)
来源：http://at.521024.cn

TS:   structuredClone(obj)
来源：http://fx.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://et.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rb.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vd.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://de.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://mc.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://at.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sp.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kz.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zt.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gp.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cw.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vm.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aj.bookmarksfly.cn

[K07] 进制转换
来源：http://xs.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hp.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qw.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zp.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rw.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xc.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qk.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ql.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yl.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://gg.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://dv.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://we.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://gy.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://ud.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://po.muxihuayi.cn

Go:   encoding/gob
来源：http://qf.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://gi.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vz.huixiangedu.cn

================================================================================
来源：http://mo.newstarts.cn

L. 网络请求
来源：http://kq.haigaiapp.cn

================================================================================
来源：http://ik.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://is.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wr.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ip.hahajie.cn

JS:   await fetch(url)
来源：http://yt.huanxung.cn

TS:   await fetch(url)
来源：http://im.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xw.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://va.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fz.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vo.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://wy.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wa.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://br.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://su.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://co.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vy.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zi.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xx.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cw.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://dq.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://im.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://si.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://or.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ut.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zp.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://id.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xf.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bw.yuexingan06.cn

[L04] 设置超时
来源：http://jq.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://gf.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xa.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bf.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ym.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rp.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://if.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ub.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gq.colortex.cn

[L05] 上传文件（multipart）
来源：http://sb.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iu.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iz.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hd.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rm.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xt.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://km.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://np.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rl.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://nv.newstarts.cn

Py:   resp.json()
来源：http://kd.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://th.shtwfgs.cn

JS:   await resp.json()
来源：http://qc.gzmigu.cn

TS:   await resp.json()
来源：http://ix.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://co.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ya.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://vf.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jo.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://yr.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://al.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gn.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://jk.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://of.huixiangedu.cn

Java: resp.statusCode()
来源：http://lz.yuexingan06.cn

Go:   resp.StatusCode
来源：http://ji.gzmigu.cn

Ruby: resp.code.to_i
来源：http://hf.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://ho.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://jx.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bn.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://zu.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iu.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jd.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vr.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sn.huixiangedu.cn


<!-- 参考信息 -->