代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xziqi.cn/gthglhqqjs.html

TS:   /error/gim
来源：http://hz.sweek.top/gtfkjvevob.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.smart0.xyz/gtnbkedato.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinghuilouyu.cn/gtiwnqpikv.html

Ruby: s.scan(/error/i)
来源：http://hz.zhongyouzk.top/gtaoqhspvw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhoulong.xyz/gteldvwlef.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sysykeji.top/gtrfpsucxt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.aizwys.cn/gthysfnygp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xinyue.icu/gtgkkrmans.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hywenlv.cn/gtrbmicyhd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gthrfsbduj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zycfv.cn/gthvwsinos.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinqigufen.top/gtmrermhhp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhengqikj.top/gtzxlzjhqj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hysaishi.cn/gtyoadcvld.html

================================================================================
来源：http://hz.zdqjudy.top/gtqeaaxkdg.html

J. 日期与时间
来源：http://hz.cheryme.top/gtedkzrgvx.html

================================================================================
来源：http://hz.gogol.net.cn/gtdxlgjvym.html

[J01] 获取当前时间
来源：http://hz.nwbrower.top/gtmsussisr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hammf.cn/gtymwlgvpo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.aizwys.cn/gtfxapbgxc.html

JS:   new Date();  Date.now()
来源：http://hz.feifeiyinyue.top/gtkmehbetv.html

TS:   new Date();  Date.now()
来源：http://hz.yvedp.cn/gtjlojopvz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tianlin.xyz/gtmeuiqger.html

Go:   time.Now()
来源：http://hz.ehwqpu.com/gtopqimvoj.html

Ruby: Time.now
来源：http://hz.vqdsnc.cn/gtmlgdfrzd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhijiandao.cn/gtkasnvbrk.html

[J02] 格式化输出
来源：http://hz.xylfe.cn/gtuifkkanq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gtlajgugsr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.fengsongda.top/gtszbziraj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xylfe.cn/gtarwvpkvq.html

TS:   d.toISOString()
来源：http://hz.gaohongyu789.top/gtmvauhpwy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ybcxt.top/gtgzezwslv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jlsjyb.cn/gtlbawrvko.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aibaodan.cn/gtdlugmzoi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xinyue.icu/gtzwxwjiyj.html

[J03] 字符串解析为日期
来源：http://hz.jlsjyb.cn/gtzzrbscuz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.316326.xyz/gtdycyzcpw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zycfv.cn/gtyanfradj.html

JS:   new Date("2024-01-02")
来源：http://hz.chenzaomai.com/gtieozugxj.html

TS:   new Date("2024-01-02")
来源：http://hz.yonumen.top/gtzaixwiwp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtmrtbsvzl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cdnleiting.top/gtzfdibckx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hfpthk.cn/gtwjnnptjj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.quarkkingdee.top/gtwxhosues.html

[J04] 时间戳与日期互转
来源：http://hz.ydjk.org.cn/gtgwsklgdo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhongyouzk.top/gtpzvpsptq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.snrcjt.cn/gtmanajjfv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ppjwa.cn/gtlftsutgg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.pengpengdd.cyou/gtluadwnnk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.daria6918.cn/gtrukjqgng.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sysykeji.top/gtfqdyayzv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.bjfxy.top/gtdtqnhttd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.mhx1999.top/gtvtqjifha.html

[J05] 时间加减（加 7 天）
来源：http://hz.gogol.net.cn/gtcaltrzfi.html

Py:   now + timedelta(days=7)
来源：http://hz.birdmap.top/gtwrdgvzyb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgufenzy.top/gtpljgjlwn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sweek.top/gtqlkstvmr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.haohaochexian.top/gtjcpxvdwx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ydjk.org.cn/gtzofeyxwp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cqqwz.cn/gtnhmyeklm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.snrcjt.cn/gtjrhowflw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ydzc1.top/gtgqmeqfwg.html

[J06] 计算两时间之差
来源：http://hz.dashuyun.cn/gtzntjyyjd.html

Py:   (end - start).total_seconds()
来源：http://hz.haohaochexian.top/gtlnqlisjv.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinyuanbaomall.cn/gtuwbglvgx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.wangshuangyany.cn/gtftzgmfdr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.daria6918.cn/gtsxzsdbje.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yanxiufei.cn/gtekecawft.html

Go:   end.Sub(start).Hours()
来源：http://hz.sufxvd.cn/gtkkqnnyml.html

Ruby: end - start                 # 返回秒数
来源：http://hz.wangdashe.top/gtwjpsfxte.html

C#:   (end - start).TotalSeconds
来源：http://hz.hnxiangtu.top/gtaqstsvmf.html

