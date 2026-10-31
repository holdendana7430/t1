代发 wailian999

[I02] 提取所有匹配
来源：http://tv.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://wt.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wi.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fm.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://np.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://st.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zi.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://mx.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ca.shxzukj.cn

[I03] 提取捕获分组
来源：http://mg.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://om.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tc.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nk.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yn.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hk.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rg.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kt.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hh.muxihuayi.cn

[I04] 正则替换
来源：http://fj.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tz.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nh.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sb.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hr.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pz.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dy.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bj.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://me.nszjky.cn

[I05] 按正则拆分
来源：http://ch.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://so.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://et.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://qn.chemitech.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://af.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://lm.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ab.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tt.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ot.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ba.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wg.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gn.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ca.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://si.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://df.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tg.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nq.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uv.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://mv.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qe.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vh.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://se.bjjhwx.cn

TS:   /error/gim
来源：http://uz.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cn.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ya.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://jf.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://am.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://cl.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dv.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://al.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://up.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zs.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zx.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kz.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yp.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fq.huanxung.cn

================================================================================
来源：http://xc.hahajie.cn

J. 日期与时间
来源：http://ya.huixiangedu.cn

================================================================================
来源：http://rk.panjiajie.cn

[J01] 获取当前时间
来源：http://iu.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gi.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ot.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://ag.asd995.cn

TS:   new Date();  Date.now()
来源：http://yc.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://du.yuexingan06.cn

Go:   time.Now()
来源：http://dr.huixiangedu.cn

Ruby: Time.now
来源：http://ms.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ye.hnjuh.cn

[J02] 格式化输出
来源：http://fc.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qn.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ri.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ew.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://dq.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ko.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dr.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lt.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jr.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://ah.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ot.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ff.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://pp.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://ks.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dj.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xb.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://in.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://be.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://lm.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jr.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vz.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ov.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bu.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qw.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://op.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ni.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pw.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://ie.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://mh.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vo.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uf.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sr.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://mc.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cx.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://jl.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pg.bjjhwx.cn

[J06] 计算两时间之差
来源：http://pc.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://zd.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://tj.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jz.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://im.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cc.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://jq.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://po.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://dj.9csxet.cn

[J07] 比较两个日期
来源：http://ew.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://sa.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://in.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xw.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vb.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qv.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ug.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://eh.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://gw.colortex.cn

[J08] 提取年月日与星期
来源：http://vz.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ia.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sd.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yb.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jl.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pe.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xi.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ei.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uz.shxzukj.cn

[J09] 时区处理
来源：http://rf.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lw.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dp.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://le.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iv.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yl.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vy.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ud.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rl.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://wj.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hq.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dt.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ov.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pr.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pn.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sf.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jf.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yuntaijiaju.cn

================================================================================
来源：http://qt.hnjuh.cn

K. JSON 与序列化
来源：http://mc.wgjwhj.cn

================================================================================
来源：http://az.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://we.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qx.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sw.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://ri.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://mp.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yg.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://of.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pm.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gq.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://vi.hnjuh.cn

Py:   json.loads(s)
来源：http://hj.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ut.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://ic.panjiajie.cn

TS:   JSON.parse(s)
来源：http://ly.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://su.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://cq.huanxung.cn

Ruby: JSON.parse(s)
来源：http://iu.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sh.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://er.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yk.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iu.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ex.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ds.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sd.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qa.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nj.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dm.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://dw.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qw.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jo.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yr.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mj.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ef.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fb.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ko.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xy.szsharing.cn

[K05] 深拷贝对象
来源：http://sq.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://kk.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://rv.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://hl.lnxyls.cn

TS:   structuredClone(obj)
来源：http://be.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tb.hnjuh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sp.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cp.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qy.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://iu.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jv.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tu.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ex.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jf.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eb.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mq.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qh.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ox.shxzskj.cn

[K07] 进制转换
来源：http://on.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cm.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://io.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cq.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rp.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fh.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xr.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pz.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://do.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://bp.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://lc.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sc.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://oh.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://ai.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://el.wgjwhj.cn

Go:   encoding/gob
来源：http://wi.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://rh.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jb.yuexingan06.cn

================================================================================
来源：http://rl.shxzukj.cn

L. 网络请求
来源：http://nd.huixiangedu.cn

================================================================================
来源：http://vj.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://jb.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sh.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qy.huanxung.cn

JS:   await fetch(url)
来源：http://sz.bjjhwx.cn

TS:   await fetch(url)
来源：http://ok.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fl.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://rs.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wm.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ea.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://ka.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tp.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ez.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://za.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qr.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oz.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mg.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ks.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wu.521024.cn

[L03] 设置自定义请求头
来源：http://rm.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ym.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gs.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rw.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sh.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lj.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pb.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ak.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jd.szxytkj.cn

[L04] 设置超时
来源：http://cx.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://el.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jo.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gt.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://we.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ii.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pn.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ws.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jn.huanxung.cn

[L05] 上传文件（multipart）
来源：http://sy.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fh.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jy.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xh.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vj.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gm.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sg.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xx.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://av.521024.cn

[L06] 解析响应为 JSON
来源：http://nw.asd995.cn

Py:   resp.json()
来源：http://os.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://rl.szsharing.cn

JS:   await resp.json()
来源：http://gs.colortex.cn

TS:   await resp.json()
来源：http://nq.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xi.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://um.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://fd.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qx.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://ug.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ni.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xd.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://cx.asd995.cn

TS:   resp.ok;  resp.status
来源：http://rj.hnjuh.cn

Java: resp.statusCode()
来源：http://vk.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://pl.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://hb.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://fn.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://jj.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uh.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://vv.szsharing.cn


<!-- 参考信息 -->