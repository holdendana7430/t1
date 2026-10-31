代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lp.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://bp.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jb.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ut.jctech888.com.cn

================================================================================
来源：http://mp.shxzskj.cn

I. 正则表达式
来源：http://nm.shxzukj.cn

================================================================================
来源：http://gr.colortex.cn

[I01] 判断是否匹配
来源：http://dx.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pn.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lp.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://py.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://oj.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bz.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dq.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://uo.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yb.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://jc.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://yp.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cy.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hn.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://os.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qu.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ti.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://qu.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oi.shtwfgs.cn

[I03] 提取捕获分组
来源：http://um.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zt.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://of.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nh.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qk.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rh.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://az.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tg.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://om.muxihuayi.cn

[I04] 正则替换
来源：http://rp.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qs.huanxung.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nm.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vh.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hk.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zh.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jw.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pc.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jq.gzmigu.cn

[I05] 按正则拆分
来源：http://jk.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fi.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nj.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://iw.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://wv.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://ic.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xo.nicolike.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rm.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mb.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pc.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ck.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dj.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yt.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nv.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aa.hahajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jj.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://np.hnjuh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sz.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://cv.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yf.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hn.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://be.hnjuh.cn

TS:   /error/gim
来源：http://as.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zy.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fk.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://qa.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mg.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://yc.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zs.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gf.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dw.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ed.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://di.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mo.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nw.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ci.colortex.cn

================================================================================
来源：http://gp.muxihuayi.cn

J. 日期与时间
来源：http://uv.gzmigu.cn

================================================================================
来源：http://ma.shxzskj.cn

[J01] 获取当前时间
来源：http://vm.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ji.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gp.nszjky.cn

JS:   new Date();  Date.now()
来源：http://ze.nszjky.cn

TS:   new Date();  Date.now()
来源：http://ef.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bl.9csxet.cn

Go:   time.Now()
来源：http://pm.shxzskj.cn

Ruby: Time.now
来源：http://cz.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gs.hahajie.cn

[J02] 格式化输出
来源：http://yf.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lh.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bb.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ym.nszjky.cn

TS:   d.toISOString()
来源：http://zj.colortex.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://du.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vv.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qi.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jk.shxzukj.cn

[J03] 字符串解析为日期
来源：http://qq.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://np.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bz.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://rr.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://gl.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://st.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ov.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://tu.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ay.nicolike.cn

[J04] 时间戳与日期互转
来源：http://zs.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ii.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gi.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zb.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jq.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qh.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sp.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ih.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ak.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://ho.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://tr.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iz.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tk.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ps.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://vc.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bz.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://ux.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ia.shxzukj.cn

[J06] 计算两时间之差
来源：http://zu.asd995.cn

Py:   (end - start).total_seconds()
来源：http://ip.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://fn.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ms.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nl.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ht.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://re.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://bn.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://gp.bjjhwx.cn

[J07] 比较两个日期
来源：http://dg.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://ty.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ei.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yo.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nq.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jl.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tb.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vo.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://on.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://fl.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uy.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yx.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ae.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mc.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ih.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dd.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nn.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wq.bookmarksfly.cn

[J09] 时区处理
来源：http://hz.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gd.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mo.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ui.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lu.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ev.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qi.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cl.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sc.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://ea.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nt.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gf.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://td.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ub.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://be.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ug.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kd.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dh.haigaiapp.cn

================================================================================
来源：http://jz.nicolike.cn

K. JSON 与序列化
来源：http://vc.yuexingan06.cn

================================================================================
来源：http://wm.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://pf.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ge.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://km.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://mt.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://it.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dj.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://lc.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nm.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uf.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://co.muxihuayi.cn

Py:   json.loads(s)
来源：http://bq.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sy.521024.cn

JS:   JSON.parse(s)
来源：http://bc.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://az.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nh.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://mo.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://rs.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://io.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://xu.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xv.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yt.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://od.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tp.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uu.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ts.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yl.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nf.hahajie.cn

[K04] 读取 JSON 文件
来源：http://pe.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nk.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fr.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://db.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://or.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fq.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pm.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://op.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iz.haigaiapp.cn

[K05] 深拷贝对象
来源：http://ya.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://ow.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://dl.gzmigu.cn

JS:   structuredClone(obj)
来源：http://jw.colortex.cn

TS:   structuredClone(obj)
来源：http://tz.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ik.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://as.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nl.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ew.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://ya.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mz.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ok.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://us.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nh.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lu.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xn.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zj.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cm.yuntaijiaju.cn

[K07] 进制转换
来源：http://sj.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qe.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wu.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gl.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tt.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nz.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fa.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lx.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tt.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://kt.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://gv.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dw.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://ul.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://yn.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://re.jianghongdianzi.cn

Go:   encoding/gob
来源：http://se.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://fb.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pc.huixiangedu.cn

================================================================================
来源：http://vj.colortex.cn

L. 网络请求
来源：http://up.9csxet.cn

================================================================================
来源：http://wk.9csxet.cn

[L01] 发送 GET 请求
来源：http://tu.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wr.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qe.chemitech.net.cn

JS:   await fetch(url)
来源：http://js.muxihuayi.cn

TS:   await fetch(url)
来源：http://si.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jg.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://yb.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xm.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ld.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://jq.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ml.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dz.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://to.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iz.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ms.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hf.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://al.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cs.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://ee.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yr.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jm.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ta.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vt.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xl.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://op.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://or.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ne.nszjky.cn

[L04] 设置超时
来源：http://wg.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://hh.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ht.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fk.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://te.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bz.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rq.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vr.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rf.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://gz.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vr.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ju.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lo.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://el.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qq.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pu.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yg.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xd.huanxung.cn

[L06] 解析响应为 JSON
来源：http://te.lnxyls.cn

Py:   resp.json()
来源：http://dv.colortex.cn

PHP:  json_decode($body, true);
来源：http://oo.asd995.cn

JS:   await resp.json()
来源：http://om.jianghongdianzi.cn

TS:   await resp.json()
来源：http://qf.yuntaijiaju.cn


<!-- 参考信息 -->