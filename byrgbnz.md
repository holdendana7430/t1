代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dn.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://po.nicolike.cn

JS:   /\d+/.test(s)
来源：http://xz.szsharing.cn

TS:   /\d+/.test(s)
来源：http://wz.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eh.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://te.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://oz.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ax.yuexingan06.cn

[I02] 提取所有匹配
来源：http://fv.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://bl.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zs.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rw.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://ne.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://od.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kw.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://ph.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yf.szxytkj.cn

[I03] 提取捕获分组
来源：http://pz.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xg.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lb.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gr.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nu.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sk.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xu.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ra.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ke.bookmarksfly.cn

[I04] 正则替换
来源：http://ew.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bp.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rd.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ae.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mo.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nn.yuntaijiaju.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wi.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jx.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cl.jctech888.com.cn

[I05] 按正则拆分
来源：http://qc.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wl.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kj.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://wn.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://fy.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://tf.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dy.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gc.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bv.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wn.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vg.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mz.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vi.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ib.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jy.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qj.haigaiapp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ei.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dq.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://ds.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jq.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lp.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fa.shxzukj.cn

TS:   /error/gim
来源：http://er.yuexingan06.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bq.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ai.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://tx.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yx.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://bd.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xo.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ep.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://la.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://km.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ns.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jp.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xl.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://st.shtwfgs.cn

================================================================================
来源：http://nw.hnjuh.cn

J. 日期与时间
来源：http://ad.lnxyls.cn

================================================================================
来源：http://yy.muxihuayi.cn

[J01] 获取当前时间
来源：http://dl.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://iq.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gw.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://sy.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://mw.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qd.jctech888.com.cn

Go:   time.Now()
来源：http://ma.newstarts.cn

Ruby: Time.now
来源：http://pn.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zh.colortex.cn

[J02] 格式化输出
来源：http://jn.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ng.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gr.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://st.jctech888.com.cn

TS:   d.toISOString()
来源：http://st.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zr.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ps.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vz.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gu.szxytkj.cn

[J03] 字符串解析为日期
来源：http://ds.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lj.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zs.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://se.asd995.cn

TS:   new Date("2024-01-02")
来源：http://xt.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hp.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nf.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://fk.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kb.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://qo.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ki.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qa.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cp.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xg.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ot.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dc.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yw.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kg.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://xb.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://tg.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bu.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sz.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gk.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://oo.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vh.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://qy.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rk.szsharing.cn

[J06] 计算两时间之差
来源：http://xe.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://uu.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://ly.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://af.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tf.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pq.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://sh.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://fv.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://vc.gzmigu.cn

[J07] 比较两个日期
来源：http://pp.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://sz.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hs.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qj.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uk.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mz.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nt.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sf.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://nt.shxzukj.cn

[J08] 提取年月日与星期
来源：http://ky.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://on.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ko.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uw.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nx.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xy.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ht.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pa.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vl.huanxung.cn

[J09] 时区处理
来源：http://bv.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mp.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dc.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cd.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ap.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bn.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dn.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vw.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ns.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://cc.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rb.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vf.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ld.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uj.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bt.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fk.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fc.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cl.nszjky.cn

================================================================================
来源：http://cc.panjiajie.cn

K. JSON 与序列化
来源：http://nn.nszjky.cn

================================================================================
来源：http://zg.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://nr.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fv.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gu.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://fg.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://ia.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sz.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://mx.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ow.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hn.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://kp.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://fe.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fr.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://of.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://ii.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://co.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://rx.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://ug.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ol.bookmarksfly.cn

[K03] JSON 美化输出（带缩进）
来源：http://zr.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ts.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lc.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gt.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kw.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iu.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ku.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vy.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nh.hahajie.cn

[K04] 读取 JSON 文件
来源：http://yy.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cm.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gf.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kh.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gy.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://og.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ad.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sl.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://se.shtwfgs.cn

[K05] 深拷贝对象
来源：http://tm.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://tl.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://zy.9csxet.cn

JS:   structuredClone(obj)
来源：http://st.shxzskj.cn

TS:   structuredClone(obj)
来源：http://qi.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://es.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://at.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rc.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uk.yuexingan06.cn

[K06] 解析 URL 查询串
来源：http://jn.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bf.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qz.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ns.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wr.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wv.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ir.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ga.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oz.nszjky.cn

[K07] 进制转换
来源：http://hq.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zh.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rf.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gx.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oy.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xv.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lg.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qw.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nm.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://no.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://qi.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gw.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://pp.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://gw.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bj.gzmigu.cn

Go:   encoding/gob
来源：http://lc.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://bc.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rv.shtwfgs.cn

================================================================================
来源：http://na.panjiajie.cn

L. 网络请求
来源：http://hm.shxzskj.cn

================================================================================
来源：http://xs.panjiajie.cn

[L01] 发送 GET 请求
来源：http://pp.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://et.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cg.hahajie.cn

JS:   await fetch(url)
来源：http://vc.haigaiapp.cn

TS:   await fetch(url)
来源：http://le.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://on.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://xa.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wr.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://na.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://xu.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://li.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fr.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nd.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jp.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hy.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vu.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cg.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://re.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://wh.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ns.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ge.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gf.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qx.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ka.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://it.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hg.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pk.shtwfgs.cn

[L04] 设置超时
来源：http://nf.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://zj.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kg.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://br.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eb.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rx.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xk.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pn.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gf.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://gf.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zz.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hh.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tv.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mv.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://in.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sc.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wy.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rk.colortex.cn

[L06] 解析响应为 JSON
来源：http://me.wgjwhj.cn

Py:   resp.json()
来源：http://pl.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://dh.newstarts.cn

JS:   await resp.json()
来源：http://nf.yuntaijiaju.cn

TS:   await resp.json()
来源：http://bo.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mt.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xw.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://ph.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rw.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://sy.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xy.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iw.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://zy.newstarts.cn


<!-- 参考信息 -->