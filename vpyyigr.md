代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://as.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dx.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://hy.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://pq.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ts.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mr.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://yl.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cr.muxihuayi.cn

[I02] 提取所有匹配
来源：http://uc.shxzukj.cn

Py:   re.findall(r"\d+", s)
来源：http://va.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oc.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gw.bjjhwx.cn

TS:   s.match(/\d+/g)
来源：http://aj.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ww.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vy.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://gv.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://su.wgjwhj.cn

[I03] 提取捕获分组
来源：http://ma.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mr.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://be.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dg.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://af.yuexingan06.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cd.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://br.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gh.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tb.nicolike.cn

[I04] 正则替换
来源：http://nq.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ts.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kk.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xy.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pk.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mk.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qf.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gc.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tx.lnxyls.cn

[I05] 按正则拆分
来源：http://cp.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xr.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jk.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://wf.lnxyls.cn

TS:   s.split(/\s*,\s*/)
来源：http://rs.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://kr.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://au.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dg.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jh.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xu.asd995.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uf.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bu.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vy.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hw.huanxung.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eh.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uc.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yg.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fn.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://dv.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zf.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ry.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yd.shxzskj.cn

TS:   /error/gim
来源：http://ik.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cy.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gs.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://qk.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ap.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://ok.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://di.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oy.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uv.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tz.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fe.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mk.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sw.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://he.jctech888.com.cn

================================================================================
来源：http://yw.panjiajie.cn

J. 日期与时间
来源：http://tm.panjiajie.cn

================================================================================
来源：http://jq.haigaiapp.cn

[J01] 获取当前时间
来源：http://cv.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xg.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uf.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://jb.nszjky.cn

TS:   new Date();  Date.now()
来源：http://fj.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ne.nszjky.cn

Go:   time.Now()
来源：http://mx.huixinmuqiang.cn

Ruby: Time.now
来源：http://cl.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zt.shxzskj.cn

[J02] 格式化输出
来源：http://gy.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ev.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ug.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ew.szsharing.cn

TS:   d.toISOString()
来源：http://ui.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qm.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ux.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dl.wgjwhj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fz.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://rq.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rj.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pv.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://ut.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://fu.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://py.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ok.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://mc.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://an.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://jq.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aw.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hm.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vt.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lp.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lx.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uq.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bw.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cp.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://ch.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://tf.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://oo.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ck.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xr.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://ns.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kv.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://kp.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cf.huanxung.cn

[J06] 计算两时间之差
来源：http://rs.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://zt.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://ep.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://as.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zb.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cj.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://cf.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://nm.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://km.bookmarksfly.cn

[J07] 比较两个日期
来源：http://xb.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://eh.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bx.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://co.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bw.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ub.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zw.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uo.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://lq.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://mm.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sb.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nh.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ao.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uf.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fn.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://af.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ms.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fh.szxytkj.cn

[J09] 时区处理
来源：http://em.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cq.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vv.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uf.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bu.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ey.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xg.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uj.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cl.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://gq.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mh.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://js.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ia.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jk.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zc.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ha.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://en.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://um.shtwfgs.cn

================================================================================
来源：http://sl.yuntaijiaju.cn

K. JSON 与序列化
来源：http://mx.bjjhwx.cn

================================================================================
来源：http://oy.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://az.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kt.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qb.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://dm.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://ex.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pe.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://ow.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sy.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vc.nszjky.cn

[K02] JSON 字符串转对象
来源：http://av.bjjhwx.cn

Py:   json.loads(s)
来源：http://ua.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wc.colortex.cn

JS:   JSON.parse(s)
来源：http://ku.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://qj.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ai.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://uy.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://pm.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lv.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://yb.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vc.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ix.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fr.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vu.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pk.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fx.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rp.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://op.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://io.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://el.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fq.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ip.gzmigu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jo.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ff.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rg.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qg.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zq.szxytkj.cn

[K05] 深拷贝对象
来源：http://jv.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://ou.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://ks.panjiajie.cn

JS:   structuredClone(obj)
来源：http://wk.nszjky.cn

TS:   structuredClone(obj)
来源：http://zh.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bo.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yw.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dq.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hm.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://ko.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wo.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://va.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ch.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ls.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dv.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ns.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://va.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://du.chemitech.net.cn

[K07] 进制转换
来源：http://cz.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yz.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sf.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kv.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ea.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tl.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dr.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tw.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ze.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://xn.colortex.cn

Py:   pickle.dumps(obj)
来源：http://xb.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sk.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://tj.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://ke.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oo.9csxet.cn

Go:   encoding/gob
来源：http://jb.521024.cn

Ruby: Marshal.dump(obj)
来源：http://ys.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ec.muxihuayi.cn

================================================================================
来源：http://qw.chemitech.net.cn

L. 网络请求
来源：http://be.shtwfgs.cn

================================================================================
来源：http://ij.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://ye.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jw.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uf.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://sz.jctech888.com.cn

TS:   await fetch(url)
来源：http://ym.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fg.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://eq.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wi.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://da.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://mu.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gz.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://st.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yr.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://os.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tm.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fg.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ox.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wf.newstarts.cn

[L03] 设置自定义请求头
来源：http://fs.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zr.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ae.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ho.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rl.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ct.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ec.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ie.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kc.jianghongdianzi.cn

[L04] 设置超时
来源：http://oc.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://wp.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gh.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eo.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tj.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yc.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pz.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ul.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ml.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://qp.9csxet.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bf.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gf.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hd.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zj.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ik.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xa.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://es.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mt.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://qo.yuntaijiaju.cn

Py:   resp.json()
来源：http://tf.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://nr.yuexingan06.cn

JS:   await resp.json()
来源：http://jq.bjjhwx.cn

TS:   await resp.json()
来源：http://mx.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tv.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vg.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://jr.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ak.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://ie.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cg.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jd.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://za.bookmarksfly.cn


<!-- 参考信息 -->