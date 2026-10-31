代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iu.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kk.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://ts.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bl.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://bf.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://tw.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xs.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://as.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://ha.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qm.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://an.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://vf.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ql.chemitech.net.cn

[I03] 提取捕获分组
来源：http://vb.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://am.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tv.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fr.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nk.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pc.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lj.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xy.muxihuayi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tg.szsharing.cn

[I04] 正则替换
来源：http://gr.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://aw.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ya.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mj.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mn.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://re.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fv.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lo.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xz.521024.cn

[I05] 按正则拆分
来源：http://xo.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ox.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uz.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://ek.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://ew.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://bu.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qe.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hy.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ck.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ft.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nx.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wh.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rk.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wa.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://an.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pz.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zl.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ui.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://ol.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://me.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xm.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ax.lnxyls.cn

TS:   /error/gim
来源：http://di.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kr.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qr.521024.cn

Ruby: s.scan(/error/i)
来源：http://gd.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vz.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://dy.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sb.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xq.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xu.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ml.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ee.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dr.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dk.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bj.jctech888.com.cn

================================================================================
来源：http://ol.521024.cn

J. 日期与时间
来源：http://az.9csxet.cn

================================================================================
来源：http://ze.hahajie.cn

[J01] 获取当前时间
来源：http://tp.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qh.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://da.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://yp.nszjky.cn

TS:   new Date();  Date.now()
来源：http://yc.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lv.wgjwhj.cn

Go:   time.Now()
来源：http://um.shxzukj.cn

Ruby: Time.now
来源：http://aj.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cu.huanxung.cn

[J02] 格式化输出
来源：http://vt.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sa.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rj.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hr.bookmarksfly.cn

TS:   d.toISOString()
来源：http://yo.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hl.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://av.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ox.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vs.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://rn.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ne.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ab.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://qm.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://nr.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://as.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oi.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://jr.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ss.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://hg.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bi.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://td.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sr.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lf.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yc.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vi.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xx.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mh.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://wt.asd995.cn

Py:   now + timedelta(days=7)
来源：http://kz.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yr.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pa.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ir.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://rv.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://if.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://dl.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dj.panjiajie.cn

[J06] 计算两时间之差
来源：http://uw.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://iv.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://ka.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yy.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pa.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xb.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://di.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://kf.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://zr.gzmigu.cn

[J07] 比较两个日期
来源：http://pv.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://jk.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://do.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rs.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jc.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ly.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ef.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ob.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://ip.9csxet.cn

[J08] 提取年月日与星期
来源：http://vh.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gi.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ks.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jg.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://an.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mc.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gw.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ug.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ql.nszjky.cn

[J09] 时区处理
来源：http://xt.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mj.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lj.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rn.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zv.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mz.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zu.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://be.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fh.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://fr.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bu.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gb.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sd.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://py.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://aa.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pz.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iw.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ox.jctech888.com.cn

================================================================================
来源：http://jz.haigaiapp.cn

K. JSON 与序列化
来源：http://pz.nicolike.cn

================================================================================
来源：http://ph.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://nj.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cw.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hk.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://ee.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://ah.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ji.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://ax.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ix.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yw.asd995.cn

[K02] JSON 字符串转对象
来源：http://va.huanxung.cn

Py:   json.loads(s)
来源：http://ig.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zu.szxytkj.cn

JS:   JSON.parse(s)
来源：http://jh.colortex.cn

TS:   JSON.parse(s)
来源：http://qy.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qn.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://aw.asd995.cn

Ruby: JSON.parse(s)
来源：http://yy.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wd.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://kl.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fw.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pm.jianghongdianzi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yl.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xo.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kz.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ai.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qa.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cj.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://hn.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qk.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wn.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kr.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xm.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rs.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yo.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jm.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mk.szsharing.cn

[K05] 深拷贝对象
来源：http://mi.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://nv.lnxyls.cn

PHP:  unserialize(serialize($obj));
来源：http://et.lnxyls.cn

JS:   structuredClone(obj)
来源：http://sw.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://bt.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qc.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pq.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://st.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nm.nszjky.cn

[K06] 解析 URL 查询串
来源：http://mu.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vs.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lt.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fs.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nl.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://at.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fj.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xo.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ol.bjjhwx.cn

[K07] 进制转换
来源：http://bc.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ry.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zr.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ac.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wd.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ud.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jy.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gm.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yj.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://ik.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://ls.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yw.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://et.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://gx.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lz.jianghongdianzi.cn

Go:   encoding/gob
来源：http://vs.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://jx.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ey.9csxet.cn

================================================================================
来源：http://kx.hahajie.cn

L. 网络请求
来源：http://tr.huanxung.cn

================================================================================
来源：http://zu.huixinmuqiang.cn

[L01] 发送 GET 请求
来源：http://bi.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nu.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ow.szxytkj.cn

JS:   await fetch(url)
来源：http://ar.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://va.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tp.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://mx.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xj.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tg.asd995.cn

[L02] 发送 POST JSON
来源：http://ex.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ob.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zv.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qs.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hg.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ak.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cx.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vx.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zk.colortex.cn

[L03] 设置自定义请求头
来源：http://nt.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lm.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nb.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zm.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://of.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lw.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ou.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ir.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yn.chemitech.net.cn

[L04] 设置超时
来源：http://xr.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://mw.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ap.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ux.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vo.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oc.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nc.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lb.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wh.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://zs.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yo.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yb.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dm.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mk.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://az.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gh.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sr.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ca.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://pj.panjiajie.cn

Py:   resp.json()
来源：http://wk.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://dg.jianghongdianzi.cn

JS:   await resp.json()
来源：http://ka.bjjhwx.cn

TS:   await resp.json()
来源：http://qk.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yj.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lr.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://sz.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://si.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://hq.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zx.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fl.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://lh.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://hr.bjjhwx.cn

Java: resp.statusCode()
来源：http://on.chemitech.net.cn

Go:   resp.StatusCode
来源：http://qk.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://oc.9csxet.cn


<!-- 参考信息 -->