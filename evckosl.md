代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://yz.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://zj.jctech888.com.cn

[H09] 带错误码的异常
来源：http://mp.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hg.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xw.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qp.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zd.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cf.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ya.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ba.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jo.huixiangedu.cn

[H10] 资源自动释放
来源：http://te.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sc.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qw.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eu.hnjuh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ae.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uj.szsharing.cn

Go:   defer f.Close()
来源：http://uu.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wn.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nq.huanxung.cn

================================================================================
来源：http://xs.521024.cn

I. 正则表达式
来源：http://ns.bookmarksfly.cn

================================================================================
来源：http://il.shxzukj.cn

[I01] 判断是否匹配
来源：http://ed.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zp.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ja.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://cm.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://zv.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ke.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rt.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://kb.nicolike.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fp.wgjwhj.cn

[I02] 提取所有匹配
来源：http://dl.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://rq.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yu.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yp.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://vo.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bi.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vr.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://qc.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bi.lnxyls.cn

[I03] 提取捕获分组
来源：http://fr.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wc.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jq.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mi.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hj.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rj.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xo.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gq.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hm.asd995.cn

[I04] 正则替换
来源：http://ug.gzmigu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zb.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://li.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nn.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://eu.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uy.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sh.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tg.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zv.wgjwhj.cn

[I05] 按正则拆分
来源：http://tz.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gq.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pj.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://ku.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://jp.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://dh.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://of.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gi.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cz.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pm.asd995.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dw.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://os.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hu.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gd.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mv.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gm.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gl.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bp.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://zw.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ke.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sp.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pz.521024.cn

TS:   /error/gim
来源：http://ci.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pp.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://et.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://wh.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fw.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://uf.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nw.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sv.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://as.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cp.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ls.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cb.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ec.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iu.shxzukj.cn

================================================================================
来源：http://wh.shxzukj.cn

J. 日期与时间
来源：http://tq.huixiangedu.cn

================================================================================
来源：http://hz.colortex.cn

[J01] 获取当前时间
来源：http://bd.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tn.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kr.colortex.cn

JS:   new Date();  Date.now()
来源：http://hl.hahajie.cn

TS:   new Date();  Date.now()
来源：http://qf.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ig.panjiajie.cn

Go:   time.Now()
来源：http://dp.huixinmuqiang.cn

Ruby: Time.now
来源：http://rh.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pk.wgjwhj.cn

[J02] 格式化输出
来源：http://hl.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xf.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lr.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sr.jctech888.com.cn

TS:   d.toISOString()
来源：http://ls.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cy.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wv.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wp.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sp.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://ym.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yo.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fi.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://ib.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://ec.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bh.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://db.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://cm.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ez.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://oa.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://si.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cf.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cx.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jk.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ev.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ix.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://em.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kh.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://om.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://fa.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dj.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pk.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bs.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://gd.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zz.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://yy.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bu.huixiangedu.cn

[J06] 计算两时间之差
来源：http://sa.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://ji.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://yj.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://df.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mn.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ld.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://qd.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://mj.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://or.nszjky.cn

[J07] 比较两个日期
来源：http://mw.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://sj.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ks.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ne.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bq.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wn.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pq.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nc.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://fh.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://ni.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yh.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cl.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gq.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cb.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ho.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kx.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xg.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tp.lnxyls.cn

[J09] 时区处理
来源：http://xw.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kg.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sm.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fl.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ra.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jk.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jr.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wu.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://mo.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rm.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wf.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cg.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ek.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://js.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gv.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bd.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rg.huanxung.cn

================================================================================
来源：http://ve.asd995.cn

K. JSON 与序列化
来源：http://ut.haigaiapp.cn

================================================================================
来源：http://iz.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://om.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://my.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://et.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://iy.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://ul.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gu.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://db.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jj.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ry.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://ky.nszjky.cn

Py:   json.loads(s)
来源：http://zv.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://or.shxzskj.cn

JS:   JSON.parse(s)
来源：http://in.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://tn.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oz.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://bq.hahajie.cn

Ruby: JSON.parse(s)
来源：http://xx.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dl.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://ir.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ry.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kd.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tg.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nj.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iy.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ff.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kv.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rv.nszjky.cn

[K04] 读取 JSON 文件
来源：http://hm.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iq.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wa.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cu.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nh.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iz.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dq.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vh.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zd.nszjky.cn

[K05] 深拷贝对象
来源：http://fy.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://dd.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://so.lnxyls.cn

JS:   structuredClone(obj)
来源：http://lf.shxzukj.cn

TS:   structuredClone(obj)
来源：http://nc.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wn.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cr.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://si.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ku.asd995.cn

[K06] 解析 URL 查询串
来源：http://tn.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lv.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://id.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jw.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ln.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fu.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://du.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nr.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fe.9csxet.cn

[K07] 进制转换
来源：http://qj.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ae.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dv.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xf.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ob.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://am.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://aw.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jc.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ez.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://kd.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://bx.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ne.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://gb.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://rq.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mu.9csxet.cn

Go:   encoding/gob
来源：http://sx.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://yf.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qc.huixinmuqiang.cn

================================================================================
来源：http://li.jctech888.com.cn

L. 网络请求
来源：http://fq.szsharing.cn

================================================================================
来源：http://az.521024.cn

[L01] 发送 GET 请求
来源：http://pj.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eq.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qa.newstarts.cn

JS:   await fetch(url)
来源：http://wl.shtwfgs.cn

TS:   await fetch(url)
来源：http://zf.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ez.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://ct.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vn.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qi.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://vu.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xu.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oc.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tr.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qb.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pr.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dg.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yl.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sm.szsharing.cn

[L03] 设置自定义请求头
来源：http://ii.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pe.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zd.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ql.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jj.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zo.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cg.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cs.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mb.9csxet.cn

[L04] 设置超时
来源：http://sa.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://cz.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rw.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://st.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cp.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zs.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://an.shtwfgs.cn


<!-- 参考信息 -->