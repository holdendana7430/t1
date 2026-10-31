代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mx.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://li.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://zg.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pa.huixiangedu.cn

[I02] 提取所有匹配
来源：http://ak.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://kw.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vh.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cr.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://zv.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wq.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tp.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://jd.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kj.haigaiapp.cn

[I03] 提取捕获分组
来源：http://mh.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jv.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fa.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tl.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yh.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dd.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ls.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vv.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cq.colortex.cn

[I04] 正则替换
来源：http://np.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://eh.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bo.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ap.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rb.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xy.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dk.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ma.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eu.haigaiapp.cn

[I05] 按正则拆分
来源：http://oj.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kl.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vp.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ym.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://sf.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://ch.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://he.nicolike.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ts.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nk.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kv.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bw.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aw.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ud.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fv.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xj.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ex.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gp.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fc.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://ni.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://id.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://as.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oc.nicolike.cn

TS:   /error/gim
来源：http://zu.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://da.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gc.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://qi.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bb.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://hf.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jn.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zk.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aa.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ey.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://od.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zk.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lg.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zt.hahajie.cn

================================================================================
来源：http://tf.newstarts.cn

J. 日期与时间
来源：http://vn.521024.cn

================================================================================
来源：http://al.nicolike.cn

[J01] 获取当前时间
来源：http://dc.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yd.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ly.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://ki.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://dj.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yz.gzmigu.cn

Go:   time.Now()
来源：http://lu.521024.cn

Ruby: Time.now
来源：http://yu.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ai.yuexingan06.cn

[J02] 格式化输出
来源：http://qj.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ad.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ti.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ak.nicolike.cn

TS:   d.toISOString()
来源：http://jh.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tu.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ld.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vm.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jh.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://fv.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rh.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ui.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://uv.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://vr.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yp.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://at.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://np.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uv.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://tp.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jp.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tx.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ta.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fn.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jt.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cs.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://is.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aa.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://eh.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://de.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fu.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jc.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yq.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://zg.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://we.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://cg.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://do.shtwfgs.cn

[J06] 计算两时间之差
来源：http://fd.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://gd.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://ud.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wf.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rx.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oj.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://xs.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://ft.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://vt.shxzukj.cn

[J07] 比较两个日期
来源：http://qg.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://yf.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nd.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wm.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xk.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ct.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xu.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fj.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://qt.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://cl.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tw.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ve.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xg.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qx.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qa.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qn.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lf.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lf.asd995.cn

[J09] 时区处理
来源：http://fq.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pn.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qh.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ja.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ur.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uh.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pi.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xy.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wj.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://ls.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://it.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pe.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://we.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bi.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wb.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dx.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cs.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qi.shtwfgs.cn

================================================================================
来源：http://mr.lnxyls.cn

K. JSON 与序列化
来源：http://ai.nszjky.cn

================================================================================
来源：http://sw.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://tz.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yr.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wt.521024.cn

JS:   JSON.stringify(obj)
来源：http://qe.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://en.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iv.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://km.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://em.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cy.colortex.cn

[K02] JSON 字符串转对象
来源：http://ar.shxzskj.cn

Py:   json.loads(s)
来源：http://po.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ky.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://ww.shxzukj.cn

TS:   JSON.parse(s)
来源：http://le.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yl.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://ky.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://nl.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ow.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://cw.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wg.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ui.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://eq.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://np.yuntaijiaju.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dr.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vo.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xv.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mu.newstarts.cn

[K04] 读取 JSON 文件
来源：http://zn.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bi.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vq.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yw.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wr.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lr.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ei.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kc.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kx.newstarts.cn

[K05] 深拷贝对象
来源：http://ik.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://oc.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://dt.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://os.huanxung.cn

TS:   structuredClone(obj)
来源：http://hf.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://to.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ij.9csxet.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zr.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mm.9csxet.cn

[K06] 解析 URL 查询串
来源：http://ja.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ik.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sq.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lw.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jf.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ds.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hd.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dp.huixiangedu.cn

[K07] 进制转换
来源：http://km.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cv.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cf.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ew.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ji.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gv.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pm.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oc.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ag.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://pv.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://dt.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tg.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://gz.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://if.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yd.panjiajie.cn

Go:   encoding/gob
来源：http://da.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://fk.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://al.9csxet.cn

================================================================================
来源：http://hk.panjiajie.cn

L. 网络请求
来源：http://cc.huixiangedu.cn

================================================================================
来源：http://lq.hahajie.cn

[L01] 发送 GET 请求
来源：http://ws.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uy.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mb.jctech888.com.cn

JS:   await fetch(url)
来源：http://jo.yuexingan06.cn

TS:   await fetch(url)
来源：http://ti.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ol.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://fj.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kk.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zy.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://ng.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mk.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dq.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nk.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lb.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vw.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kr.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ow.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tm.szsharing.cn

[L03] 设置自定义请求头
来源：http://qf.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wv.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uz.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tg.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sb.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ij.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://es.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ie.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sm.huixinmuqiang.cn

[L04] 设置超时
来源：http://ny.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://er.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ld.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gq.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aa.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://um.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ai.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ah.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wl.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://el.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gn.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bn.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bj.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xw.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zu.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sm.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ql.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hf.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://oy.wgjwhj.cn

Py:   resp.json()
来源：http://ai.nicolike.cn

PHP:  json_decode($body, true);
来源：http://jo.asd995.cn

JS:   await resp.json()
来源：http://wn.huixiangedu.cn

TS:   await resp.json()
来源：http://nc.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ys.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ir.asd995.cn

Ruby: JSON.parse(resp.body)
来源：http://qa.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ox.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://rs.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ym.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://az.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://xu.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://vp.newstarts.cn

Java: resp.statusCode()
来源：http://az.muxihuayi.cn

Go:   resp.StatusCode
来源：http://ef.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://za.521024.cn


<!-- 参考信息 -->