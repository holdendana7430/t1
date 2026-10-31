代发 wailian999

[I02] 提取所有匹配
来源：http://fj.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://xp.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hg.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ww.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://kq.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mc.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mf.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://vw.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ku.wgjwhj.cn

[I03] 提取捕获分组
来源：http://xn.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ii.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wf.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://em.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ji.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xr.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sh.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ae.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zh.yuntaijiaju.cn

[I04] 正则替换
来源：http://re.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gq.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ua.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://br.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ws.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ij.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wc.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zw.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rt.panjiajie.cn

[I05] 按正则拆分
来源：http://eq.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ey.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ew.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://xc.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://ot.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://lk.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aq.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fe.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nl.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uh.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vl.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://im.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ys.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://og.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yw.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ze.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ee.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ec.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://nq.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qp.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://np.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mz.colortex.cn

TS:   /error/gim
来源：http://jp.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xf.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jx.521024.cn

Ruby: s.scan(/error/i)
来源：http://ni.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lq.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://nt.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mg.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jj.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ua.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zk.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ut.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://di.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gl.chemitech.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jd.szsharing.cn

================================================================================
来源：http://du.shxzukj.cn

J. 日期与时间
来源：http://jr.huixinmuqiang.cn

================================================================================
来源：http://zc.bjjhwx.cn

[J01] 获取当前时间
来源：http://rr.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://es.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lv.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://wy.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://uq.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vn.jianghongdianzi.cn

Go:   time.Now()
来源：http://fd.shtwfgs.cn

Ruby: Time.now
来源：http://ly.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ef.bookmarksfly.cn

[J02] 格式化输出
来源：http://so.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gx.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kr.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tw.jctech888.com.cn

TS:   d.toISOString()
来源：http://vm.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gk.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yo.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wk.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rk.colortex.cn

[J03] 字符串解析为日期
来源：http://rw.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tt.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wj.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://nu.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://su.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bq.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ml.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://mn.521024.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yz.nszjky.cn

[J04] 时间戳与日期互转
来源：http://xi.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ik.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dd.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fq.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ey.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fq.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ns.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gd.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pp.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://vs.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://og.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ym.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://np.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hp.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://wr.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://si.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://oo.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sj.panjiajie.cn

[J06] 计算两时间之差
来源：http://pa.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://zz.521024.cn

PHP:  $end->diff($start)->days;
来源：http://wy.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kl.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ds.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ve.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://zu.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://np.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://we.panjiajie.cn

[J07] 比较两个日期
来源：http://cf.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://cd.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qp.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://by.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dg.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://by.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zn.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://me.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://aq.9csxet.cn

[J08] 提取年月日与星期
来源：http://bo.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bq.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jy.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://op.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ty.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mq.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://av.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nq.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zo.nicolike.cn

[J09] 时区处理
来源：http://nc.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lw.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rp.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ch.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://be.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sn.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tk.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ly.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yi.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://va.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yu.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xb.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ua.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ty.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xm.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pm.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lv.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ho.huixinmuqiang.cn

================================================================================
来源：http://hs.shxzskj.cn

K. JSON 与序列化
来源：http://sf.wgjwhj.cn

================================================================================
来源：http://ol.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://bh.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ka.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://od.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://vn.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://hl.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rq.hahajie.cn

Go:   json.Marshal(obj)
来源：http://zd.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wf.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vi.huanxung.cn

[K02] JSON 字符串转对象
来源：http://qi.nszjky.cn

Py:   json.loads(s)
来源：http://rs.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://um.nszjky.cn

JS:   JSON.parse(s)
来源：http://ww.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://ma.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sr.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://pl.hahajie.cn

Ruby: JSON.parse(s)
来源：http://iv.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sy.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://kq.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uz.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xi.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ot.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ml.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fp.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rj.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pa.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dn.hahajie.cn

[K04] 读取 JSON 文件
来源：http://pj.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://il.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wr.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://st.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zs.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wn.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ez.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vq.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://us.haigaiapp.cn

[K05] 深拷贝对象
来源：http://iw.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://as.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://nn.panjiajie.cn

JS:   structuredClone(obj)
来源：http://fl.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://dg.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://da.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gu.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mi.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://eb.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://wr.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nb.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ud.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ju.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cl.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hq.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ki.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://co.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iv.shxzskj.cn

[K07] 进制转换
来源：http://ph.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gg.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uq.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zo.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vx.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vz.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cy.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jy.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bg.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://qb.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://pz.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zk.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://xo.hahajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://iz.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://um.huixinmuqiang.cn

Go:   encoding/gob
来源：http://pc.521024.cn

Ruby: Marshal.dump(obj)
来源：http://hi.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://au.huixiangedu.cn

================================================================================
来源：http://rl.yuexingan06.cn

L. 网络请求
来源：http://fh.bjjhwx.cn

================================================================================
来源：http://je.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://it.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yv.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ul.muxihuayi.cn

JS:   await fetch(url)
来源：http://qs.huixiangedu.cn

TS:   await fetch(url)
来源：http://ki.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kj.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://ba.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xx.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yx.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://ch.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ks.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hn.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rl.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ej.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oy.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rx.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://do.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ik.shxzskj.cn

[L03] 设置自定义请求头
来源：http://pf.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uj.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zj.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://te.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bl.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://og.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jv.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rs.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bv.muxihuayi.cn

[L04] 设置超时
来源：http://dq.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://dc.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cy.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wf.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://li.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pm.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cp.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eo.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://in.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://tt.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hi.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sl.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sn.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mb.nszjky.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yt.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://en.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fc.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ag.nszjky.cn

[L06] 解析响应为 JSON
来源：http://vw.bookmarksfly.cn

Py:   resp.json()
来源：http://hd.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://jn.521024.cn

JS:   await resp.json()
来源：http://ol.huixinmuqiang.cn

TS:   await resp.json()
来源：http://du.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://br.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lo.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://pb.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fp.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://ks.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rc.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tb.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://hq.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://fc.huixiangedu.cn

Java: resp.statusCode()
来源：http://sv.jctech888.com.cn

Go:   resp.StatusCode
来源：http://yy.panjiajie.cn

Ruby: resp.code.to_i
来源：http://qs.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://fg.shxzukj.cn

[L08] 并发请求多个地址
来源：http://wh.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kv.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://zb.huixiangedu.cn


<!-- 参考信息 -->