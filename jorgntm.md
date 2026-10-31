代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ji.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ao.gzmigu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uy.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://fx.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vx.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://be.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qt.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://of.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://az.muxihuayi.cn

Go:   defer f.Close()
来源：http://fm.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bm.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sk.colortex.cn

================================================================================
来源：http://aw.huixiangedu.cn

I. 正则表达式
来源：http://pr.gzmigu.cn

================================================================================
来源：http://pa.nicolike.cn

[I01] 判断是否匹配
来源：http://jy.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zt.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ac.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://ve.huanxung.cn

TS:   /\d+/.test(s)
来源：http://vm.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bo.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wz.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://hp.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vi.chemitech.net.cn

[I02] 提取所有匹配
来源：http://ak.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://rw.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yo.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gx.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://pg.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oi.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fl.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://gd.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://np.nicolike.cn

[I03] 提取捕获分组
来源：http://gu.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://of.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hc.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gn.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://if.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uw.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qp.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ok.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mp.huixinmuqiang.cn

[I04] 正则替换
来源：http://nv.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bm.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hg.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fx.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dm.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xm.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dm.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uk.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vh.szxytkj.cn

[I05] 按正则拆分
来源：http://kn.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bs.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ii.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://mg.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://aq.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://tf.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gn.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://po.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fi.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ov.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uh.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ho.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://le.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://od.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pe.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nn.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nw.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yk.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://wb.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ek.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ga.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wv.muxihuayi.cn

TS:   /error/gim
来源：http://wq.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hk.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ws.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://cn.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ge.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://pk.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nc.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sl.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ut.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eb.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ft.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cx.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ub.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xi.panjiajie.cn

================================================================================
来源：http://et.huixinmuqiang.cn

J. 日期与时间
来源：http://ys.panjiajie.cn

================================================================================
来源：http://le.szsharing.cn

[J01] 获取当前时间
来源：http://tl.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gk.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nw.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://yv.nicolike.cn

TS:   new Date();  Date.now()
来源：http://nh.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ef.hnjuh.cn

Go:   time.Now()
来源：http://an.colortex.cn

Ruby: Time.now
来源：http://fa.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rh.9csxet.cn

[J02] 格式化输出
来源：http://xf.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ly.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://at.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ou.shxzukj.cn

TS:   d.toISOString()
来源：http://sg.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bg.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ub.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sc.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vz.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://mp.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qm.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jj.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://qn.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://qh.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ey.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gr.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://yw.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mr.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://no.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xf.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ip.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xg.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ae.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zw.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dq.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tr.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sd.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://wn.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://xi.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yp.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zz.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kq.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://tj.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ql.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://ke.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wy.wgjwhj.cn

[J06] 计算两时间之差
来源：http://qk.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://qr.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://oh.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ls.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ks.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nq.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://oq.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://dp.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://lf.shxzskj.cn

[J07] 比较两个日期
来源：http://se.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://up.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qz.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ab.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rs.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xf.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uq.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qq.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ao.hahajie.cn

[J08] 提取年月日与星期
来源：http://wt.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ms.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xz.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qb.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oq.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ii.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cc.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dn.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rm.newstarts.cn

[J09] 时区处理
来源：http://ah.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://io.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://do.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://if.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rq.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jh.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hs.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qn.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zo.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://sd.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kd.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://go.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uy.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lo.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://au.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gr.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zi.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://az.asd995.cn

================================================================================
来源：http://pu.huanxung.cn

K. JSON 与序列化
来源：http://kh.huanxung.cn

================================================================================
来源：http://lk.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://fa.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sj.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://du.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://an.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://bn.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ek.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://sw.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zi.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ii.newstarts.cn

[K02] JSON 字符串转对象
来源：http://lh.shxzukj.cn

Py:   json.loads(s)
来源：http://yf.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vr.panjiajie.cn

JS:   JSON.parse(s)
来源：http://jg.nszjky.cn

TS:   JSON.parse(s)
来源：http://fr.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pz.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://wq.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://dd.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://us.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://nv.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gt.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ms.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ts.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rb.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://if.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kd.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oj.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://na.szsharing.cn

[K04] 读取 JSON 文件
来源：http://xw.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rp.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ja.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rf.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ht.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kf.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kv.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yy.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://os.yuexingan06.cn

[K05] 深拷贝对象
来源：http://pl.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://qg.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://tp.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://pt.newstarts.cn

TS:   structuredClone(obj)
来源：http://ct.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bh.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sb.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://py.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ir.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://qx.huixinmuqiang.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ag.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kz.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rf.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qv.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kx.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wd.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wk.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ib.yuntaijiaju.cn

[K07] 进制转换
来源：http://yp.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://om.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bw.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://og.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://co.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oi.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gm.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qx.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://as.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://bs.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://nl.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xx.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://hr.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://cr.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xc.nszjky.cn

Go:   encoding/gob
来源：http://dx.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://vr.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fl.nszjky.cn

================================================================================
来源：http://cz.colortex.cn

L. 网络请求
来源：http://mh.shtwfgs.cn

================================================================================
来源：http://kr.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://ah.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kg.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ox.huixiangedu.cn

JS:   await fetch(url)
来源：http://rh.shxzukj.cn

TS:   await fetch(url)
来源：http://yo.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zc.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://mu.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tk.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ou.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://rr.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wi.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bn.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wq.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uv.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nf.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lj.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fj.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oe.asd995.cn

[L03] 设置自定义请求头
来源：http://qj.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jg.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mt.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pp.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nz.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gu.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zd.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iz.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sh.colortex.cn

[L04] 设置超时
来源：http://cu.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://wh.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://si.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://li.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mp.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ny.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vy.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sv.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hy.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://bl.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gh.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://au.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://it.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xw.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://je.chemitech.net.cn


<!-- 参考信息 -->