代发 wailian999

================================================================================
来源：http://po.panjiajie.cn

I. 正则表达式
来源：http://xy.panjiajie.cn

================================================================================
来源：http://dn.chemitech.net.cn

[I01] 判断是否匹配
来源：http://va.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ij.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sk.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://wn.newstarts.cn

TS:   /\d+/.test(s)
来源：http://uh.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fe.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cr.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://gx.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gk.newstarts.cn

[I02] 提取所有匹配
来源：http://dv.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://dq.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lp.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://re.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://xe.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uh.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://or.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://pk.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dk.huixiangedu.cn

[I03] 提取捕获分组
来源：http://xo.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dh.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bv.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xd.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xf.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vi.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rc.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fg.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hi.gzmigu.cn

[I04] 正则替换
来源：http://kv.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oq.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sm.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://og.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tg.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fz.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://en.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sq.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bc.9csxet.cn

[I05] 按正则拆分
来源：http://he.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ao.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zg.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://np.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://iz.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://hx.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fq.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ic.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ml.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gg.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zh.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ak.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mr.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://td.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ax.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kc.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lc.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hw.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://hz.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mx.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rs.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cj.asd995.cn

TS:   /error/gim
来源：http://uk.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kj.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lk.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://kx.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://az.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://oc.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://at.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ap.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xs.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pl.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://je.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://po.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pd.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gx.shtwfgs.cn

================================================================================
来源：http://tv.gzmigu.cn

J. 日期与时间
来源：http://kn.nicolike.cn

================================================================================
来源：http://yr.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://tc.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://be.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://po.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://gs.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://lo.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lr.yuexingan06.cn

Go:   time.Now()
来源：http://tz.nicolike.cn

Ruby: Time.now
来源：http://wd.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yf.muxihuayi.cn

[J02] 格式化输出
来源：http://rn.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jh.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wp.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aw.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://xk.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sy.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ab.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zq.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qk.521024.cn

[J03] 字符串解析为日期
来源：http://vf.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bj.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wu.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://bw.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://lu.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ai.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nl.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://hy.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tp.nicolike.cn

[J04] 时间戳与日期互转
来源：http://as.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kn.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nb.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vo.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://em.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zr.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kk.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zj.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ry.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://ef.asd995.cn

Py:   now + timedelta(days=7)
来源：http://ec.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://je.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wr.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tx.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://nk.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pe.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://ih.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vs.haigaiapp.cn

[J06] 计算两时间之差
来源：http://kr.colortex.cn

Py:   (end - start).total_seconds()
来源：http://lx.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://gn.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pa.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sv.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xh.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://qy.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://mu.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://rl.bookmarksfly.cn

[J07] 比较两个日期
来源：http://tu.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://zh.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://de.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zw.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sw.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ur.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kf.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sn.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://py.shxzukj.cn

[J08] 提取年月日与星期
来源：http://ee.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zv.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ps.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dr.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vr.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ck.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jr.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jo.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mc.nszjky.cn

[J09] 时区处理
来源：http://yh.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tt.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ct.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bu.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://te.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ye.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gt.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hl.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qj.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://nl.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jh.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ij.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ls.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qp.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vt.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gu.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vm.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gz.shxzskj.cn

================================================================================
来源：http://bh.nszjky.cn

K. JSON 与序列化
来源：http://cq.nicolike.cn

================================================================================
来源：http://qd.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://xm.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tz.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zq.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://gs.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://vb.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uz.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://mu.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ug.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kb.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://xo.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://dz.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wf.9csxet.cn

JS:   JSON.parse(s)
来源：http://qb.panjiajie.cn

TS:   JSON.parse(s)
来源：http://rl.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wd.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://bs.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://qr.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dr.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://vk.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yw.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ri.jianghongdianzi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zj.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vx.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mm.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vv.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tz.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ej.521024.cn

[K04] 读取 JSON 文件
来源：http://hc.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sk.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ul.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mf.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sm.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yz.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cn.shtwfgs.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://eu.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qd.jctech888.com.cn

[K05] 深拷贝对象
来源：http://tq.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://ae.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://yz.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://tm.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://bx.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tt.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ac.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gs.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hk.nszjky.cn

[K06] 解析 URL 查询串
来源：http://zm.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xi.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://we.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yt.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ir.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://op.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ye.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ds.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mn.huanxung.cn

[K07] 进制转换
来源：http://vx.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uq.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ue.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xd.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zh.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cu.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gm.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kn.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nk.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://la.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://xu.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sk.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://wh.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ep.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zx.asd995.cn

Go:   encoding/gob
来源：http://op.521024.cn

Ruby: Marshal.dump(obj)
来源：http://du.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ek.szsharing.cn

================================================================================
来源：http://bu.nicolike.cn

L. 网络请求
来源：http://wy.panjiajie.cn

================================================================================
来源：http://xh.colortex.cn

[L01] 发送 GET 请求
来源：http://tq.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qk.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sh.shxzskj.cn

JS:   await fetch(url)
来源：http://fq.nicolike.cn

TS:   await fetch(url)
来源：http://hs.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xd.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://uk.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ut.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yf.huanxung.cn

[L02] 发送 POST JSON
来源：http://pt.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dx.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://au.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ih.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eg.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lh.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kg.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wb.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uf.asd995.cn

[L03] 设置自定义请求头
来源：http://ef.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qc.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bn.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sc.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fh.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rq.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://id.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qb.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tg.nicolike.cn

[L04] 设置超时
来源：http://ax.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://yb.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hf.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sj.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vn.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sz.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cj.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yv.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yj.521024.cn

[L05] 上传文件（multipart）
来源：http://ii.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://in.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xl.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ge.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lf.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ie.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://so.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yr.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eq.szsharing.cn

[L06] 解析响应为 JSON
来源：http://hy.panjiajie.cn

Py:   resp.json()
来源：http://nt.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://de.jctech888.com.cn

JS:   await resp.json()
来源：http://xk.bookmarksfly.cn

TS:   await resp.json()
来源：http://ig.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hw.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nn.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://hm.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fv.yuntaijiaju.cn


<!-- 参考信息 -->