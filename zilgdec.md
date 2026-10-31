代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kj.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rm.521024.cn

JS:   /\d+/.test(s)
来源：http://uk.9csxet.cn

TS:   /\d+/.test(s)
来源：http://xm.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://et.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gu.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://jt.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://at.huanxung.cn

[I02] 提取所有匹配
来源：http://kl.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://kt.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tm.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bh.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://mo.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ix.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gn.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://ic.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://et.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://nu.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dg.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lb.haigaiapp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qf.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tx.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://od.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bf.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ac.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qr.9csxet.cn

[I04] 正则替换
来源：http://hw.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kl.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mb.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bj.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jw.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zq.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fr.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fb.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fw.gzmigu.cn

[I05] 按正则拆分
来源：http://tv.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ou.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fs.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://nt.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://xr.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://kh.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oo.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fl.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zn.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://td.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://go.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hq.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wb.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nn.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ts.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vk.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mf.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sn.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://af.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ft.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wa.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fw.szsharing.cn

TS:   /error/gim
来源：http://ee.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gi.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hv.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://xk.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tg.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://re.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ug.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://za.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bz.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qb.huanxung.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zy.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ff.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xy.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qb.jianghongdianzi.cn

================================================================================
来源：http://qg.bjjhwx.cn

J. 日期与时间
来源：http://mt.newstarts.cn

================================================================================
来源：http://nt.jctech888.com.cn

[J01] 获取当前时间
来源：http://jm.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yi.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://po.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://sj.nszjky.cn

TS:   new Date();  Date.now()
来源：http://ai.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vs.bookmarksfly.cn

Go:   time.Now()
来源：http://ja.panjiajie.cn

Ruby: Time.now
来源：http://ej.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ax.szsharing.cn

[J02] 格式化输出
来源：http://he.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://no.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jw.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wl.chemitech.net.cn

TS:   d.toISOString()
来源：http://oi.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pt.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ex.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kw.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hx.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://jl.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yi.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bj.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://ik.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://qt.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bj.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kz.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://gx.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nd.hahajie.cn

[J04] 时间戳与日期互转
来源：http://ha.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gz.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zs.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yz.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fg.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ml.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vc.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yq.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uq.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://dq.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://ho.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jw.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qa.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ym.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://im.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://op.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://hi.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tm.szsharing.cn

[J06] 计算两时间之差
来源：http://fm.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://ai.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://ai.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kl.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ok.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gc.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://cc.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://rp.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://om.9csxet.cn

[J07] 比较两个日期
来源：http://vt.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://tt.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://km.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vc.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pc.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ub.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ab.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lq.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://rm.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://gz.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ff.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://po.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lw.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hr.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sf.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gt.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eh.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ox.newstarts.cn

[J09] 时区处理
来源：http://ws.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vf.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qc.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oo.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tu.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bc.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ew.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kj.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bv.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://mk.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ur.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hs.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hr.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pp.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gv.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ra.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hy.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uk.shxzukj.cn

================================================================================
来源：http://gn.szxytkj.cn

K. JSON 与序列化
来源：http://gu.521024.cn

================================================================================
来源：http://nl.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://ji.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hp.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://li.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://cp.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://nn.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uy.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://jx.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cn.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sz.hahajie.cn

[K02] JSON 字符串转对象
来源：http://fj.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://jq.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rv.hahajie.cn

JS:   JSON.parse(s)
来源：http://sl.panjiajie.cn

TS:   JSON.parse(s)
来源：http://zh.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dp.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://ai.nszjky.cn

Ruby: JSON.parse(s)
来源：http://pr.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jb.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://hi.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jr.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ln.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://aa.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bd.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cc.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ui.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jg.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://er.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://vi.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://md.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tb.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fx.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bu.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qf.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xi.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ow.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oo.gzmigu.cn

[K05] 深拷贝对象
来源：http://mr.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://qi.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://pj.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://rc.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://pp.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rk.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://st.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qx.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bv.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://hz.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dk.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cr.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pf.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ve.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://do.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://al.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hv.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hg.hahajie.cn

[K07] 进制转换
来源：http://qj.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rb.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://da.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rx.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ma.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ex.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://as.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oc.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qk.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://pf.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://hs.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://he.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://dj.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://rh.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vu.szxytkj.cn

Go:   encoding/gob
来源：http://it.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://ls.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nh.jctech888.com.cn

================================================================================
来源：http://cy.shxzskj.cn

L. 网络请求
来源：http://sm.huixiangedu.cn

================================================================================
来源：http://ow.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://wy.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ki.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qm.szxytkj.cn

JS:   await fetch(url)
来源：http://ii.nicolike.cn

TS:   await fetch(url)
来源：http://wt.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mw.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://zp.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hs.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ns.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://ur.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tl.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://im.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iw.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://id.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ti.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gv.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vf.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oh.nszjky.cn

[L03] 设置自定义请求头
来源：http://lx.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lh.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ez.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pn.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://om.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nf.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nr.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pt.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://az.nszjky.cn

[L04] 设置超时
来源：http://yx.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://sv.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://df.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ac.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://de.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tw.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://er.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lk.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ji.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://pi.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gj.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yo.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yw.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hd.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iw.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://je.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bo.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uh.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://jn.newstarts.cn

Py:   resp.json()
来源：http://nk.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://el.hahajie.cn

JS:   await resp.json()
来源：http://if.nszjky.cn

TS:   await resp.json()
来源：http://em.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rn.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ls.asd995.cn

Ruby: JSON.parse(resp.body)
来源：http://qo.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tm.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://bo.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oc.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ut.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://js.jianghongdianzi.cn


<!-- 参考信息 -->