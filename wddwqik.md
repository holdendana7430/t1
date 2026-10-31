代发 wailian999

================================================================================
来源：http://hf.bookmarksfly.cn

I. 正则表达式
来源：http://vu.newstarts.cn

================================================================================
来源：http://ak.szxytkj.cn

[I01] 判断是否匹配
来源：http://xr.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bp.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fi.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://yp.9csxet.cn

TS:   /\d+/.test(s)
来源：http://fw.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ym.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pk.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://jb.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gh.huixiangedu.cn

[I02] 提取所有匹配
来源：http://zb.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://lo.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bl.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://at.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://jp.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pq.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mn.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://fn.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ol.521024.cn

[I03] 提取捕获分组
来源：http://is.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ht.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xj.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pf.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ai.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ox.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vn.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fu.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qs.haigaiapp.cn

[I04] 正则替换
来源：http://dz.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vp.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ft.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ys.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://og.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ip.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jq.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wa.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bd.shtwfgs.cn

[I05] 按正则拆分
来源：http://oa.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kg.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jt.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://pr.lnxyls.cn

TS:   s.split(/\s*,\s*/)
来源：http://fh.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://tj.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ji.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qo.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fk.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oa.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ti.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yv.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qn.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pe.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dy.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eg.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ak.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gd.521024.cn

[I07] 忽略大小写与多行模式
来源：http://fc.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cb.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mf.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://up.huixiangedu.cn

TS:   /error/gim
来源：http://eu.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://if.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gz.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://bo.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vj.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://hp.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bk.huixiangedu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bu.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xn.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uf.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pb.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fe.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dm.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hw.jianghongdianzi.cn

================================================================================
来源：http://lv.chemitech.net.cn

J. 日期与时间
来源：http://tq.newstarts.cn

================================================================================
来源：http://li.hahajie.cn

[J01] 获取当前时间
来源：http://vt.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cf.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oi.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://rf.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://ns.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://aq.9csxet.cn

Go:   time.Now()
来源：http://ry.shxzskj.cn

Ruby: Time.now
来源：http://pd.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bb.shtwfgs.cn

[J02] 格式化输出
来源：http://ek.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tq.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ii.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wz.521024.cn

TS:   d.toISOString()
来源：http://tw.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ey.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xv.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ji.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ng.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://bu.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://do.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ph.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://gn.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://wn.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://py.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ec.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ze.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hq.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://pq.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gx.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zu.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bc.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jb.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hl.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eg.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zs.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sb.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://ji.colortex.cn

Py:   now + timedelta(days=7)
来源：http://js.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ce.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bq.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pq.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://xq.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pm.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://pe.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uo.haigaiapp.cn

[J06] 计算两时间之差
来源：http://pi.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://vd.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://zo.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://za.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kq.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uz.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://hz.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://tz.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://ez.shxzukj.cn

[J07] 比较两个日期
来源：http://rq.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://sw.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sw.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ml.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rb.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jl.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ae.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ae.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://px.colortex.cn

[J08] 提取年月日与星期
来源：http://yn.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tk.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vp.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ar.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jf.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ns.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kj.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ru.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zq.shxzukj.cn

[J09] 时区处理
来源：http://bw.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ve.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hb.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://km.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bn.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dg.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hl.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ol.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fp.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://su.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pn.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zw.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hp.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kq.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hf.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ic.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qz.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nf.shxzukj.cn

================================================================================
来源：http://fm.gzmigu.cn

K. JSON 与序列化
来源：http://xs.wgjwhj.cn

================================================================================
来源：http://qd.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://um.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fq.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gq.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://ps.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://ag.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ri.nicolike.cn

Go:   json.Marshal(obj)
来源：http://au.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://eo.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kc.nszjky.cn

[K02] JSON 字符串转对象
来源：http://nz.9csxet.cn

Py:   json.loads(s)
来源：http://fl.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dn.szxytkj.cn

JS:   JSON.parse(s)
来源：http://um.shxzskj.cn

TS:   JSON.parse(s)
来源：http://vp.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bj.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://wm.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://qo.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zv.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://oq.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cr.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cx.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ot.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://in.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ey.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vl.521024.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zf.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lu.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://zi.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vm.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qy.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pr.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pp.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ed.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zr.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pu.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iq.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://hu.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://eh.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://wo.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://zf.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://do.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qr.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bo.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zs.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lp.hahajie.cn

[K06] 解析 URL 查询串
来源：http://os.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://km.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sn.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vf.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hk.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nb.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cf.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xc.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pm.panjiajie.cn

[K07] 进制转换
来源：http://ls.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eq.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wo.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://it.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ln.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ei.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ru.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fx.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://av.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://lb.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://ob.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://by.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://rz.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://yv.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wr.hnjuh.cn

Go:   encoding/gob
来源：http://pt.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://dc.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kl.nicolike.cn

================================================================================
来源：http://ai.jctech888.com.cn

L. 网络请求
来源：http://qc.huixinmuqiang.cn

================================================================================
来源：http://aa.nszjky.cn

[L01] 发送 GET 请求
来源：http://yg.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gg.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zx.lnxyls.cn

JS:   await fetch(url)
来源：http://ew.haigaiapp.cn

TS:   await fetch(url)
来源：http://ic.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dy.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://oz.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nq.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fa.9csxet.cn

[L02] 发送 POST JSON
来源：http://yu.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bf.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dt.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sn.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dj.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sk.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bh.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://of.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ro.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://jv.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ph.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lx.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://au.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jb.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ii.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tb.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bs.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wy.chemitech.net.cn

[L04] 设置超时
来源：http://vq.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://lh.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gu.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yy.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bc.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hj.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mg.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ld.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rf.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://ea.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wn.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cz.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bs.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pr.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qy.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ef.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iq.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iy.9csxet.cn

[L06] 解析响应为 JSON
来源：http://xt.bjjhwx.cn

Py:   resp.json()
来源：http://gw.huanxung.cn

PHP:  json_decode($body, true);
来源：http://dq.szsharing.cn

JS:   await resp.json()
来源：http://oa.jianghongdianzi.cn

TS:   await resp.json()
来源：http://iq.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ya.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ty.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://jy.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bm.shxzukj.cn


<!-- 参考信息 -->