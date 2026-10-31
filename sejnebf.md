代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zm.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tx.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lw.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://mt.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://eq.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xg.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gu.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bl.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vl.521024.cn

Go:   defer f.Close()
来源：http://rw.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://on.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hh.nicolike.cn

================================================================================
来源：http://kr.newstarts.cn

I. 正则表达式
来源：http://tk.panjiajie.cn

================================================================================
来源：http://ze.szxytkj.cn

[I01] 判断是否匹配
来源：http://er.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mv.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nu.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://cp.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://jh.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ld.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eq.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://ho.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cs.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://it.shxzukj.cn

Py:   re.findall(r"\d+", s)
来源：http://zf.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qv.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fg.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://jo.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qh.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fx.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://vs.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ws.panjiajie.cn

[I03] 提取捕获分组
来源：http://ld.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ze.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sl.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wb.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jn.yuexingan06.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ua.wgjwhj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bn.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wx.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fa.colortex.cn

[I04] 正则替换
来源：http://fe.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ow.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://on.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mm.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bw.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://un.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sh.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pw.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ku.newstarts.cn

[I05] 按正则拆分
来源：http://xs.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ld.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gg.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://wl.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://ym.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://ps.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fs.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pe.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kg.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tz.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gb.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gq.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ah.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iv.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xq.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://su.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sn.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://az.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://lx.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ss.bookmarksfly.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://id.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kw.lnxyls.cn

TS:   /error/gim
来源：http://yc.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://om.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://so.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://ix.szsharing.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dt.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ir.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vp.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ph.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ho.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gv.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ka.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ix.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zr.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ec.nicolike.cn

================================================================================
来源：http://eb.hnjuh.cn

J. 日期与时间
来源：http://va.szsharing.cn

================================================================================
来源：http://qm.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://yh.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tz.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tv.521024.cn

JS:   new Date();  Date.now()
来源：http://sa.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://dj.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ii.jianghongdianzi.cn

Go:   time.Now()
来源：http://li.szsharing.cn

Ruby: Time.now
来源：http://yy.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sm.szxytkj.cn

[J02] 格式化输出
来源：http://za.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hd.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hp.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rg.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://du.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xi.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ri.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ed.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hv.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://qa.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yi.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gq.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://dj.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://rq.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vb.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wr.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://gy.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qk.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://io.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rw.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jn.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zq.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ag.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mb.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ga.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gc.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zf.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://cc.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://mr.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fi.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://he.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gd.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://lp.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lg.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://wq.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ef.gzmigu.cn

[J06] 计算两时间之差
来源：http://sd.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://dx.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://ml.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bn.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://me.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pk.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://lw.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://rh.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://al.szsharing.cn

[J07] 比较两个日期
来源：http://fc.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://tp.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ix.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fo.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://me.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kh.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cy.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://st.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://cz.gzmigu.cn

[J08] 提取年月日与星期
来源：http://ht.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tq.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jf.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ob.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eq.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yj.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ds.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zj.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zy.chemitech.net.cn

[J09] 时区处理
来源：http://am.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ez.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tr.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ul.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vw.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zx.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yr.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://em.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ei.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://fg.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oy.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ms.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fb.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qc.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ui.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lt.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bb.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ht.hahajie.cn

================================================================================
来源：http://lz.shtwfgs.cn

K. JSON 与序列化
来源：http://tj.shxzskj.cn

================================================================================
来源：http://yc.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://wq.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sz.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vz.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://lu.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://jc.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://go.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://dz.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nk.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zh.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://em.lnxyls.cn

Py:   json.loads(s)
来源：http://vd.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bh.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://sq.panjiajie.cn

TS:   JSON.parse(s)
来源：http://az.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gt.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://rc.hahajie.cn

Ruby: JSON.parse(s)
来源：http://to.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://en.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://zy.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qb.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://am.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ua.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ly.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lz.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gs.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zq.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ga.521024.cn

[K04] 读取 JSON 文件
来源：http://uq.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qb.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sk.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eq.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ki.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://di.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ms.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hq.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jc.newstarts.cn

[K05] 深拷贝对象
来源：http://dh.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://ec.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://zt.szxytkj.cn

JS:   structuredClone(obj)
来源：http://ow.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://xr.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dh.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mn.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tx.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ys.szsharing.cn

[K06] 解析 URL 查询串
来源：http://yg.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ag.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fn.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fi.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://si.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dq.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wz.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pj.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gu.nszjky.cn

[K07] 进制转换
来源：http://pb.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iz.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ia.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zd.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eo.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sj.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vc.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gp.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ug.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://cm.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://ad.haigaiapp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ad.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://wb.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://ur.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nt.bookmarksfly.cn

Go:   encoding/gob
来源：http://jh.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://xo.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zv.wgjwhj.cn

================================================================================
来源：http://oy.newstarts.cn

L. 网络请求
来源：http://nw.bookmarksfly.cn

================================================================================
来源：http://qu.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://gw.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://no.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sh.lnxyls.cn

JS:   await fetch(url)
来源：http://mf.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://va.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tl.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://qw.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://or.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bz.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://va.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pg.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://db.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vs.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zi.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bp.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hc.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zs.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gu.nszjky.cn

[L03] 设置自定义请求头
来源：http://vl.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ei.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mn.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lb.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ds.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ow.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://at.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aa.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pl.huixinmuqiang.cn

[L04] 设置超时
来源：http://jm.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://ta.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://si.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ln.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aj.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://af.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gf.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ny.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ng.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://ku.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qx.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gw.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bg.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://on.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vs.muxihuayi.cn


<!-- 参考信息 -->