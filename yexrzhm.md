代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://go.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gk.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hp.shxzukj.cn

[H10] 资源自动释放
来源：http://hk.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cp.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uu.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vi.hnjuh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qn.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lm.chemitech.net.cn

Go:   defer f.Close()
来源：http://em.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://il.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ni.hnjuh.cn

================================================================================
来源：http://ja.shxzukj.cn

I. 正则表达式
来源：http://fy.9csxet.cn

================================================================================
来源：http://oe.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://db.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://da.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eh.colortex.cn

JS:   /\d+/.test(s)
来源：http://ol.szsharing.cn

TS:   /\d+/.test(s)
来源：http://cv.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nq.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ct.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://rt.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jg.bjjhwx.cn

[I02] 提取所有匹配
来源：http://lx.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://qf.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vk.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lz.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://fr.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://op.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tz.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://xs.muxihuayi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bn.haigaiapp.cn

[I03] 提取捕获分组
来源：http://up.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://he.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sn.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bv.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fh.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fk.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pv.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zm.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ij.jctech888.com.cn

[I04] 正则替换
来源：http://fr.yuexingan06.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://po.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sd.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pk.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ah.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yj.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oq.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uu.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ql.asd995.cn

[I05] 按正则拆分
来源：http://mx.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wa.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://om.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://gg.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ci.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://la.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ip.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vv.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ke.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lz.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hi.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jn.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ea.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://op.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://er.yuntaijiaju.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qe.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mj.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tj.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://mo.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ke.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lf.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tw.nszjky.cn

TS:   /error/gim
来源：http://oz.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ia.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ne.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://lh.521024.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ug.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://ae.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qw.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pw.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rw.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nq.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://db.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qf.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dk.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sy.jctech888.com.cn

================================================================================
来源：http://pq.haigaiapp.cn

J. 日期与时间
来源：http://xr.bookmarksfly.cn

================================================================================
来源：http://lp.muxihuayi.cn

[J01] 获取当前时间
来源：http://xe.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fd.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mt.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://hs.szsharing.cn

TS:   new Date();  Date.now()
来源：http://ag.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dd.yuexingan06.cn

Go:   time.Now()
来源：http://mi.haigaiapp.cn

Ruby: Time.now
来源：http://pd.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hc.haigaiapp.cn

[J02] 格式化输出
来源：http://ux.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rd.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://li.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lo.nszjky.cn

TS:   d.toISOString()
来源：http://rl.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sb.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zu.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tt.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zg.hahajie.cn

[J03] 字符串解析为日期
来源：http://vq.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tg.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pr.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://jk.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://pu.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hl.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hv.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://sj.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oq.521024.cn

[J04] 时间戳与日期互转
来源：http://av.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kn.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ok.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wj.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wv.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ps.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gv.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gb.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cf.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://ci.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://yy.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ke.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wm.bookmarksfly.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://li.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://xr.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://po.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://pr.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tn.nszjky.cn

[J06] 计算两时间之差
来源：http://xv.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://dq.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://ed.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eu.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kw.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xf.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://lo.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://qd.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://km.gzmigu.cn

[J07] 比较两个日期
来源：http://hx.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://so.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oo.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pe.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jq.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zp.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vw.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cm.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://ge.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://gj.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fz.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oj.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hg.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zh.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://np.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tt.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tp.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gn.muxihuayi.cn

[J09] 时区处理
来源：http://ea.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ot.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nv.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tq.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wv.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ry.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uu.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ni.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://so.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://kt.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://au.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sy.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cn.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dn.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hm.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://we.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ib.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ao.chemitech.net.cn

================================================================================
来源：http://ki.asd995.cn

K. JSON 与序列化
来源：http://qq.muxihuayi.cn

================================================================================
来源：http://fz.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://xx.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ht.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cb.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://br.huanxung.cn

TS:   JSON.stringify(obj)
来源：http://qw.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iv.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://bg.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zb.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zg.huanxung.cn

[K02] JSON 字符串转对象
来源：http://bp.muxihuayi.cn

Py:   json.loads(s)
来源：http://ie.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ek.hahajie.cn

JS:   JSON.parse(s)
来源：http://lb.szsharing.cn

TS:   JSON.parse(s)
来源：http://nb.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oj.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://qv.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://mg.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jy.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://dz.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kw.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tj.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ov.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ax.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://es.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jl.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dl.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fk.521024.cn

[K04] 读取 JSON 文件
来源：http://qk.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hf.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ke.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tn.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mw.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vd.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ot.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dg.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yu.chemitech.net.cn

[K05] 深拷贝对象
来源：http://ql.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://de.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://gr.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://hk.panjiajie.cn

TS:   structuredClone(obj)
来源：http://hp.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://st.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hr.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cw.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xn.nicolike.cn

[K06] 解析 URL 查询串
来源：http://ax.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rx.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sb.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hy.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tf.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fj.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cc.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pc.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xv.huixiangedu.cn

[K07] 进制转换
来源：http://bo.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ie.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ue.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gc.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yt.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rr.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://at.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ym.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jr.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://rf.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://go.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wy.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://nq.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://uh.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pf.9csxet.cn

Go:   encoding/gob
来源：http://gf.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://mp.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yt.chemitech.net.cn

================================================================================
来源：http://qo.yuexingan06.cn

L. 网络请求
来源：http://hf.shxzskj.cn

================================================================================
来源：http://cx.szxytkj.cn

[L01] 发送 GET 请求
来源：http://ox.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xg.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mq.bookmarksfly.cn

JS:   await fetch(url)
来源：http://nj.chemitech.net.cn

TS:   await fetch(url)
来源：http://zq.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gc.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://lv.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ru.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cu.hnjuh.cn

[L02] 发送 POST JSON
来源：http://po.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://to.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zj.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vn.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ti.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ma.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ud.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qi.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hg.shxzskj.cn

[L03] 设置自定义请求头
来源：http://jk.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xc.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xe.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qr.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jl.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lj.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rw.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rq.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kb.huixiangedu.cn

[L04] 设置超时
来源：http://cj.jianghongdianzi.cn

Py:   requests.get(url, timeout=5)
来源：http://lg.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yz.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gg.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uh.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ch.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ec.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gt.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://si.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://io.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ei.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vl.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tt.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gn.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rg.hnjuh.cn


<!-- 参考信息 -->