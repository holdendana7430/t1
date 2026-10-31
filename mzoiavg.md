代发 wailian999

[I02] 提取所有匹配
来源：http://hq.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://yh.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oc.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aa.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://cd.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oz.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wt.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://go.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mf.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://eb.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bq.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hf.haigaiapp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uj.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ek.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ps.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xm.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wf.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uy.nicolike.cn

[I04] 正则替换
来源：http://tj.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mp.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://az.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rp.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xt.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://au.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://in.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xy.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fq.szsharing.cn

[I05] 按正则拆分
来源：http://jl.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uv.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tx.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://ee.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://fe.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://ib.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qj.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://px.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bf.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yi.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sd.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://th.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yj.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ut.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wp.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rt.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hn.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yx.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://rj.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tj.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://as.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cs.bookmarksfly.cn

TS:   /error/gim
来源：http://zx.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ih.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://so.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://aa.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cf.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://rg.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xs.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ds.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wa.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wq.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lu.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zb.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wp.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fy.hahajie.cn

================================================================================
来源：http://bt.nicolike.cn

J. 日期与时间
来源：http://zy.yuexingan06.cn

================================================================================
来源：http://px.9csxet.cn

[J01] 获取当前时间
来源：http://cf.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lr.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hf.521024.cn

JS:   new Date();  Date.now()
来源：http://mg.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://gw.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bj.asd995.cn

Go:   time.Now()
来源：http://bl.muxihuayi.cn

Ruby: Time.now
来源：http://mr.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zp.muxihuayi.cn

[J02] 格式化输出
来源：http://nr.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rf.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lc.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mq.gzmigu.cn

TS:   d.toISOString()
来源：http://uf.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hl.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cr.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rv.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rb.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://lh.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nf.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jb.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://cg.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://ld.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pn.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mp.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://wv.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ss.hahajie.cn

[J04] 时间戳与日期互转
来源：http://ka.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rf.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gw.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nt.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ry.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ov.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ud.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ol.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ys.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://az.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://zp.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lk.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vg.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://km.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://sa.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ck.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://ql.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vi.nicolike.cn

[J06] 计算两时间之差
来源：http://mi.asd995.cn

Py:   (end - start).total_seconds()
来源：http://nn.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://er.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ps.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kf.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://it.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://km.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://vm.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://ti.shtwfgs.cn

[J07] 比较两个日期
来源：http://qv.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://ii.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zf.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bl.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hp.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kr.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xb.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lp.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ku.lnxyls.cn

[J08] 提取年月日与星期
来源：http://ap.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ue.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bs.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sa.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cl.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ci.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hg.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kz.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://es.haigaiapp.cn

[J09] 时区处理
来源：http://ba.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nd.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iy.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ma.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gr.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rh.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fp.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cs.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tw.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://bg.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wy.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ka.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ed.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wj.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wz.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://by.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://co.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ft.huanxung.cn

================================================================================
来源：http://jk.szxytkj.cn

K. JSON 与序列化
来源：http://xz.newstarts.cn

================================================================================
来源：http://mn.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://rx.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gt.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vf.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://uw.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://jt.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vy.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://bw.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://aq.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oq.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://xm.hnjuh.cn

Py:   json.loads(s)
来源：http://vy.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qo.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://er.asd995.cn

TS:   JSON.parse(s)
来源：http://gc.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jq.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://ed.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://yw.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ew.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://ud.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fb.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qj.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yl.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fs.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://px.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gu.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yw.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bk.colortex.cn

[K04] 读取 JSON 文件
来源：http://uk.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qg.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ll.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ot.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nl.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ef.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aj.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mz.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mw.yuexingan06.cn

[K05] 深拷贝对象
来源：http://pq.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://zb.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://wa.shxzukj.cn

JS:   structuredClone(obj)
来源：http://jx.szxytkj.cn

TS:   structuredClone(obj)
来源：http://up.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fh.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pg.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://la.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dc.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://jw.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wt.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qf.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bx.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vo.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dh.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ng.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nf.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zf.nszjky.cn

[K07] 进制转换
来源：http://eg.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wq.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://do.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gy.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ua.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://om.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gc.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xm.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aw.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://wn.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://pv.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ql.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://mw.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://ta.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ca.chemitech.net.cn

Go:   encoding/gob
来源：http://nt.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://jt.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ix.chemitech.net.cn

================================================================================
来源：http://wb.yuntaijiaju.cn

L. 网络请求
来源：http://pd.shtwfgs.cn

================================================================================
来源：http://aq.nszjky.cn

[L01] 发送 GET 请求
来源：http://rg.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wf.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zt.nszjky.cn

JS:   await fetch(url)
来源：http://gh.szxytkj.cn

TS:   await fetch(url)
来源：http://ha.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ui.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://sc.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nm.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://be.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://ck.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uz.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qp.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://we.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rt.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hk.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dr.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ls.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pj.panjiajie.cn

[L03] 设置自定义请求头
来源：http://aa.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://db.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bn.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://op.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pq.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fa.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tg.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pj.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oe.muxihuayi.cn

[L04] 设置超时
来源：http://vm.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://hh.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bh.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sy.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xj.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hp.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kl.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mv.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pq.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://ep.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iw.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qy.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ki.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cd.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wf.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ox.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wo.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tz.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://hn.asd995.cn

Py:   resp.json()
来源：http://sx.newstarts.cn

PHP:  json_decode($body, true);
来源：http://ab.521024.cn

JS:   await resp.json()
来源：http://wy.newstarts.cn

TS:   await resp.json()
来源：http://bw.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qm.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sc.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://rl.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hr.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://ei.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mw.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fx.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://gs.asd995.cn

TS:   resp.ok;  resp.status
来源：http://mz.huixiangedu.cn

Java: resp.statusCode()
来源：http://xb.9csxet.cn

Go:   resp.StatusCode
来源：http://bo.panjiajie.cn

Ruby: resp.code.to_i
来源：http://ff.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://rn.newstarts.cn

[L08] 并发请求多个地址
来源：http://wo.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nc.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://vh.szxytkj.cn


<!-- 参考信息 -->