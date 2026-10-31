代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gr.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xv.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://ug.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yu.szxytkj.cn

[I02] 提取所有匹配
来源：http://gy.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://uo.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ym.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ny.bjjhwx.cn

TS:   s.match(/\d+/g)
来源：http://rd.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sv.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hm.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://gw.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yf.lnxyls.cn

[I03] 提取捕获分组
来源：http://gc.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://or.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ec.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xc.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gj.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sp.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rv.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kj.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hp.colortex.cn

[I04] 正则替换
来源：http://om.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xa.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kp.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tg.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cv.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dm.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bc.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uj.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xm.wgjwhj.cn

[I05] 按正则拆分
来源：http://ll.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nt.521024.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ll.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://zi.lnxyls.cn

TS:   s.split(/\s*,\s*/)
来源：http://ex.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://ya.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sh.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rf.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bj.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mo.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tm.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kf.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rq.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ro.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sj.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ei.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ky.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pm.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://nm.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uk.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gu.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vt.bookmarksfly.cn

TS:   /error/gim
来源：http://vc.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ge.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wi.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://fg.szsharing.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fe.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://nw.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vi.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://as.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xk.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oa.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fn.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hl.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vc.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qf.huanxung.cn

================================================================================
来源：http://ie.chemitech.net.cn

J. 日期与时间
来源：http://fj.szxytkj.cn

================================================================================
来源：http://fi.bjjhwx.cn

[J01] 获取当前时间
来源：http://jj.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qv.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hd.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://bg.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://at.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ek.yuexingan06.cn

Go:   time.Now()
来源：http://gh.hahajie.cn

Ruby: Time.now
来源：http://bs.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gs.jianghongdianzi.cn

[J02] 格式化输出
来源：http://er.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xs.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vj.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pn.haigaiapp.cn

TS:   d.toISOString()
来源：http://en.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ja.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zs.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ne.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zk.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://xm.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zj.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oy.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://ig.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://oa.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qw.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xe.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://dn.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cy.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://jq.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vt.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hy.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vw.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lw.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eb.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rs.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ur.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vj.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://gb.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://kh.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://oj.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aa.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fg.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://to.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ak.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://wc.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hv.9csxet.cn

[J06] 计算两时间之差
来源：http://me.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://kd.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://bh.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://is.hnjuh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xo.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yx.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://qr.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://qu.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://ol.9csxet.cn

[J07] 比较两个日期
来源：http://bp.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://oq.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ea.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xy.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qa.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oj.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bh.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pn.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://fl.szsharing.cn

[J08] 提取年月日与星期
来源：http://on.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sn.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tc.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://st.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://al.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nz.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dt.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ti.haigaiapp.cn

[J09] 时区处理
来源：http://yp.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qe.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mv.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yg.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ki.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vr.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uh.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://he.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sm.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://dx.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zj.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sm.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ql.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://el.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jo.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sa.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lv.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pl.yuntaijiaju.cn

================================================================================
来源：http://no.jctech888.com.cn

K. JSON 与序列化
来源：http://lf.muxihuayi.cn

================================================================================
来源：http://nx.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://gs.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pn.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dc.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://ls.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://jz.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hy.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://gl.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mo.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mw.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://dp.wgjwhj.cn

Py:   json.loads(s)
来源：http://kr.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pm.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://wr.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://bu.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tf.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://oq.nszjky.cn

Ruby: JSON.parse(s)
来源：http://zp.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qc.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://jh.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jg.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wr.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fl.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sj.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ss.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tt.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qy.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bn.521024.cn

[K04] 读取 JSON 文件
来源：http://rm.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yo.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://no.szsharing.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zo.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fq.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pp.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pp.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://it.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://um.haigaiapp.cn

[K05] 深拷贝对象
来源：http://sw.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://av.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://za.panjiajie.cn

JS:   structuredClone(obj)
来源：http://xh.9csxet.cn

TS:   structuredClone(obj)
来源：http://ac.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ta.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sl.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eb.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://iy.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://ne.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fa.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lb.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://at.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zr.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sv.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xz.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ej.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xi.nicolike.cn

[K07] 进制转换
来源：http://gi.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gq.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wb.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rm.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yb.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ej.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iq.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oe.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bf.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://fg.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://pv.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bp.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://rx.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://yo.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wu.bookmarksfly.cn

Go:   encoding/gob
来源：http://dp.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://mr.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nv.huanxung.cn

================================================================================
来源：http://ep.hahajie.cn

L. 网络请求
来源：http://qg.yuntaijiaju.cn

================================================================================
来源：http://ri.shxzskj.cn

[L01] 发送 GET 请求
来源：http://yw.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://it.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tk.gzmigu.cn

JS:   await fetch(url)
来源：http://dq.bookmarksfly.cn

TS:   await fetch(url)
来源：http://du.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gw.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://ef.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qd.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oi.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://fx.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rt.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jv.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gq.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mh.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lc.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nc.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bs.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ju.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://wk.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ab.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cg.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dz.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vt.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pq.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sz.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fa.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://au.yuexingan06.cn

[L04] 设置超时
来源：http://un.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://hr.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://do.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://af.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ds.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lj.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sk.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vk.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://on.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://zc.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hp.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fd.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ax.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yw.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wb.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jn.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rk.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mx.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://ny.bjjhwx.cn

Py:   resp.json()
来源：http://ji.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://lw.colortex.cn

JS:   await resp.json()
来源：http://xc.bjjhwx.cn

TS:   await resp.json()
来源：http://uf.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mq.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sl.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://fd.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bv.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://cp.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://di.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ha.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://ej.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://bn.9csxet.cn

Java: resp.statusCode()
来源：http://du.szsharing.cn

Go:   resp.StatusCode
来源：http://ft.szsharing.cn

Ruby: resp.code.to_i
来源：http://ot.gzmigu.cn


<!-- 参考信息 -->