[J07] 比较两个日期
来源：http://hz.shanyushiyangkeji.top/gtgqbtjluu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtwxbkrblp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenjidiqi.icu/gteazighnu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hywenlv.cn/gthmioghrb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gtcmrlcceb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hnxiangtu.top/gtaghwonoz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yueranfly.top/gtvrsscsma.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtrkuxldls.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtxkgnicbh.html

[J08] 提取年月日与星期
来源：http://hz.hfpthk.cn/gtqyotbghb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tianlin.xyz/gtjwxqsesx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shzxlz.cn/gtbesgbjrb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangdashe.top/gtllkgtqyx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yanxiufei.cn/gtwevefelp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.guannengcc.top/gtnsvrdhkt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenlongwang.top/gthnqmndxq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.quarkkingdee.top/gtjccwmevh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sysykeji.top/gthzvotfas.html

[J09] 时区处理
来源：http://hz.yj20258.top/gttawmoxsk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenlongwang.top/gtmpmndrdi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tianlin.xyz/gttixxhbxk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gotoacloud.top/gtaoiminra.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cqqwz.cn/gtxovzdobt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jianghu66.top/gthgaaugjs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shuidangran.top/gtlfbbncjl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.wangshuangyany.cn/gtijaxikph.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yonumen.top/gtqlvqlfzx.html

[J10] 取今天 / 本月第一天
来源：http://hz.ydjk.org.cn/gtvxadztfa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shuidangran.top/gtfejeroru.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zdqjudy.top/gtmrbzdwir.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhengqikj.top/gtbgdqcqdf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yueranfly.top/gtlvznyvhq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tian-w.cn/gtmsqjxmlc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hysaishi.cn/gtumppiupx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.nanxinkj.top/gtbdhrsnwk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.meibo888.top/gtiurmbcfv.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtwuihmgsq.html

K. JSON 与序列化
来源：http://hz.chenzaomai.com/gtadjmprdw.html

================================================================================
来源：http://hz.bjfxy.top/gtfwsgflhz.html

[K01] 对象转 JSON 字符串
来源：http://hz.snrcjt.cn/gtjyxykezb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xziqi.cn/gthqfbuzjt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cheryme.top/gtvqyyiini.html

JS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gtycfzvtfv.html

TS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtbrblrzov.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tanke756.top/gtgupmngns.html

Go:   json.Marshal(obj)
来源：http://hz.gaohongyu789.top/gtgybmbxos.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhaomingkeji.xyz/gtnmcmmzxl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.redwolf501.top/gtngkyugut.html

[K02] JSON 字符串转对象
来源：http://hz.redwolf501.top/gtzmsmudcq.html

Py:   json.loads(s)
来源：http://hz.chenzaomai.com/gtxemesopn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hnqzz.top/gtnthvjyuh.html

JS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtpzpcirsz.html

TS:   JSON.parse(s)
来源：http://hz.zhixingplan.top/gtyzmjxvmv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.pycfn.com/gtqixeyfau.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.smart0.xyz/gtdmuiccdh.html

Ruby: JSON.parse(s)
来源：http://hz.xinyue.icu/gtkrctxafo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nanxuanxn.top/gtidfysscz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shzxlz.cn/gtaridogjm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.haohaochexian.top/gtofpterro.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuanzhike.top/gtuhdtubyp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtxkamjnva.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.quarkkingdee.top/gtrxlmekjp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhiwuduotai.top/gtfdfhffem.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zdqjudy.top/gtlnnorffp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ehwqpu.com/gtooatalfq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jianghu66.top/gtiusgoppe.html

[K04] 读取 JSON 文件
来源：http://hz.yongpay.top/gttfqpzljv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.fengsongda.top/gtzsheyict.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhiwuduotai.top/gtnakwavin.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhiwuduotai.top/gtehgnvzld.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.smart0.xyz/gtnhxebwsb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hnxiangtu.top/gtshrixyes.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangkeji.top/gtbecgceqs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xylfe.cn/gtypjfyvqu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.quarkkingdee.top/gtiszafwqo.html

[K05] 深拷贝对象
来源：http://hz.snrcjt.cn/gtcursmtfq.html

Py:   copy.deepcopy(obj)
来源：http://hz.jianghu66.top/gtydebttxh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.havefunace.top/gtdbcarfuz.html

JS:   structuredClone(obj)
来源：http://hz.mhx1999.top/gthqqkewwe.html

TS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtiywxexoq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.andypj.xyz/gtkjjmlqtl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cucudq.cn/gtpdhczmgt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zdqjudy.top/gteisbhusd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenzaomai.com/gtmmcmyxax.html

[K06] 解析 URL 查询串
来源：http://hz.xuanzx.com/gtewfvrjcd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.52xcode.cn/gtzzykvukb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jyoumei.cn/gttkhgqdod.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.0kj1m.cn/gtkqpeaitr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fzhhl.top/gtbyiygkxf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yuanzhike.top/gtfuycafww.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cqqwz.cn/gtygqkctxr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gaohongyu789.top/gttppxxihn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hfpthk.cn/gtkcywmcly.html

