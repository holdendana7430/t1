代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://py.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rg.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bw.521024.cn

[H10] 资源自动释放
来源：http://tz.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vd.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://is.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yj.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://te.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lb.bjjhwx.cn

Go:   defer f.Close()
来源：http://vs.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xt.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qd.jctech888.com.cn

================================================================================
来源：http://aq.huixiangedu.cn

I. 正则表达式
来源：http://hq.nicolike.cn

================================================================================
来源：http://du.shtwfgs.cn

[I01] 判断是否匹配
来源：http://nm.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fk.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jc.nicolike.cn

JS:   /\d+/.test(s)
来源：http://cl.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://hj.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ut.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uj.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://qk.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wi.szxytkj.cn

[I02] 提取所有匹配
来源：http://wu.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://rs.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://us.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zb.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://ds.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mu.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vr.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://mr.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mg.jctech888.com.cn

[I03] 提取捕获分组
来源：http://lx.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uv.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vp.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hl.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xs.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wf.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pd.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zs.muxihuayi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://af.yuntaijiaju.cn

[I04] 正则替换
来源：http://et.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ji.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jc.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pu.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zl.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vl.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://he.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jj.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dh.colortex.cn

[I05] 按正则拆分
来源：http://qv.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zp.colortex.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ur.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://ip.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://al.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://de.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fi.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pk.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jm.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ia.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kp.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sn.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rl.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xo.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sk.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tu.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lk.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://po.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://sx.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vd.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vm.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cs.huixiangedu.cn

TS:   /error/gim
来源：http://tr.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qf.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ow.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://zk.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zq.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://jo.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://im.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mf.shxzukj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qu.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rz.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://px.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sg.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wj.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qj.wgjwhj.cn

================================================================================
来源：http://wd.hnjuh.cn

J. 日期与时间
来源：http://vs.shxzskj.cn

================================================================================
来源：http://fc.huixiangedu.cn

[J01] 获取当前时间
来源：http://ap.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cm.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ob.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://xl.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://zw.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://he.huanxung.cn

Go:   time.Now()
来源：http://bk.9csxet.cn

Ruby: Time.now
来源：http://ix.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pk.hahajie.cn

[J02] 格式化输出
来源：http://yv.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lh.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nt.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nc.haigaiapp.cn

TS:   d.toISOString()
来源：http://zu.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rs.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tx.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://au.wgjwhj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sn.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://yd.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xt.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qq.colortex.cn

JS:   new Date("2024-01-02")
来源：http://os.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://qi.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gg.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mf.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://pf.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ic.nszjky.cn

[J04] 时间戳与日期互转
来源：http://dl.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sb.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sh.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sw.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://do.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vg.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sa.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ay.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ve.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://zm.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://pe.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yz.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xv.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://co.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://jq.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sd.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://iw.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ls.szxytkj.cn

[J06] 计算两时间之差
来源：http://li.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://qg.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://yt.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nd.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pb.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://la.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://bj.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://gk.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://un.lnxyls.cn

[J07] 比较两个日期
来源：http://wp.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://lh.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dn.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kh.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ut.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://an.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kh.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://eb.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://br.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://yi.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mq.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ao.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://or.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fw.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yz.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dn.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://be.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rc.panjiajie.cn

[J09] 时区处理
来源：http://tk.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ep.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://km.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ja.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gx.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ch.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wg.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jg.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qr.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://qz.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ib.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pq.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://di.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tj.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ca.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pd.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://du.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qt.yuntaijiaju.cn

================================================================================
来源：http://jr.hahajie.cn

K. JSON 与序列化
来源：http://hi.shtwfgs.cn

================================================================================
来源：http://pv.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://an.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pm.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kg.colortex.cn

JS:   JSON.stringify(obj)
来源：http://as.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://ig.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://et.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://cl.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gg.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pa.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://ig.bookmarksfly.cn

Py:   json.loads(s)
来源：http://rn.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tw.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://xk.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://yh.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nt.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://mz.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://nb.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kd.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://rd.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://we.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cz.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ch.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sk.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lq.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://af.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ht.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kv.521024.cn

[K04] 读取 JSON 文件
来源：http://ie.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xk.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://es.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bw.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://px.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fq.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ts.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kx.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lf.asd995.cn

[K05] 深拷贝对象
来源：http://ec.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://xf.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://al.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://bx.asd995.cn

TS:   structuredClone(obj)
来源：http://sd.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ty.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://de.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vs.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fb.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://hh.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://an.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bj.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uz.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wm.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uu.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sa.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://im.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://db.panjiajie.cn

[K07] 进制转换
来源：http://hy.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hq.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://py.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://id.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ry.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nm.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ti.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dd.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vc.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://xg.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://lu.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ob.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://fe.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://as.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ka.newstarts.cn

Go:   encoding/gob
来源：http://co.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://av.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tv.szsharing.cn

================================================================================
来源：http://gu.newstarts.cn

L. 网络请求
来源：http://cu.hahajie.cn

================================================================================
来源：http://pp.colortex.cn

[L01] 发送 GET 请求
来源：http://ag.shxzukj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qn.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ib.hnjuh.cn

JS:   await fetch(url)
来源：http://xm.huanxung.cn

TS:   await fetch(url)
来源：http://fl.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sj.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://ky.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rz.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tk.colortex.cn

[L02] 发送 POST JSON
来源：http://nb.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://eu.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ta.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zk.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dc.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gx.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://px.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ai.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oh.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://cb.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qv.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vq.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bt.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dd.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jn.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ok.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bf.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lh.muxihuayi.cn

[L04] 设置超时
来源：http://ad.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://tu.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uo.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ha.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ut.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nt.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zo.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xd.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jx.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://go.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aj.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zk.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mv.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oc.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uj.huixiangedu.cn


<!-- 参考信息 -->