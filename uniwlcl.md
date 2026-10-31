代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wr.gzmigu.cn

Go:   defer f.Close()
来源：http://qu.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fh.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ki.huixiangedu.cn

================================================================================
来源：http://pa.chemitech.net.cn

I. 正则表达式
来源：http://zo.chemitech.net.cn

================================================================================
来源：http://ng.chemitech.net.cn

[I01] 判断是否匹配
来源：http://pj.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mm.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tn.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://vk.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://nt.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fu.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bv.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://ai.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vd.wgjwhj.cn

[I02] 提取所有匹配
来源：http://og.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://kz.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ep.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xv.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://fb.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uh.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://um.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://qe.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wu.gzmigu.cn

[I03] 提取捕获分组
来源：http://gj.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wh.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://iz.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pr.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ar.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hb.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yh.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vj.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tg.newstarts.cn

[I04] 正则替换
来源：http://km.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://am.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hk.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fz.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ws.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kx.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ck.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jg.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yq.chemitech.net.cn

[I05] 按正则拆分
来源：http://oc.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bd.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ez.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://av.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://bi.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://gw.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ze.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nu.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tb.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://el.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jg.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lg.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xs.521024.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vu.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://af.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cd.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tn.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ir.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://tz.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://al.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ly.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://si.wgjwhj.cn

TS:   /error/gim
来源：http://yo.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ut.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ak.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://zm.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bh.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://ht.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jm.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zv.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yr.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bm.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zk.nszjky.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xy.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jm.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mp.521024.cn

================================================================================
来源：http://oo.panjiajie.cn

J. 日期与时间
来源：http://es.lnxyls.cn

================================================================================
来源：http://fo.huanxung.cn

[J01] 获取当前时间
来源：http://qf.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bc.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jj.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://kk.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://km.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ez.shtwfgs.cn

Go:   time.Now()
来源：http://ir.newstarts.cn

Ruby: Time.now
来源：http://po.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rp.bjjhwx.cn

[J02] 格式化输出
来源：http://bk.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pn.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wz.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lg.chemitech.net.cn

TS:   d.toISOString()
来源：http://mp.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mh.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kf.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ky.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://da.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://rg.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://df.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wx.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://gl.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://ss.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ec.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vj.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://ky.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gr.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://xx.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dq.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zw.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gy.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tj.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hl.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ay.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xr.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sh.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://de.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://se.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vu.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nu.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vz.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://cf.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vd.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://by.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lk.haigaiapp.cn

[J06] 计算两时间之差
来源：http://pj.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://os.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://mb.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cj.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zc.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://in.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://tl.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://mo.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://dm.nszjky.cn

[J07] 比较两个日期
来源：http://ud.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://jt.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wn.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zd.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fa.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://up.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tg.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://aw.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://ez.521024.cn

[J08] 提取年月日与星期
来源：http://ck.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vo.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gl.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ew.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uf.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wx.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rh.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://di.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cx.asd995.cn

[J09] 时区处理
来源：http://vm.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ej.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ha.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ah.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eg.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qe.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eg.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lu.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pp.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://yk.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jr.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cq.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dv.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kz.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yk.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fj.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qz.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hc.colortex.cn

================================================================================
来源：http://fd.nszjky.cn

K. JSON 与序列化
来源：http://wh.newstarts.cn

================================================================================
来源：http://bg.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://cn.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vc.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zk.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://hf.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://he.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ax.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://ll.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ym.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://de.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://wj.yuexingan06.cn

Py:   json.loads(s)
来源：http://uk.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dm.asd995.cn

JS:   JSON.parse(s)
来源：http://kx.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://dy.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kz.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://vk.nszjky.cn

Ruby: JSON.parse(s)
来源：http://yi.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yy.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://tm.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tf.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mv.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rj.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rl.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uo.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gb.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cz.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gx.nicolike.cn

[K04] 读取 JSON 文件
来源：http://je.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yk.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pm.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jo.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hl.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rj.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wx.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jk.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ba.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://th.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://dz.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://in.colortex.cn

JS:   structuredClone(obj)
来源：http://gk.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://xx.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sq.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cc.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yp.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jb.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://ls.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uk.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fb.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yu.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lv.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nx.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hr.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gh.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cc.newstarts.cn

[K07] 进制转换
来源：http://oe.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ox.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rq.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kc.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dj.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ua.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sb.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qv.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wv.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://td.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://kv.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pb.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://lm.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://is.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ds.wgjwhj.cn

Go:   encoding/gob
来源：http://zz.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://mf.9csxet.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://az.yuntaijiaju.cn

================================================================================
来源：http://kz.hnjuh.cn

L. 网络请求
来源：http://fc.yuexingan06.cn

================================================================================
来源：http://kp.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://dv.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bx.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xe.bookmarksfly.cn

JS:   await fetch(url)
来源：http://di.shxzskj.cn

TS:   await fetch(url)
来源：http://ot.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ig.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://dh.asd995.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://up.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rd.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://qk.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uq.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cw.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qk.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://if.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qh.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://to.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zo.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fa.9csxet.cn

[L03] 设置自定义请求头
来源：http://nt.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eu.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ur.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yr.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dg.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ht.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qs.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lz.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pi.huixinmuqiang.cn

[L04] 设置超时
来源：http://wq.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://lf.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jb.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pq.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qj.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://og.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ug.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://je.9csxet.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yr.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://nr.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ji.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uw.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uv.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fr.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oo.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ml.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zy.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ei.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://rm.yuntaijiaju.cn

Py:   resp.json()
来源：http://rm.colortex.cn

PHP:  json_decode($body, true);
来源：http://qz.colortex.cn

JS:   await resp.json()
来源：http://oy.asd995.cn

TS:   await resp.json()
来源：http://fv.521024.cn


<!-- 参考信息 -->