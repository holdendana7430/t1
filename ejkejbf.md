代发 wailian999

TS:   s.match(/\d+/g)
来源：http://ah.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yo.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://to.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://zi.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ct.szxytkj.cn

[I03] 提取捕获分组
来源：http://je.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fg.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kl.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rd.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pv.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zv.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://px.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kn.muxihuayi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cu.shxzukj.cn

[I04] 正则替换
来源：http://ip.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ly.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qw.muxihuayi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fl.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jx.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yk.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xs.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mm.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jg.nszjky.cn

[I05] 按正则拆分
来源：http://tu.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nr.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kl.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://rs.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://bh.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://tk.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wr.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nm.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xe.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ah.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ck.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sx.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gw.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sl.szxytkj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aw.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dw.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rr.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qf.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://kv.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xp.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://px.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dc.lnxyls.cn

TS:   /error/gim
来源：http://tr.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zh.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xz.jctech888.com.cn

Ruby: s.scan(/error/i)
来源：http://cw.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ut.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://df.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gh.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cs.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nw.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://be.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fq.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pt.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tm.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mr.szsharing.cn

================================================================================
来源：http://mb.shtwfgs.cn

J. 日期与时间
来源：http://di.haigaiapp.cn

================================================================================
来源：http://ba.bookmarksfly.cn

[J01] 获取当前时间
来源：http://mw.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yz.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xx.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://zl.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://vd.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dz.bjjhwx.cn

Go:   time.Now()
来源：http://sd.newstarts.cn

Ruby: Time.now
来源：http://qx.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pp.colortex.cn

[J02] 格式化输出
来源：http://en.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eq.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ln.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zs.bjjhwx.cn

TS:   d.toISOString()
来源：http://vq.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fd.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ua.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pt.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ma.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://ro.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hd.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lj.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://ua.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://xe.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ys.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yu.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://td.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xy.huanxung.cn

[J04] 时间戳与日期互转
来源：http://vz.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cd.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zw.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qr.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tf.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xv.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mc.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vo.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mn.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://dt.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://jl.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pp.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fz.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kv.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://wk.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ym.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://lk.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bn.bjjhwx.cn

[J06] 计算两时间之差
来源：http://dq.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://un.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://vo.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lg.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tg.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://er.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://el.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://tl.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://yg.haigaiapp.cn

[J07] 比较两个日期
来源：http://nn.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://me.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uc.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vz.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cg.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qr.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://um.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://la.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://xb.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://qp.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://th.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vk.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lo.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yz.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pi.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gz.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aa.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gh.bjjhwx.cn

[J09] 时区处理
来源：http://xa.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://di.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zm.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dh.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mr.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yt.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ho.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://aq.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://db.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://zd.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jv.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jo.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ha.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cr.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fr.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://su.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ut.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xi.huixinmuqiang.cn

================================================================================
来源：http://gu.shxzskj.cn

K. JSON 与序列化
来源：http://zc.shxzukj.cn

================================================================================
来源：http://mg.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://fr.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jz.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oj.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://ov.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://qt.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dn.szsharing.cn

Go:   json.Marshal(obj)
来源：http://kj.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://al.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sg.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://nw.chemitech.net.cn

Py:   json.loads(s)
来源：http://do.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qx.huanxung.cn

JS:   JSON.parse(s)
来源：http://km.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://ms.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tu.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://pi.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://af.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gw.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ji.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wr.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ry.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fu.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://og.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dx.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vg.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ld.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gs.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://oa.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vy.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ka.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bf.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://to.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uk.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xo.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bw.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ae.nicolike.cn

[K05] 深拷贝对象
来源：http://vh.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://vc.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://lo.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://hn.shxzukj.cn

TS:   structuredClone(obj)
来源：http://lg.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rp.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aj.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xu.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vt.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://tr.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vg.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://co.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hj.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dd.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vw.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nz.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qc.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ph.shtwfgs.cn

[K07] 进制转换
来源：http://qv.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ks.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ki.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vy.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zb.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zp.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xm.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ir.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wq.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://hw.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://am.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mn.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://vm.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://cz.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zu.panjiajie.cn

Go:   encoding/gob
来源：http://as.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://cg.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eb.yuexingan06.cn

================================================================================
来源：http://ar.chemitech.net.cn

L. 网络请求
来源：http://ah.haigaiapp.cn

================================================================================
来源：http://fz.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://hj.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tx.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://to.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://ub.huixiangedu.cn

TS:   await fetch(url)
来源：http://co.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ea.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://ag.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sb.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qq.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://lv.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kq.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ky.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ui.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pc.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wf.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aj.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fl.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rz.nszjky.cn

[L03] 设置自定义请求头
来源：http://pl.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wi.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xu.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yz.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vk.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xq.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ha.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fr.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vk.shxzskj.cn

[L04] 设置超时
来源：http://ef.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://lk.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wl.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ux.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ba.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xy.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ha.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jn.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ti.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://ms.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ba.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sd.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zg.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vg.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gt.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gf.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rk.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ys.newstarts.cn

[L06] 解析响应为 JSON
来源：http://qu.jctech888.com.cn

Py:   resp.json()
来源：http://me.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://ou.huixinmuqiang.cn

JS:   await resp.json()
来源：http://bl.haigaiapp.cn

TS:   await resp.json()
来源：http://ea.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://af.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kw.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://kh.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ek.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://pf.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oj.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aj.colortex.cn

JS:   resp.ok;  resp.status
来源：http://px.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://cw.colortex.cn

Java: resp.statusCode()
来源：http://ff.colortex.cn

Go:   resp.StatusCode
来源：http://hs.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://zf.colortex.cn

C#:   (int)resp.StatusCode
来源：http://mp.szxytkj.cn

[L08] 并发请求多个地址
来源：http://xf.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nd.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://uj.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ki.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://py.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dg.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oh.colortex.cn


<!-- 参考信息 -->