代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://js.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nq.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ek.hnjuh.cn

[H10] 资源自动释放
来源：http://tq.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cv.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oi.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cf.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dh.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vs.shxzskj.cn

Go:   defer f.Close()
来源：http://oa.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jq.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ok.jctech888.com.cn

================================================================================
来源：http://wo.huixinmuqiang.cn

I. 正则表达式
来源：http://xh.panjiajie.cn

================================================================================
来源：http://zd.yuexingan06.cn

[I01] 判断是否匹配
来源：http://pi.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pv.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eu.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://yn.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://ke.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ef.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ji.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://es.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://re.gzmigu.cn

[I02] 提取所有匹配
来源：http://if.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://jk.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cl.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hk.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://rj.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xd.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qp.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://di.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qc.colortex.cn

[I03] 提取捕获分组
来源：http://pa.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mf.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://an.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lj.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jn.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fy.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vh.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fn.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://er.colortex.cn

[I04] 正则替换
来源：http://bc.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ky.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rk.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://do.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pj.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wm.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xg.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://er.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lt.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://nl.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://do.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ax.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://cy.lnxyls.cn

TS:   s.split(/\s*,\s*/)
来源：http://ve.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://la.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zj.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xv.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fh.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ob.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oy.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vc.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vr.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aw.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ot.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hs.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qq.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ty.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://fv.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yq.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tl.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ze.yuexingan06.cn

TS:   /error/gim
来源：http://yn.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iv.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hv.asd995.cn

Ruby: s.scan(/error/i)
来源：http://ur.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wc.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://uo.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tk.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qt.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pj.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vl.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bq.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iy.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://js.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tw.9csxet.cn

================================================================================
来源：http://is.yuntaijiaju.cn

J. 日期与时间
来源：http://gy.jianghongdianzi.cn

================================================================================
来源：http://fp.521024.cn

[J01] 获取当前时间
来源：http://kv.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cw.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://og.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://ne.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://nr.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zs.szxytkj.cn

Go:   time.Now()
来源：http://np.huixiangedu.cn

Ruby: Time.now
来源：http://jn.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uy.huanxung.cn

[J02] 格式化输出
来源：http://np.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kk.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://px.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cl.9csxet.cn

TS:   d.toISOString()
来源：http://fq.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nt.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yo.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ou.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lu.nicolike.cn

[J03] 字符串解析为日期
来源：http://jv.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ab.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ft.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://ck.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://mn.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fi.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bj.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://qk.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zc.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://cd.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tc.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rs.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://za.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yy.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xc.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kz.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cy.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fy.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://it.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://av.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gx.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gf.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://te.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://ni.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ea.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://zw.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ic.shxzskj.cn

[J06] 计算两时间之差
来源：http://wm.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://zz.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://fh.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gs.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yb.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ax.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://td.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://ag.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://wt.lnxyls.cn

[J07] 比较两个日期
来源：http://lx.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://ac.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ga.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qr.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tw.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://va.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qe.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://oe.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://zo.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://xc.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xj.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lj.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kv.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ug.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pk.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ib.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ud.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lj.nicolike.cn

[J09] 时区处理
来源：http://zs.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sa.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mu.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uu.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://td.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ic.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jj.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ht.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jz.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://kh.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kc.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iq.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hf.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sj.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qg.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sh.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kc.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zs.lnxyls.cn

================================================================================
来源：http://lg.jctech888.com.cn

K. JSON 与序列化
来源：http://yk.jianghongdianzi.cn

================================================================================
来源：http://vl.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://hw.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tt.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qr.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://yf.asd995.cn

TS:   JSON.stringify(obj)
来源：http://gg.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kw.nszjky.cn

Go:   json.Marshal(obj)
来源：http://og.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fz.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vw.colortex.cn

[K02] JSON 字符串转对象
来源：http://bg.bjjhwx.cn

Py:   json.loads(s)
来源：http://rl.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wl.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://fa.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://eg.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nl.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://qc.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://al.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hr.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://dg.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ws.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tt.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vc.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bf.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vj.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vu.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jx.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rw.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://cd.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vk.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bq.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yc.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mg.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fs.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xm.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fh.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kv.panjiajie.cn

[K05] 深拷贝对象
来源：http://do.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://ew.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://up.szxytkj.cn

JS:   structuredClone(obj)
来源：http://xw.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://gr.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://og.hnjuh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xj.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zf.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bj.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://ev.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rz.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lr.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xp.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kk.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qm.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ko.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ep.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ly.9csxet.cn

[K07] 进制转换
来源：http://jc.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vy.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://me.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wv.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yh.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pu.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mt.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://do.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hp.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://bi.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://yr.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gu.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://oi.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://eu.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vx.muxihuayi.cn

Go:   encoding/gob
来源：http://be.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://uu.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pb.wgjwhj.cn

================================================================================
来源：http://zl.muxihuayi.cn

L. 网络请求
来源：http://qm.gzmigu.cn

================================================================================
来源：http://zp.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://wd.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vi.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vn.jctech888.com.cn

JS:   await fetch(url)
来源：http://ft.hahajie.cn

TS:   await fetch(url)
来源：http://yw.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vo.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://uc.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sn.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zi.nicolike.cn

[L02] 发送 POST JSON
来源：http://cf.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uv.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tu.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aa.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qs.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://de.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qd.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gi.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kk.newstarts.cn

[L03] 设置自定义请求头
来源：http://ve.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fa.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ak.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lu.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vq.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://el.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://um.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fw.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sx.nszjky.cn

[L04] 设置超时
来源：http://ui.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://pi.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jr.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cw.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://df.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bx.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yi.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sg.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yz.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://go.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lc.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zf.nszjky.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jq.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hs.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ci.newstarts.cn


<!-- 参考信息 -->