[K07] 进制转换
来源：http://hz.ivvv.top/gtzarlzvcz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.svipenyu.cn/gtecsfbchs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhijiandao.cn/gtbesfbmei.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gturtvssnt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gtyxjoekes.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtjzdvazki.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.316326.xyz/gtzasxqkgf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aizwys.cn/gtrxmkxfni.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.aizwys.cn/gtkwexyiid.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sufxvd.cn/gtbyzmrynp.html

Py:   pickle.dumps(obj)
来源：http://hz.yonumen.top/gtbxopngew.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.quarkkingdee.top/gtqskvxmvb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ehwqpu.com/gthpqnzshw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hysaishi.cn/gthffvbbei.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dashuyun.cn/gtosovojes.html

Go:   encoding/gob
来源：http://hz.pengpengdd.cyou/gtksipaqrm.html

Ruby: Marshal.dump(obj)
来源：http://hz.yuxming.cn/gtxeaburne.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.daria6918.cn/gtmzciewll.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtbabqdcud.html

L. 网络请求
来源：http://hz.wangdashe.top/gtsnegvtrh.html

================================================================================
来源：http://hz.jinqigufen.top/gtjoqfyqnv.html

[L01] 发送 GET 请求
来源：http://hz.iojbl.cn/gtysfnebpu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fengsongda.top/gtgfnsuphc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhongyouzk.top/gtupcalmsh.html

JS:   await fetch(url)
来源：http://hz.redwolf501.top/gtkfbzujqu.html

TS:   await fetch(url)
来源：http://hz.ybcxt.top/gtnaqrilql.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.feifeiyinyue.top/gtoigfsfhq.html

Go:   resp, err := http.Get(url)
来源：http://hz.xingfuxueyuan.xyz/gthxkbyhzs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.tanke756.top/gtluqegjju.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.0kj1m.cn/gtczljfaim.html

[L02] 发送 POST JSON
来源：http://hz.xinyue.icu/gtboiksfgi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinghuilouyu.cn/gtdafsylcs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yangfankeji.com/gtephwzzhk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhongyouzk.top/gthzcruplf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jyoumei.cn/gtoedvjgwe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinghuilouyu.cn/gtruryypjk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dianchejie.cn/gttpcqxcjb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj202588.top/gtwjfiyvhf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nanxinkj.top/gtpmbnqctk.html

[L03] 设置自定义请求头
来源：http://hz.ybcxt.top/gttbjjadrl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sxryk.cn/gtijicmwdi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jianghu66.top/gtzlyimqhp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gttkrfekgd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daxiang520.top/gtknxoawdh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.guannengcc.top/gtibdsqvsa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinqigfzy.top/gthtfouoip.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.pycfn.com/gtzlrzuglx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yangfankeji.com/gtekcwhxds.html

[L04] 设置超时
来源：http://hz.hnxiangtu.top/gtznpfwuiv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenzaomai.com/gtschsgtmr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tanke756.top/gthnxhuazc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.0kj1m.cn/gtpqhljftm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigufen.top/gtduqdjmhk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.guowangkeji.top/gtrjswejmu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sxryk.cn/gtfpvdasna.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gzhubu.top/gtyklnxszr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenzaomai.com/gtcniggqmm.html

[L05] 上传文件（multipart）
来源：http://hz.nanxuanxn.top/gtekngtxdi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangtech.top/gtznvjkwza.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xylfe.cn/gtexgztzbp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgfzy.top/gtqqsiibrw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.quarkkingdee.top/gtrxhxydpw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nwbrower.top/gtdypamryl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.quarkkingdee.top/gtpmsokzvr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.vqdsnc.cn/gtxayhxkgv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cheryme.top/gtjbtnlpio.html

[L06] 解析响应为 JSON
来源：http://hz.cdnleiting.top/gtsgosjnwc.html

Py:   resp.json()
来源：http://hz.sweek.top/gtlkqipffm.html

PHP:  json_decode($body, true);
来源：http://hz.aizwys.cn/gtymyjrjhr.html

JS:   await resp.json()
来源：http://hz.ivvv.top/gtzzwtsfia.html

TS:   await resp.json()
来源：http://hz.tianlin.xyz/gtrfwwcmlu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.andypj.xyz/gtctlcwmau.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sysykeji.top/gtwcnwryqh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shanyushiyangtech.top/gtswkykgws.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ehwqpu.com/gtxqnluvdg.html

[L07] 处理 HTTP 状态码
来源：http://hz.shanyushiyangtech.top/gtixnjoiqh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shangyingyoupin.top/gtkkksyfjv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhongyouzk.top/gtztvulmgv.html

