代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uy.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kp.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://ic.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ld.haigaiapp.cn

[I02] 提取所有匹配
来源：http://yt.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://pz.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jb.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jn.bjjhwx.cn

TS:   s.match(/\d+/g)
来源：http://bd.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jn.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ls.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://uv.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wz.huanxung.cn

[I03] 提取捕获分组
来源：http://zp.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://va.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hx.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uh.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fe.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hd.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vz.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zs.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vt.szsharing.cn

[I04] 正则替换
来源：http://ov.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ow.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://la.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dp.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://px.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://om.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ya.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bj.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fd.jctech888.com.cn

[I05] 按正则拆分
来源：http://tq.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pl.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kf.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://cp.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://zq.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://bq.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mq.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zj.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jx.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qd.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ah.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yl.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gr.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://te.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ht.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sa.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bq.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ic.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://ld.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zn.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eb.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ss.huixiangedu.cn

TS:   /error/gim
来源：http://tr.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cq.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mq.asd995.cn

Ruby: s.scan(/error/i)
来源：http://xs.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xn.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ut.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ng.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vd.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qy.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yz.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eq.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gr.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://su.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xd.szxytkj.cn

================================================================================
来源：http://mu.szxytkj.cn

J. 日期与时间
来源：http://pb.newstarts.cn

================================================================================
来源：http://jt.szxytkj.cn

[J01] 获取当前时间
来源：http://ok.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dd.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zh.newstarts.cn

JS:   new Date();  Date.now()
来源：http://vd.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://jx.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gi.muxihuayi.cn

Go:   time.Now()
来源：http://re.gzmigu.cn

Ruby: Time.now
来源：http://dc.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wt.9csxet.cn

[J02] 格式化输出
来源：http://ag.muxihuayi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nn.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vm.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nj.jctech888.com.cn

TS:   d.toISOString()
来源：http://sk.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zr.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://be.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eh.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ia.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://xn.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oe.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kw.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://sm.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://uf.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yg.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ki.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://po.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ip.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://jh.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://en.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rj.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ct.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dq.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bx.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nj.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ot.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sx.521024.cn

[J05] 时间加减（加 7 天）
来源：http://nt.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://bb.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kt.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pw.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gf.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://xx.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://be.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://bq.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bz.wgjwhj.cn

[J06] 计算两时间之差
来源：http://fm.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://qd.521024.cn

PHP:  $end->diff($start)->days;
来源：http://sb.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bc.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fz.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tz.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://ej.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://qn.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://yl.shtwfgs.cn

[J07] 比较两个日期
来源：http://xc.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://qf.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://md.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hy.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nh.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ec.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hx.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ud.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://kc.colortex.cn

[J08] 提取年月日与星期
来源：http://wc.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oy.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xs.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ei.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fa.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://df.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://il.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xn.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dz.9csxet.cn

[J09] 时区处理
来源：http://pk.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qv.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://st.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://im.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ks.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wh.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rv.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gu.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fh.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://bp.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zd.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vc.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vf.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mj.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ph.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://em.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ie.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rf.panjiajie.cn

================================================================================
来源：http://yi.huixiangedu.cn

K. JSON 与序列化
来源：http://nx.chemitech.net.cn

================================================================================
来源：http://jh.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://ki.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://em.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ik.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://ce.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://bx.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vh.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://gy.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://be.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rz.9csxet.cn

[K02] JSON 字符串转对象
来源：http://bu.shxzukj.cn

Py:   json.loads(s)
来源：http://ku.huixiangedu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://at.9csxet.cn

JS:   JSON.parse(s)
来源：http://xt.shxzskj.cn

TS:   JSON.parse(s)
来源：http://ro.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pt.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://pn.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://rx.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xr.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://kk.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zd.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nb.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lz.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://br.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nz.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wo.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://td.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gm.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://ji.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ig.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kc.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://le.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ht.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sb.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oc.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://av.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ae.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://jo.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://fj.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://bb.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://fb.szsharing.cn

TS:   structuredClone(obj)
来源：http://iq.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://aw.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://df.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fc.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ea.asd995.cn

[K06] 解析 URL 查询串
来源：http://sn.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cw.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://er.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wd.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yo.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ba.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ol.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ik.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hu.shxzskj.cn

[K07] 进制转换
来源：http://kh.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ol.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oq.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tq.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://js.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ce.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://al.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bd.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bc.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://jk.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://ah.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sj.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://fa.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://gh.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vz.shtwfgs.cn

Go:   encoding/gob
来源：http://an.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://lh.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bq.shxzskj.cn

================================================================================
来源：http://xv.gzmigu.cn

L. 网络请求
来源：http://ub.lnxyls.cn

================================================================================
来源：http://rk.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://re.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lr.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ge.szsharing.cn

JS:   await fetch(url)
来源：http://go.bjjhwx.cn

TS:   await fetch(url)
来源：http://ei.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oq.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://uy.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yx.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tq.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://aw.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fu.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ol.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ep.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mt.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dr.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jn.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ri.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vc.shxzskj.cn

[L03] 设置自定义请求头
来源：http://wk.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://co.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uy.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sn.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yp.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zf.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://id.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ax.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ax.bjjhwx.cn

[L04] 设置超时
来源：http://ll.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://rb.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hy.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fg.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gk.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tl.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ai.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yi.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dn.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://jr.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zy.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://om.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gu.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qw.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fw.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cf.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ld.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ow.nszjky.cn

[L06] 解析响应为 JSON
来源：http://wt.huixiangedu.cn

Py:   resp.json()
来源：http://ut.colortex.cn

PHP:  json_decode($body, true);
来源：http://lw.bjjhwx.cn

JS:   await resp.json()
来源：http://gw.shxzukj.cn

TS:   await resp.json()
来源：http://cw.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rd.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cn.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://mr.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bx.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://fj.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mm.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://be.huanxung.cn

JS:   resp.ok;  resp.status
来源：http://fd.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://la.szxytkj.cn

Java: resp.statusCode()
来源：http://vw.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://bz.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://kd.shtwfgs.cn


<!-- 参考信息 -->