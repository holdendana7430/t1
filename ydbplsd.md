代发 wailian999

[I02] 提取所有匹配
来源：http://iu.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://nb.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zu.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://up.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://qx.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jw.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yh.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://pp.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fb.huixiangedu.cn

[I03] 提取捕获分组
来源：http://bw.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yg.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nz.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qz.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vk.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://du.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lg.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ca.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cm.bjjhwx.cn

[I04] 正则替换
来源：http://av.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ff.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nj.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dj.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wf.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cp.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jv.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gl.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yi.asd995.cn

[I05] 按正则拆分
来源：http://pe.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gw.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://co.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://st.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://rs.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://lx.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vr.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rh.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ah.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tm.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oz.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jz.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yb.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ka.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rc.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bn.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fr.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fo.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://gz.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://no.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lj.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://le.haigaiapp.cn

TS:   /error/gim
来源：http://yh.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kd.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ys.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://bv.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wn.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://oa.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wk.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eo.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ow.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ei.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sa.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vj.szxytkj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lw.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xq.huanxung.cn

================================================================================
来源：http://qb.shxzukj.cn

J. 日期与时间
来源：http://zq.szxytkj.cn

================================================================================
来源：http://hf.chemitech.net.cn

[J01] 获取当前时间
来源：http://jj.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ps.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://cj.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://xe.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xd.yuntaijiaju.cn

Go:   time.Now()
来源：http://ha.gzmigu.cn

Ruby: Time.now
来源：http://fe.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xx.yuntaijiaju.cn

[J02] 格式化输出
来源：http://un.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hx.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jy.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lv.newstarts.cn

TS:   d.toISOString()
来源：http://ah.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ru.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mn.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://id.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eu.szxytkj.cn

[J03] 字符串解析为日期
来源：http://wy.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yx.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gc.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://sr.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://ib.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qs.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yw.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://fq.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oh.nicolike.cn

[J04] 时间戳与日期互转
来源：http://cq.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ly.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vv.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ki.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mx.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xl.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ug.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mh.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uq.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://ne.colortex.cn

Py:   now + timedelta(days=7)
来源：http://xr.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gu.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://an.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fe.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://hs.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iq.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://am.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jm.szxytkj.cn

[J06] 计算两时间之差
来源：http://ug.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://qv.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://ew.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ff.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rv.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pa.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://om.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://zb.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://vs.panjiajie.cn

[J07] 比较两个日期
来源：http://co.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://ck.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ii.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jj.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qc.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qv.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yk.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vr.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://ry.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://mr.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bc.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ik.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kt.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://is.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://px.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://it.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bz.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qi.huixiangedu.cn

[J09] 时区处理
来源：http://lm.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ku.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ti.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ga.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bp.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kc.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ny.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kj.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://li.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://vh.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sw.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dx.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ns.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yb.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ik.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sl.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jv.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sg.bookmarksfly.cn

================================================================================
来源：http://lj.shtwfgs.cn

K. JSON 与序列化
来源：http://ky.huixinmuqiang.cn

================================================================================
来源：http://dn.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://ce.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xw.gzmigu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uz.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://mn.colortex.cn

TS:   JSON.stringify(obj)
来源：http://gw.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vk.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://ie.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://on.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bh.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://gg.jctech888.com.cn

Py:   json.loads(s)
来源：http://nk.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iw.gzmigu.cn

JS:   JSON.parse(s)
来源：http://rn.hahajie.cn

TS:   JSON.parse(s)
来源：http://fs.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xu.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://bw.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://cn.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pf.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://rh.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lg.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://up.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yu.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tl.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gk.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ik.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pm.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ry.newstarts.cn

[K04] 读取 JSON 文件
来源：http://ud.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ow.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jc.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qj.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ol.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gv.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oo.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lz.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://se.shxzskj.cn

[K05] 深拷贝对象
来源：http://ro.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://ok.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://wu.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://xq.shxzskj.cn

TS:   structuredClone(obj)
来源：http://wj.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gx.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://by.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wb.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mf.nicolike.cn

[K06] 解析 URL 查询串
来源：http://vs.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://et.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mg.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eb.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sb.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qn.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mt.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tr.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xo.szxytkj.cn

[K07] 进制转换
来源：http://au.panjiajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zb.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cz.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://an.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cp.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bp.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nm.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cj.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aj.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://mn.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://xi.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://be.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://wr.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://bb.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yh.shxzskj.cn

Go:   encoding/gob
来源：http://li.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://an.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mv.hnjuh.cn

================================================================================
来源：http://ht.yuntaijiaju.cn

L. 网络请求
来源：http://yp.521024.cn

================================================================================
来源：http://tf.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://hu.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ek.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ql.bookmarksfly.cn

JS:   await fetch(url)
来源：http://al.huixiangedu.cn

TS:   await fetch(url)
来源：http://st.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nv.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://vv.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://go.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pw.panjiajie.cn

[L02] 发送 POST JSON
来源：http://yb.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rp.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kj.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cv.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dl.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kn.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bg.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nn.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qt.szsharing.cn

[L03] 设置自定义请求头
来源：http://pw.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fa.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xb.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bx.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dd.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lc.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wy.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cc.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qa.shxzskj.cn

[L04] 设置超时
来源：http://uo.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://td.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rs.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bn.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ki.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gy.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vr.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ip.yuntaijiaju.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bh.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://pv.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lr.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lc.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oi.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tb.nszjky.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lx.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://we.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ix.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sw.nszjky.cn

[L06] 解析响应为 JSON
来源：http://dz.jianghongdianzi.cn

Py:   resp.json()
来源：http://bm.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://sz.huixinmuqiang.cn

JS:   await resp.json()
来源：http://xm.jianghongdianzi.cn

TS:   await resp.json()
来源：http://pq.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pa.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iy.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://cc.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oj.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://oo.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://au.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xw.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://vd.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://bx.yuexingan06.cn

Java: resp.statusCode()
来源：http://qp.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://qc.huanxung.cn

Ruby: resp.code.to_i
来源：http://is.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://rv.newstarts.cn

[L08] 并发请求多个地址
来源：http://dt.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fe.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://ua.bookmarksfly.cn


<!-- 参考信息 -->