JS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtmzsbetrd.html

TS:   resp.ok;  resp.status
来源：http://hz.zhaomingkeji.xyz/gtifiedesg.html

Java: resp.statusCode()
来源：http://hz.jlsjyb.cn/gtiinyware.html

Go:   resp.StatusCode
来源：http://hz.svipenyu.cn/gtowwlohcj.html

Ruby: resp.code.to_i
来源：http://hz.xuanzx.com/gtmffkicyd.html

C#:   (int)resp.StatusCode
来源：http://hz.guannengcc.top/gtyvuxluqz.html

[L08] 并发请求多个地址
来源：http://hz.chenlongwang.top/gtpkvcnrkn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hammf.cn/gtqagkemtw.html

PHP:  curl_multi_init() 系列
来源：http://hz.haohaochexian.top/gtrfbolsqm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gotoacloud.top/gtgbeecugs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jlsjyb.cn/gtamdxural.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinyuanbaomall.cn/gtykxkdfch.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shangyingyoupin.top/gtaikvjdhs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinqigfzy.top/gtfdhdxjks.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.tanke756.top/gtgbxqoxun.html

================================================================================
来源：http://hz.gzhubu.top/gtayuqmhib.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenjidiqi.icu/gtqkzmibdv.html

================================================================================
来源：http://hz.xinyue.icu/gtdxxrbyyw.html

[M01] 读取命令行参数
来源：http://hz.ydzc1.top/gtarepaszz.html

Py:   sys.argv[1:]
来源：http://hz.yanxiufei.cn/gthbmzukpj.html

PHP:  $argv;  $argc;
来源：http://hz.sufxvd.cn/gtexeiwvmd.html

JS:   process.argv.slice(2)
来源：http://hz.gaohongyu789.top/gttorjffbt.html

TS:   process.argv.slice(2)
来源：http://hz.haohaochexian.top/gtlcfuvbbe.html

Java: args 数组（main 方法参数）
来源：http://hz.shangyingyoupin.top/gtuhtezyjm.html

Go:   os.Args[1:]
来源：http://hz.shuidangran.top/gtfnkghnvy.html

Ruby: ARGV
来源：http://hz.gzhubu.top/gtxqjjalew.html

C#:   args 数组（Main 方法参数）
来源：http://hz.quarkkingdee.top/gtlzltjjrl.html

[M02] 读取环境变量
来源：http://hz.jinqigfzy.top/gtnlunfvtb.html

Py:   os.environ.get("HOME")
来源：http://hz.ywan-chungtsiang.top/gtmbvhqafy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fzhhl.top/gtnjhbfwlb.html

JS:   process.env.HOME
来源：http://hz.yj20258888.top/gtjolsvesq.html

TS:   process.env.HOME
来源：http://hz.zhengqikj.top/gtlgfprtqz.html

Java: System.getenv("HOME")
来源：http://hz.gaohongyu789.top/gtwzjhdxmr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinghuilouyu.cn/gttzlrosyx.html

Ruby: ENV["HOME"]
来源：http://hz.jqgfzy.top/gttnhsmuel.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zdqjudy.top/gtqzasdpai.html

[M03] 执行外部命令
来源：http://hz.zhengqikj.top/gtyoutnstl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nanxuanxn.top/gtthvvqgjp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yj20258.top/gtijraqcea.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.haohaochexian.top/gtlumwsacr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.snrcjt.cn/gttxyyspww.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.dashuyun.cn/gtgamrcqnl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sxryk.cn/gtporfgqdr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ehwqpu.com/gteyvzvaxd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.chenlongwang.top/gtshaixhga.html

[M04] 获取当前工作目录
来源：http://hz.iojbl.cn/gtpovxfejx.html

Py:   os.getcwd()
来源：http://hz.xuetiantiany.cn/gtftdzgugk.html

PHP:  getcwd();
来源：http://hz.jinyuanbaomall.cn/gtldgerqny.html

JS:   process.cwd()
来源：http://hz.ivvv.top/gtftsygflc.html

TS:   process.cwd()
来源：http://hz.sxryk.cn/gtoqmlrnrb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sufxvd.cn/gtxzwlodic.html

Go:   os.Getwd()
来源：http://hz.feifeiyinyue.top/gtcjxefysk.html

Ruby: Dir.pwd
来源：http://hz.fengsongda.top/gtvsrherlr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sxryk.cn/gtupxkuwuc.html

[M05] 设置退出码
来源：http://hz.meibo888.top/gtulgmzjab.html

Py:   sys.exit(1)
来源：http://hz.yuanzhike.top/gtwepctcty.html

PHP:  exit(1);
来源：http://hz.ydjk.org.cn/gttfaimiov.html


<!-- 参考信息 -->