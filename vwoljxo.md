代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://sx.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ru.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bo.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://he.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zi.muxihuayi.cn

Go:   defer f.Close()
来源：http://bf.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gc.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://he.yuntaijiaju.cn

================================================================================
来源：http://hp.huixinmuqiang.cn

I. 正则表达式
来源：http://ba.shxzukj.cn

================================================================================
来源：http://ms.huanxung.cn

[I01] 判断是否匹配
来源：http://to.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qd.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hn.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://uv.colortex.cn

TS:   /\d+/.test(s)
来源：http://pu.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://da.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vp.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://wi.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://or.panjiajie.cn

[I02] 提取所有匹配
来源：http://fd.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://bh.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zc.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zk.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://lz.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zm.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bt.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://dt.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://in.huanxung.cn

[I03] 提取捕获分组
来源：http://pi.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vd.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yt.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vh.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bb.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ql.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://il.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ez.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ce.asd995.cn

[I04] 正则替换
来源：http://wy.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nd.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vl.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cs.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bz.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://up.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lv.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vr.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kc.shxzskj.cn

[I05] 按正则拆分
来源：http://dm.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ot.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uk.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://zg.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://ig.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://pv.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pt.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ju.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xq.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zq.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vc.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hb.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qw.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cg.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uc.hahajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ou.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ov.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pg.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://ar.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uh.colortex.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://du.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rz.muxihuayi.cn

TS:   /error/gim
来源：http://zp.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sg.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wv.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://qv.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ds.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://bz.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zg.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mf.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ll.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://in.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fr.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bv.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cj.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ty.bjjhwx.cn

================================================================================
来源：http://xw.bookmarksfly.cn

J. 日期与时间
来源：http://wu.haigaiapp.cn

================================================================================
来源：http://nw.newstarts.cn

[J01] 获取当前时间
来源：http://vj.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vg.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mq.colortex.cn

JS:   new Date();  Date.now()
来源：http://un.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://yz.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tc.muxihuayi.cn

Go:   time.Now()
来源：http://px.bookmarksfly.cn

Ruby: Time.now
来源：http://ly.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zp.szxytkj.cn

[J02] 格式化输出
来源：http://qu.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://te.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://id.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jr.shxzskj.cn

TS:   d.toISOString()
来源：http://nn.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ob.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bd.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dt.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lt.hahajie.cn

[J03] 字符串解析为日期
来源：http://og.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bz.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zf.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://kd.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://da.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jm.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xd.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://ex.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ug.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://nv.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bq.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://un.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ll.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zh.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xo.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bl.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cf.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sw.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://ws.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://bq.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xi.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tr.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://av.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://ol.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ql.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://bs.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zk.nicolike.cn

[J06] 计算两时间之差
来源：http://uv.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://jt.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://yz.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ux.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sv.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://im.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://xc.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://ty.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://bp.521024.cn

[J07] 比较两个日期
来源：http://xl.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://bz.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fj.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://br.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://by.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wz.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pp.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mo.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://mb.hahajie.cn

[J08] 提取年月日与星期
来源：http://vz.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://su.bookmarksfly.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xw.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ff.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nz.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wh.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sx.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vv.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ut.9csxet.cn

[J09] 时区处理
来源：http://xa.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hd.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rg.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://be.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lg.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ym.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://do.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pt.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jw.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://rl.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ue.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gc.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://on.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://un.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jq.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ko.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bn.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fp.jianghongdianzi.cn

================================================================================
来源：http://jc.shxzskj.cn

K. JSON 与序列化
来源：http://jj.shtwfgs.cn

================================================================================
来源：http://ws.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://rg.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://im.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fk.asd995.cn

JS:   JSON.stringify(obj)
来源：http://ct.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://gb.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zi.nszjky.cn

Go:   json.Marshal(obj)
来源：http://zf.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ww.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://st.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://ce.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://hg.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qm.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://yf.szxytkj.cn

TS:   JSON.parse(s)
来源：http://wn.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://im.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://ic.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://rd.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ix.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://zd.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rn.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ob.jianghongdianzi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dd.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qn.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ox.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tx.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vg.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vk.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://ka.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ez.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sq.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rf.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ga.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rh.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://be.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://an.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ds.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://tj.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://lh.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://ez.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://pz.shxzukj.cn

TS:   structuredClone(obj)
来源：http://pm.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ti.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fl.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hk.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vm.szsharing.cn

[K06] 解析 URL 查询串
来源：http://he.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mk.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://st.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://es.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oz.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bo.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fx.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mb.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oa.colortex.cn

[K07] 进制转换
来源：http://wv.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cj.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gr.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mj.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fe.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cw.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ja.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://go.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bb.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://nq.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://le.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fw.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://ch.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://lc.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pj.szxytkj.cn

Go:   encoding/gob
来源：http://hf.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://ai.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ei.lnxyls.cn

================================================================================
来源：http://np.wgjwhj.cn

L. 网络请求
来源：http://kt.jianghongdianzi.cn

================================================================================
来源：http://uw.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://qm.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jt.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dl.gzmigu.cn

JS:   await fetch(url)
来源：http://xw.521024.cn

TS:   await fetch(url)
来源：http://wx.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ep.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://jw.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://km.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jz.9csxet.cn

[L02] 发送 POST JSON
来源：http://vb.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rm.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pt.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gg.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://et.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qu.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://we.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oa.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ij.shxzukj.cn

[L03] 设置自定义请求头
来源：http://oq.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jn.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qa.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gm.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ja.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dm.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xt.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ew.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ip.shxzukj.cn

[L04] 设置超时
来源：http://md.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://ky.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jl.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hm.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://np.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cm.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sl.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wc.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ct.newstarts.cn

[L05] 上传文件（multipart）
来源：http://lh.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mi.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kn.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://za.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zg.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xm.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sm.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vw.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://te.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://gv.gzmigu.cn


<!-- 参考信息 -->