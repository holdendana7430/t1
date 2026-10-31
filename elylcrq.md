代发 wailian999

[I02] 提取所有匹配
来源：http://mv.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://qi.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vu.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xd.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://qo.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pk.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nz.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://pc.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nu.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://sn.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yv.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qj.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://it.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xb.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zj.wgjwhj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kr.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kg.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ng.9csxet.cn

[I04] 正则替换
来源：http://kx.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mf.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zn.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ak.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://km.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qx.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ys.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pz.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gd.nszjky.cn

[I05] 按正则拆分
来源：http://sx.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hf.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kx.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://oj.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://it.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://cx.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yh.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://iw.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yu.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gu.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ni.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cp.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ox.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mx.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fn.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vs.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mf.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ad.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://px.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://by.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://os.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uc.muxihuayi.cn

TS:   /error/gim
来源：http://np.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gp.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xm.colortex.cn

Ruby: s.scan(/error/i)
来源：http://kz.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uk.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://gc.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sq.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wc.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ez.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yu.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vj.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://em.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ww.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://er.shxzukj.cn

================================================================================
来源：http://nn.nicolike.cn

J. 日期与时间
来源：http://ky.shxzskj.cn

================================================================================
来源：http://si.szsharing.cn

[J01] 获取当前时间
来源：http://sf.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ff.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ld.newstarts.cn

JS:   new Date();  Date.now()
来源：http://su.521024.cn

TS:   new Date();  Date.now()
来源：http://nx.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nm.wgjwhj.cn

Go:   time.Now()
来源：http://xd.colortex.cn

Ruby: Time.now
来源：http://eb.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hf.hnjuh.cn

[J02] 格式化输出
来源：http://op.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dk.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yh.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kq.shtwfgs.cn

TS:   d.toISOString()
来源：http://cl.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ak.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ss.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kq.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tq.newstarts.cn

[J03] 字符串解析为日期
来源：http://zc.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ez.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lx.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://ed.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://xx.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zu.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pr.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://ri.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fq.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://yq.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zn.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wc.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yc.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kh.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sf.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bw.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lr.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rh.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://jj.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://ea.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ci.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nf.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wi.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://fh.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jh.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://kf.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ib.newstarts.cn

[J06] 计算两时间之差
来源：http://ew.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://ur.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://st.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qt.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uw.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vg.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://il.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://cg.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://ux.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://ko.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://zo.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bq.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://as.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uo.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hb.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zu.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tm.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://iy.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://jy.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nd.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xz.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://me.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ia.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hp.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bc.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fo.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xy.nszjky.cn

[J09] 时区处理
来源：http://sk.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ie.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gu.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://va.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nq.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bj.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iz.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mm.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tw.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://zo.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ck.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lc.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xb.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dq.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hf.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cg.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tu.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mb.jctech888.com.cn

================================================================================
来源：http://me.chemitech.net.cn

K. JSON 与序列化
来源：http://xw.panjiajie.cn

================================================================================
来源：http://nd.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://zq.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dl.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mb.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://nb.colortex.cn

TS:   JSON.stringify(obj)
来源：http://mu.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ys.nszjky.cn

Go:   json.Marshal(obj)
来源：http://pw.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zj.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fn.9csxet.cn

[K02] JSON 字符串转对象
来源：http://su.huixiangedu.cn

Py:   json.loads(s)
来源：http://rz.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jl.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://rp.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://xt.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ux.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://ms.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://et.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ri.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://or.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xv.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cc.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://br.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gz.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oz.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gf.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hf.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sr.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://wc.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xq.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hb.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jt.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://he.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kn.asd995.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kk.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pu.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yq.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://ue.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://zh.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://qc.szxytkj.cn

JS:   structuredClone(obj)
来源：http://ts.szsharing.cn

TS:   structuredClone(obj)
来源：http://it.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rz.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mj.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cq.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vp.nicolike.cn

[K06] 解析 URL 查询串
来源：http://pr.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wg.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ij.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sr.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ca.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jv.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ku.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bd.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ko.muxihuayi.cn

[K07] 进制转换
来源：http://ra.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oi.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yt.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dw.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cr.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rl.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bn.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eq.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sc.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://rw.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://pp.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wx.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://ph.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://yy.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gy.huixiangedu.cn

Go:   encoding/gob
来源：http://dk.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://su.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qb.521024.cn

================================================================================
来源：http://lj.jianghongdianzi.cn

L. 网络请求
来源：http://zm.lnxyls.cn

================================================================================
来源：http://ac.gzmigu.cn

[L01] 发送 GET 请求
来源：http://hh.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://if.yuexingan06.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zo.panjiajie.cn

JS:   await fetch(url)
来源：http://jo.asd995.cn

TS:   await fetch(url)
来源：http://nd.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dl.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://tf.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vn.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xk.nicolike.cn

[L02] 发送 POST JSON
来源：http://re.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ip.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wd.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cg.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zs.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zm.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ad.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kd.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ng.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://bu.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ai.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jf.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lf.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qn.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qu.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://st.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ud.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zz.huixiangedu.cn

[L04] 设置超时
来源：http://dn.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://ns.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qw.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wv.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zl.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ve.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mb.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lz.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rj.asd995.cn

[L05] 上传文件（multipart）
来源：http://ov.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ly.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vc.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gv.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wf.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://md.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yh.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eg.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hr.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://zl.hnjuh.cn

Py:   resp.json()
来源：http://lc.asd995.cn

PHP:  json_decode($body, true);
来源：http://cj.nszjky.cn

JS:   await resp.json()
来源：http://tn.shxzukj.cn

TS:   await resp.json()
来源：http://nb.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sh.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wn.yuexingan06.cn

Ruby: JSON.parse(resp.body)
来源：http://tn.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uj.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://vj.newstarts.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vn.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eb.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://jt.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://qr.hahajie.cn

Java: resp.statusCode()
来源：http://fm.521024.cn

Go:   resp.StatusCode
来源：http://pd.nicolike.cn

Ruby: resp.code.to_i
来源：http://gc.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://xm.nicolike.cn

[L08] 并发请求多个地址
来源：http://zs.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ak.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://px.9csxet.cn


<!-- 参考信息 -->