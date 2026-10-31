代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zf.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vc.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://le.szsharing.cn

TS:   /\d+/.test(s)
来源：http://xr.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mk.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mw.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://km.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://az.haigaiapp.cn

[I02] 提取所有匹配
来源：http://ga.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://yk.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hy.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rd.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://ah.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wk.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pw.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://ac.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hl.gzmigu.cn

[I03] 提取捕获分组
来源：http://gv.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vj.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jk.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mi.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ah.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vz.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vv.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gz.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hq.521024.cn

[I04] 正则替换
来源：http://nm.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qv.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fr.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bt.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mx.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vj.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gf.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xq.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://by.nicolike.cn

[I05] 按正则拆分
来源：http://td.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qe.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hv.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ph.hahajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://bo.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://er.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://og.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://eo.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nh.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nq.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wt.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ua.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mm.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gx.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rr.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qm.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uc.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fr.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://py.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lp.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kc.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gy.hahajie.cn

TS:   /error/gim
来源：http://sj.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nl.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ds.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://oq.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fk.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://wd.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cf.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mm.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ix.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nt.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vj.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rk.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qf.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zf.huixinmuqiang.cn

================================================================================
来源：http://bj.bookmarksfly.cn

J. 日期与时间
来源：http://fb.huanxung.cn

================================================================================
来源：http://wc.colortex.cn

[J01] 获取当前时间
来源：http://qe.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://or.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uv.9csxet.cn

JS:   new Date();  Date.now()
来源：http://td.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://fq.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xd.bookmarksfly.cn

Go:   time.Now()
来源：http://il.9csxet.cn

Ruby: Time.now
来源：http://rq.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bx.bookmarksfly.cn

[J02] 格式化输出
来源：http://ck.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rz.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://of.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bu.nicolike.cn

TS:   d.toISOString()
来源：http://jh.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yv.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yu.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://st.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mg.panjiajie.cn

[J03] 字符串解析为日期
来源：http://hc.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://el.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ma.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://pc.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://pi.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qr.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://us.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://oe.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vb.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://pt.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uk.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wi.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ki.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lw.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uk.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ju.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qd.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ap.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://pb.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://em.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://en.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iy.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fm.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://ir.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jt.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://zl.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://eu.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://wj.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://so.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://nu.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nz.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qb.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://to.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://wo.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://uj.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://gn.panjiajie.cn

[J07] 比较两个日期
来源：http://om.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://uc.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ds.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mn.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bk.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ox.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fs.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jg.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://to.huixiangedu.cn

[J08] 提取年月日与星期
来源：http://tn.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pk.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cd.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fe.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yg.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ai.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oq.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fk.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wf.lnxyls.cn

[J09] 时区处理
来源：http://nj.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ue.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bz.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rn.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ed.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mz.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pd.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zk.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://up.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://wk.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vs.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://np.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pd.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hq.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://je.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ly.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ds.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kc.jianghongdianzi.cn

================================================================================
来源：http://eq.wgjwhj.cn

K. JSON 与序列化
来源：http://mv.panjiajie.cn

================================================================================
来源：http://py.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://im.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dj.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lq.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://iu.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://da.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ye.szsharing.cn

Go:   json.Marshal(obj)
来源：http://ob.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ar.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pq.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://ry.lnxyls.cn

Py:   json.loads(s)
来源：http://tn.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pe.colortex.cn

JS:   JSON.parse(s)
来源：http://jd.521024.cn

TS:   JSON.parse(s)
来源：http://ea.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wn.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://fk.szsharing.cn

Ruby: JSON.parse(s)
来源：http://cq.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dq.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://tf.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ka.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xp.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qm.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://iq.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rf.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fo.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ss.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yg.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://yw.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://md.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://js.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ld.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nr.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xd.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://io.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bf.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://td.panjiajie.cn

[K05] 深拷贝对象
来源：http://ni.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://nn.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://go.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://dh.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://kx.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qq.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://be.9csxet.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://io.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vz.521024.cn

[K06] 解析 URL 查询串
来源：http://yv.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dp.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ae.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dm.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eu.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yy.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ew.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ef.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rc.bookmarksfly.cn

[K07] 进制转换
来源：http://yr.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zc.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ib.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cr.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ad.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xz.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iw.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ij.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lw.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://ms.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://ie.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://we.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://xx.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://ub.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dy.521024.cn

Go:   encoding/gob
来源：http://zx.521024.cn

Ruby: Marshal.dump(obj)
来源：http://da.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lz.yuexingan06.cn

================================================================================
来源：http://te.shtwfgs.cn

L. 网络请求
来源：http://ao.asd995.cn

================================================================================
来源：http://kr.huanxung.cn

[L01] 发送 GET 请求
来源：http://wm.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qa.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cb.shxzukj.cn

JS:   await fetch(url)
来源：http://ak.shxzukj.cn

TS:   await fetch(url)
来源：http://ho.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jr.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://jz.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ae.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tt.nicolike.cn

[L02] 发送 POST JSON
来源：http://wr.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zk.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mc.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qd.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zh.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://js.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yv.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://za.bjjhwx.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xf.nszjky.cn

[L03] 设置自定义请求头
来源：http://pk.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yz.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bz.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zc.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dm.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zr.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cb.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qq.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kb.szxytkj.cn

[L04] 设置超时
来源：http://hr.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://vp.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mg.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ej.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aq.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hj.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mv.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ft.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jm.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://xs.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xg.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qb.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://my.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uc.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zz.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ss.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://la.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uz.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://mv.shxzskj.cn

Py:   resp.json()
来源：http://uc.521024.cn

PHP:  json_decode($body, true);
来源：http://zt.szsharing.cn

JS:   await resp.json()
来源：http://tl.nszjky.cn

TS:   await resp.json()
来源：http://wo.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vl.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uw.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://pe.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://er.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://cb.newstarts.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qo.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bo.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://sa.lnxyls.cn


<!-- 参考信息 -->