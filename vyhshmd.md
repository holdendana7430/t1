代发 wailian999

[I02] 提取所有匹配
来源：http://zz.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://lg.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vb.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mg.asd995.cn

TS:   s.match(/\d+/g)
来源：http://se.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ct.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://in.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://lv.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bl.haigaiapp.cn

[I03] 提取捕获分组
来源：http://ew.hnjuh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bg.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vb.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jo.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nz.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qr.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gy.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mn.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://up.szxytkj.cn

[I04] 正则替换
来源：http://ce.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gr.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cc.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qb.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://md.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zp.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oq.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://op.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sg.panjiajie.cn

[I05] 按正则拆分
来源：http://ky.nszjky.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mp.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pg.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://ug.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://yp.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://mn.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cb.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ep.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bz.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sf.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fz.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zm.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bd.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gi.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ya.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bc.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ce.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://av.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://il.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hb.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wx.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kf.panjiajie.cn

TS:   /error/gim
来源：http://hx.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://df.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oj.asd995.cn

Ruby: s.scan(/error/i)
来源：http://ll.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ce.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://tx.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lo.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oi.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tt.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jf.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rx.muxihuayi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tm.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ca.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zw.gzmigu.cn

================================================================================
来源：http://bb.yuexingan06.cn

J. 日期与时间
来源：http://mq.9csxet.cn

================================================================================
来源：http://sb.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://lm.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cj.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bc.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://jy.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://nq.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gz.wgjwhj.cn

Go:   time.Now()
来源：http://kd.panjiajie.cn

Ruby: Time.now
来源：http://xy.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ds.521024.cn

[J02] 格式化输出
来源：http://nx.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wm.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://na.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rb.wgjwhj.cn

TS:   d.toISOString()
来源：http://gf.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wg.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mv.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zp.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uf.panjiajie.cn

[J03] 字符串解析为日期
来源：http://hc.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xt.hnjuh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ty.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://jn.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://nr.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kx.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ll.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://bt.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rp.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://le.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jq.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zy.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yc.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zv.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wr.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mt.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bv.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://om.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://sl.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://oo.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xe.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lh.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uk.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://km.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yz.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://sf.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kr.hnjuh.cn

[J06] 计算两时间之差
来源：http://wo.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://ss.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://jt.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://de.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mc.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uq.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://wj.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://ns.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://xf.nszjky.cn

[J07] 比较两个日期
来源：http://ks.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://fu.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ad.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ph.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ev.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://et.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pm.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rx.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://fj.hnjuh.cn

[J08] 提取年月日与星期
来源：http://fe.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kc.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://de.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rc.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://es.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jd.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hh.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://me.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ht.gzmigu.cn

[J09] 时区处理
来源：http://pt.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yk.nicolike.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dd.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oz.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eu.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dz.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gc.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ia.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pj.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://oc.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xi.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rs.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qj.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mq.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vh.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rx.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oh.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aw.yuntaijiaju.cn

================================================================================
来源：http://pc.chemitech.net.cn

K. JSON 与序列化
来源：http://lq.szxytkj.cn

================================================================================
来源：http://pq.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://gm.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://of.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ys.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://cy.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://ru.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qa.huanxung.cn

Go:   json.Marshal(obj)
来源：http://im.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hq.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pu.asd995.cn

[K02] JSON 字符串转对象
来源：http://oh.gzmigu.cn

Py:   json.loads(s)
来源：http://pf.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bg.shxzukj.cn

JS:   JSON.parse(s)
来源：http://zt.asd995.cn

TS:   JSON.parse(s)
来源：http://ll.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ix.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://md.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://kr.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jx.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://ut.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://co.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sd.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pv.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hl.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pu.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kn.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yw.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kd.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://qh.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gt.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dp.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qw.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tl.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qx.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nt.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://il.nicolike.cn

[K05] 深拷贝对象
来源：http://gv.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://kv.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://gw.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://em.panjiajie.cn

TS:   structuredClone(obj)
来源：http://sr.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ne.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ri.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uf.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://du.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://qv.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xf.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qb.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zj.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bz.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rd.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ut.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hp.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kh.colortex.cn

[K07] 进制转换
来源：http://ix.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wi.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yu.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pk.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ce.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pp.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ur.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jh.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sg.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://py.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://uy.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pr.szsharing.cn

JS:   v8.serialize(obj)        // Node
来源：http://ud.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://ro.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://te.lnxyls.cn

Go:   encoding/gob
来源：http://dq.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://az.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xm.gzmigu.cn

================================================================================
来源：http://sx.nszjky.cn

L. 网络请求
来源：http://wk.bookmarksfly.cn

================================================================================
来源：http://qd.nicolike.cn

[L01] 发送 GET 请求
来源：http://nu.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tw.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qe.wgjwhj.cn

JS:   await fetch(url)
来源：http://ok.bjjhwx.cn

TS:   await fetch(url)
来源：http://tg.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sx.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://ta.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cb.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xs.hnjuh.cn

[L02] 发送 POST JSON
来源：http://wb.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bb.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yv.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://op.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ho.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ff.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vo.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://px.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zu.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://yg.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nz.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nx.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nw.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qi.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://in.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ed.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zl.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jk.haigaiapp.cn

[L04] 设置超时
来源：http://rb.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://ej.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yj.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gy.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ed.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ll.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iw.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oh.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sw.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://io.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://it.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xh.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uc.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rn.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ip.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ek.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xn.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://od.huanxung.cn

[L06] 解析响应为 JSON
来源：http://rl.muxihuayi.cn

Py:   resp.json()
来源：http://oo.hahajie.cn

PHP:  json_decode($body, true);
来源：http://pn.huixinmuqiang.cn

JS:   await resp.json()
来源：http://dt.bjjhwx.cn

TS:   await resp.json()
来源：http://qh.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ay.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lx.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://eb.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qf.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://fy.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ia.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gf.colortex.cn

JS:   resp.ok;  resp.status
来源：http://ev.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://xz.haigaiapp.cn

Java: resp.statusCode()
来源：http://ww.lnxyls.cn

Go:   resp.StatusCode
来源：http://wr.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://sz.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://xp.szxytkj.cn

[L08] 并发请求多个地址
来源：http://lq.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://si.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://lo.gzmigu.cn


<!-- 参考信息 -->