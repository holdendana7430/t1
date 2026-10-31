代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tr.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eq.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zr.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fi.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tn.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jz.colortex.cn

[I04] 正则替换
来源：http://vd.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dh.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ww.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tr.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rs.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jl.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qu.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pk.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zx.newstarts.cn

[I05] 按正则拆分
来源：http://fg.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hm.521024.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pe.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://td.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://pj.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://ho.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qp.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nw.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jn.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jl.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ow.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zr.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ib.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ad.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sx.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cl.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ef.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qq.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://qy.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://up.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nj.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yk.huanxung.cn

TS:   /error/gim
来源：http://mr.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fm.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qp.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://un.szsharing.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mc.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://tb.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jg.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ot.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ei.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ap.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oj.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sw.szxytkj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hj.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kc.gzmigu.cn

================================================================================
来源：http://vh.chemitech.net.cn

J. 日期与时间
来源：http://ge.hahajie.cn

================================================================================
来源：http://da.shxzskj.cn

[J01] 获取当前时间
来源：http://da.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://au.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ft.lnxyls.cn

JS:   new Date();  Date.now()
来源：http://bj.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://tc.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hr.panjiajie.cn

Go:   time.Now()
来源：http://jl.9csxet.cn

Ruby: Time.now
来源：http://zy.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lp.szxytkj.cn

[J02] 格式化输出
来源：http://en.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qb.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nm.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ek.hahajie.cn

TS:   d.toISOString()
来源：http://xm.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bd.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yp.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ie.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yt.shxzskj.cn

[J03] 字符串解析为日期
来源：http://gs.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://os.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oq.521024.cn

JS:   new Date("2024-01-02")
来源：http://tp.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://dh.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wy.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://az.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://nx.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yz.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://ea.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ov.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hq.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yq.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sq.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nl.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vn.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ut.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xk.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://nf.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://ur.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wr.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dc.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oe.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://js.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fq.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://se.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gh.shxzskj.cn

[J06] 计算两时间之差
来源：http://lc.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://ro.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://zw.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gq.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xt.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dp.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://ou.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://pg.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://ck.colortex.cn

[J07] 比较两个日期
来源：http://py.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://ir.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ow.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lh.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rg.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://is.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ul.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jk.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://jd.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://he.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lh.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tn.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://az.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zo.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://st.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sj.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ed.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wf.nicolike.cn

[J09] 时区处理
来源：http://ie.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ue.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://za.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ad.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oo.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rh.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yy.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fz.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tw.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://qq.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uo.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jj.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gb.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zs.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ut.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dq.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zw.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gp.haigaiapp.cn

================================================================================
来源：http://ei.newstarts.cn

K. JSON 与序列化
来源：http://zd.gzmigu.cn

================================================================================
来源：http://vm.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://tk.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://og.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://be.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://ah.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://pd.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sf.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://bc.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cv.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hr.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://rx.9csxet.cn

Py:   json.loads(s)
来源：http://ad.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cy.szsharing.cn

JS:   JSON.parse(s)
来源：http://af.shxzukj.cn

TS:   JSON.parse(s)
来源：http://nd.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mk.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://rz.huanxung.cn

Ruby: JSON.parse(s)
来源：http://ch.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dr.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ic.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bm.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vm.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ql.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ft.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vh.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tn.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oo.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pc.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://ev.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zl.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ay.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zw.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uc.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xo.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kl.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bz.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jm.szsharing.cn

[K05] 深拷贝对象
来源：http://vs.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://ht.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://li.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://la.gzmigu.cn

TS:   structuredClone(obj)
来源：http://wy.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ac.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ul.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jy.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ts.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://om.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fo.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ov.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nd.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sc.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ev.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tn.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wt.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cj.shxzskj.cn

[K07] 进制转换
来源：http://gj.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xn.chemitech.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ap.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://du.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gb.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fa.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dy.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qr.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://af.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://pa.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://pd.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://od.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://rh.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://tk.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ph.gzmigu.cn

Go:   encoding/gob
来源：http://zy.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://pv.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nu.hnjuh.cn

================================================================================
来源：http://ic.yuexingan06.cn

L. 网络请求
来源：http://em.shxzskj.cn

================================================================================
来源：http://me.shxzskj.cn

[L01] 发送 GET 请求
来源：http://ur.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ed.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ab.shxzskj.cn

JS:   await fetch(url)
来源：http://aa.gzmigu.cn

TS:   await fetch(url)
来源：http://rl.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hl.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://gp.asd995.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ch.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bw.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://sc.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gt.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xi.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qm.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gr.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ap.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vw.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jj.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uy.521024.cn

[L03] 设置自定义请求头
来源：http://es.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yo.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://te.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nx.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kk.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mz.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tv.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iz.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kp.yuexingan06.cn

[L04] 设置超时
来源：http://kt.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://kk.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qz.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wu.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yc.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kt.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dc.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://we.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gf.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://kf.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bs.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ae.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pp.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pv.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pe.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wl.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://em.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oj.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://je.lnxyls.cn

Py:   resp.json()
来源：http://uk.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://bz.chemitech.net.cn

JS:   await resp.json()
来源：http://oj.bookmarksfly.cn

TS:   await resp.json()
来源：http://qr.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xe.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oo.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://fo.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uq.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://hb.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bp.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sr.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://ww.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://os.nszjky.cn

Java: resp.statusCode()
来源：http://fp.muxihuayi.cn

Go:   resp.StatusCode
来源：http://mf.newstarts.cn

Ruby: resp.code.to_i
来源：http://yg.521024.cn

C#:   (int)resp.StatusCode
来源：http://pr.nicolike.cn

[L08] 并发请求多个地址
来源：http://bm.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ce.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://cv.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vi.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sp.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://we.yuntaijiaju.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oy.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ec.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cs.szsharing.cn

================================================================================
来源：http://kb.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://bm.huixiangedu.cn

================================================================================
来源：http://vv.wgjwhj.cn

[M01] 读取命令行参数
来源：http://yf.521024.cn

Py:   sys.argv[1:]
来源：http://oy.hahajie.cn

PHP:  $argv;  $argc;
来源：http://gj.nicolike.cn


<!-- 参考信息 -->