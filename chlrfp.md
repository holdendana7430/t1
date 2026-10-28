代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daxiang520.top/gterjqqcpt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gtglkrplio.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtltouegeh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtotqtkcvb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinyuanbaomall.cn/gtqqvdzhbf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yuanzhike.top/gtjdaqzdad.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.9152youxi.cn/gtgmcqyosx.html

================================================================================
来源：http://hz.xuanzx.com/gtpjruuvoj.html

J. 日期与时间
来源：http://hz.aibaodan.cn/gthxawgmva.html

================================================================================
来源：http://hz.andypj.xyz/gtreaaygmz.html

[J01] 获取当前时间
来源：http://hz.nanxinkj.top/gtnyykdnqs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xuetiantiany.cn/gtkamcasds.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shuidangran.top/gtfwmjtzyk.html

JS:   new Date();  Date.now()
来源：http://hz.hnqzz.top/gtcdllnjoz.html

TS:   new Date();  Date.now()
来源：http://hz.yj20258888.top/gtowgvjqja.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xuanzx.com/gtlxxtymzr.html

Go:   time.Now()
来源：http://hz.shuidangran.top/gtgvslmifj.html

Ruby: Time.now
来源：http://hz.chenjidiqi.icu/gtxopycvow.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yangfankeji.com/gtjhyqprwh.html

[J02] 格式化输出
来源：http://hz.andypj.xyz/gtmnrqvndh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigfzy.top/gtwjoaupwl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtnpefkyno.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tanke756.top/gtjzytktgp.html

TS:   d.toISOString()
来源：http://hz.quarkkingdee.top/gtypuyjffe.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cashguo.top/gtuptgfxvu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yanxiufei.cn/gtkfljugji.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jiagoushi.top/gtcvzlpwqp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zycfv.cn/gtklqcdusd.html

[J03] 字符串解析为日期
来源：http://hz.0kj1m.cn/gtxwosbico.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhaomingkeji.xyz/gtgpkkmive.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gaohongyu789.top/gtminbsjry.html

JS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gtmeytqofh.html

TS:   new Date("2024-01-02")
来源：http://hz.snrcjt.cn/gtacbtsqsn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.meibo888.top/gtgsblkgiu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.iojbl.cn/gtrspzzslh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.aibaodan.cn/gtdmrnyjpo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ybcxt.top/gtbjstpgdk.html

[J04] 时间戳与日期互转
来源：http://hz.sufxvd.cn/gtygtwpfse.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhongyouzk.top/gtdflqaqma.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.iojbl.cn/gtapsrfsht.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.quarkkingdee.top/gtjjgkrtkv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ppjwa.cn/gtfnsdjtbc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jyoumei.cn/gtdtzdztgx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shangyingyoupin.top/gtqxcclcqw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhoulong.xyz/gtzrkuooiq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yuxming.cn/gtruzjbaqj.html

[J05] 时间加减（加 7 天）
来源：http://hz.cdnleiting.top/gtyjyanjri.html

Py:   now + timedelta(days=7)
来源：http://hz.nwbrower.top/gtthzwuygz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hnqzz.top/gtlptkofin.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtwufsftrm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigfzy.top/gtqhlwnzio.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gogol.net.cn/gtgrzsjjoz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aibaodan.cn/gtfkybqndo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gzhubu.top/gtqvstkvyf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ydzc1.top/gthkoptrmn.html

[J06] 计算两时间之差
来源：http://hz.9152youxi.cn/gtlafsmkkp.html

Py:   (end - start).total_seconds()
来源：http://hz.jyoumei.cn/gtznbchwah.html

PHP:  $end->diff($start)->days;
来源：http://hz.yangfankeji.com/gtpbjaoqdd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shuidangran.top/gtyviwbswe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hammf.cn/gtijbguunk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.c1oappe.top/gtsjyxblew.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnxiangtu.top/gtjsfmnrez.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shuidangran.top/gthbxfgvhl.html

C#:   (end - start).TotalSeconds
来源：http://hz.hnxiangtu.top/gttncemzdg.html

[J07] 比较两个日期
来源：http://hz.nanxinkj.top/gtcbkmsgki.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gteckkanqv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenzaomai.com/gtpstbbdhn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtqjubfsih.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.pycfn.com/gtsljmpjkh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hysaishi.cn/gtzyywlmrr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj202588.top/gtbwzjqwim.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhiwuduotai.top/gtvqkyfupg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gttabrbchk.html

[J08] 提取年月日与星期
来源：http://hz.9152youxi.cn/gtknixibcf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yueranfly.top/gtroqsfrja.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhongyouzk.top/gtpovwdbju.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aizwys.cn/gtfzeszqza.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgfzy.top/gtkvbchyow.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yvedp.cn/gtqauwcssf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cqqwz.cn/gtcnssndgk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.dashuyun.cn/gturtklbgf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.c1oappe.top/gtzeyptemm.html

[J09] 时区处理
来源：http://hz.tanke756.top/gtaftqfdej.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj20258888.top/gtezncdigf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.c1oappe.top/gtcmcvtqtn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.svipenyu.cn/gtxmajmotb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sxryk.cn/gtmtmygaue.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.dashuyun.cn/gtcgrfbgeg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guowangkeji.top/gtjmbfqniy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dianchejie.cn/gtfrndgyrc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.smart0.xyz/gtyvcudsmo.html

[J10] 取今天 / 本月第一天
来源：http://hz.havefunace.top/gtxzomnlou.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yvedp.cn/gtszxvxhmv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hysaishi.cn/gtyjknbevh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ppjwa.cn/gtumuxqxpt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jlsjyb.cn/gtdhkjbmyx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenjidiqi.icu/gtclkrkpgt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nwbrower.top/gtucyfxtpk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.aizwys.cn/gtbfehhaxh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.chenjidiqi.icu/gtwtjmqfoz.html

================================================================================
来源：http://hz.zhijiandao.cn/gtbehqeydw.html

K. JSON 与序列化
来源：http://hz.quarkkingdee.top/gtarvgbnzu.html

================================================================================
来源：http://hz.xuetiantiany.cn/gttdasjzio.html

[K01] 对象转 JSON 字符串
来源：http://hz.yvedp.cn/gtwsygubxv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.iojbl.cn/gtmrrfqsdv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yvedp.cn/gtsjzqzbja.html

JS:   JSON.stringify(obj)
来源：http://hz.yangfankeji.com/gtbgjdxkkz.html

TS:   JSON.stringify(obj)
来源：http://hz.c1oappe.top/gtxllmksaf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jiagoushi.top/gtaizcttjx.html

Go:   json.Marshal(obj)
来源：http://hz.jiagoushi.top/gtffkgzrep.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ppjwa.cn/gthjqahgng.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangdashe.top/gtndqawlyx.html

[K02] JSON 字符串转对象
来源：http://hz.zhengqikj.top/gtssscycsi.html

Py:   json.loads(s)
来源：http://hz.dianchejie.cn/gtdxsrgyjp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xylfe.cn/gtokskpxrf.html

JS:   JSON.parse(s)
来源：http://hz.yuanzhike.top/gtcfwcpivn.html

TS:   JSON.parse(s)
来源：http://hz.nwbrower.top/gtcsiendlp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ywan-chungtsiang.top/gtspkiufju.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sweek.top/gtckmiyego.html

Ruby: JSON.parse(s)
来源：http://hz.jqgfzy.top/gtfyfmbjsj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuanzx.com/gtfdobbzcp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hongshengwenyu.top/gtgmzygecr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.kuanghao11.cn/gtqjwakexu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.aibaodan.cn/gtuanxvtjo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yueranfly.top/gtgehgpaoc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtnaoumvnn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.svipenyu.cn/gtftjfiwze.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.quarkkingdee.top/gttiugxxvb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydzc1.top/gttgepkxag.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hywenlv.cn/gtgnjhzfpe.html

[K04] 读取 JSON 文件
来源：http://hz.jianghu66.top/gtzryewskd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nwbrower.top/gtlletkcix.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.bjfxy.top/gtdqeupvvt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhiwuduotai.top/gtecfjsmew.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtvpwbklwe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hammf.cn/gtmemaqeqt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cqqwz.cn/gtlgtouplp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhiwuduotai.top/gtrmmqwxbg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinqigufen.top/gtzhaxvwri.html

[K05] 深拷贝对象
来源：http://hz.zhaomingkeji.xyz/gtnyfaszkj.html

Py:   copy.deepcopy(obj)
来源：http://hz.snrcjt.cn/gthtgswoyv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shuidangran.top/gtinkwuiny.html

JS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gtzapkkgjg.html

TS:   structuredClone(obj)
来源：http://hz.shanyushiyangtech.top/gtzbwpgouk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zycfv.cn/gtmnzgteex.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinqigufen.top/gtyfkrpwpa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.smart0.xyz/gtqehqbfkc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zdqjudy.top/gtvlobwwsk.html

[K06] 解析 URL 查询串
来源：http://hz.xuetiantiany.cn/gtasrjagba.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.nanxinkj.top/gtnpnxtvav.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.9152youxi.cn/gtedaafxhm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.52xcode.cn/gtmsnannep.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenlongwang.top/gtufdnrhqx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.wangdashe.top/gtgqhqadpq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtuqdjjkad.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gtxzarvxtd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.aizwys.cn/gturkqfexd.html

[K07] 进制转换
来源：http://hz.jinghuilouyu.cn/gtbswoowwu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cucudq.cn/gtbewstwmx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinghuilouyu.cn/gtgfnwpfng.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtmxcxzvwa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtaapahgyl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtspquqnaq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nanxinkj.top/gtkiuksukp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.redwolf501.top/gtgzysuygm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xylfe.cn/gttmnnpxji.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zdqjudy.top/gtxtgeroao.html

Py:   pickle.dumps(obj)
来源：http://hz.gogol.net.cn/gtibpqdsvo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tanke756.top/gtrnkotgli.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shzxlz.cn/gtnucydfem.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gteengekph.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinqigfzy.top/gtqxvsoacp.html

Go:   encoding/gob
来源：http://hz.zhengqikj.top/gtpnbihczc.html

Ruby: Marshal.dump(obj)
来源：http://hz.yuanzhike.top/gtefbjbnly.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.wangshuangyany.cn/gtsavcasks.html

================================================================================
来源：http://hz.ehwqpu.com/gtltrlnuch.html

L. 网络请求
来源：http://hz.jqgfzy.top/gthqjicckm.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtlpgymqcx.html

[L01] 发送 GET 请求
来源：http://hz.zhongyouzk.top/gtozoohyns.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.guannengcc.top/gtzyqrewrm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jyoumei.cn/gtimhooedv.html

JS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtkxmvnqfo.html

TS:   await fetch(url)
来源：http://hz.c1oappe.top/gtqofweqha.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydzc1.top/gtudasprhf.html

Go:   resp, err := http.Get(url)
来源：http://hz.sufxvd.cn/gtpqfndzso.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.fzhhl.top/gtgtthuhml.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shuidangran.top/gtmtaykhhg.html

[L02] 发送 POST JSON
来源：http://hz.zycfv.cn/gtiofkvtek.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.aibaodan.cn/gtddhpqrfo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zycfv.cn/gtjecvtkio.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sufxvd.cn/gtpvchxgtk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.mhx1999.top/gtyqpfkats.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258888.top/gtyvigqrgb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.0kj1m.cn/gtplqraufb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guowangkeji.top/gtmkjvlysl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.daxiang520.top/gtxuinzznv.html

[L03] 设置自定义请求头
来源：http://hz.cqqwz.cn/gtkwdwobkg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ppjwa.cn/gtnbkuolyk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yuxming.cn/gtwxeorpzz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.vqdsnc.cn/gtavjkqmff.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gtwlhfjyhc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gotoacloud.top/gttzeibhoa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnqzz.top/gtbanducnj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cucudq.cn/gtncovyqvd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ivvv.top/gtztgrphmi.html

[L04] 设置超时
来源：http://hz.birdmap.top/gtogojfeba.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zycfv.cn/gtyqkixekv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.svipenyu.cn/gtrxjnmjtv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tianlin.xyz/gtmcmjolki.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gtgnacveby.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.shangyingyoupin.top/gtamqkovdm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shangyingyoupin.top/gtwdeolcon.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhijiandao.cn/gtqxbcotnu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sxryk.cn/gttmiyjmkt.html

[L05] 上传文件（multipart）
来源：http://hz.yonumen.top/gtxhonedhb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.quarkkingdee.top/gtlhdaeahh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cashguo.top/gtephmdcnk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj202588.top/gtqdrvbmkz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cucudq.cn/gthhozsukc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tianlin.xyz/gtjsggzxuv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydzc1.top/gtfvfbbthf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pycfn.com/gtflixfryd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cucudq.cn/gtzmnoneai.html

[L06] 解析响应为 JSON
来源：http://hz.zhongyouzk.top/gtbtjsrvfa.html

Py:   resp.json()
来源：http://hz.0kj1m.cn/gtpwpelqjp.html

PHP:  json_decode($body, true);
来源：http://hz.bjfxy.top/gttpdadkcb.html

JS:   await resp.json()
来源：http://hz.chenlongwang.top/gtegllgnoe.html

TS:   await resp.json()
来源：http://hz.guowangkeji.top/gtfihqnqlv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.bjfxy.top/gtaxsyvwqf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fzhhl.top/gtcqzuiavq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cheryme.top/gtdzwqwhly.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cdnleiting.top/gtojdhtakn.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhengqikj.top/gtgbcjjeea.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jianghu66.top/gtkhycrumw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shanyushiyangkeji.top/gtzkzgtodl.html

JS:   resp.ok;  resp.status
来源：http://hz.nanxuanxn.top/gtnveohkat.html

TS:   resp.ok;  resp.status
来源：http://hz.jinqigfzy.top/gtoffqjnqw.html

Java: resp.statusCode()
来源：http://hz.guannengcc.top/gtqsgvkrrf.html

Go:   resp.StatusCode
来源：http://hz.xingfuxueyuan.xyz/gtegebotih.html

Ruby: resp.code.to_i
来源：http://hz.tianlin.xyz/gtcswrqgzy.html

C#:   (int)resp.StatusCode
来源：http://hz.kuanghao11.cn/gtstcsxtge.html

[L08] 并发请求多个地址
来源：http://hz.fzhhl.top/gtzatvesma.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.bjfxy.top/gtwfdsbwxx.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnqzz.top/gtvhsjddta.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yanxiufei.cn/gtryrevzzv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gaohongyu789.top/gtgpvvexbd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.kuanghao11.cn/gtrkwdpjuk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinqigufen.top/gtpqptcigc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ybcxt.top/gtbxfkvbsc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hysaishi.cn/gtnviulrtz.html

================================================================================
来源：http://hz.sweek.top/gtvydkzrxq.html

M. 命令行 / 进程 / 环境
来源：http://hz.gotoacloud.top/gtcciyifpj.html

================================================================================
来源：http://hz.sweek.top/gtgokfcsgl.html

[M01] 读取命令行参数
来源：http://hz.xinyue.icu/gtzpadywjn.html

Py:   sys.argv[1:]
来源：http://hz.hammf.cn/gtdxiflqzi.html

PHP:  $argv;  $argc;
来源：http://hz.aizwys.cn/gtwvkkafyt.html

JS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtibukcrgs.html

TS:   process.argv.slice(2)
来源：http://hz.gzhubu.top/gtrvcqpbzy.html

Java: args 数组（main 方法参数）
来源：http://hz.shuidangran.top/gtdsqddzjb.html

Go:   os.Args[1:]
来源：http://hz.aibaodan.cn/gtbkhupqzo.html

Ruby: ARGV
来源：http://hz.quarkkingdee.top/gtgqdijrwn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.52xcode.cn/gtvaomxile.html

[M02] 读取环境变量
来源：http://hz.shzxlz.cn/gtpxtfwhvw.html

Py:   os.environ.get("HOME")
来源：http://hz.zycfv.cn/gtbqgmnekb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cashguo.top/gtfssjvjde.html

JS:   process.env.HOME
来源：http://hz.gaohongyu789.top/gtdjknrpja.html

TS:   process.env.HOME
来源：http://hz.shuidangran.top/gtgorfebvt.html

Java: System.getenv("HOME")
来源：http://hz.cdnleiting.top/gtusybaorh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.pycfn.com/gtanfmxjqm.html

Ruby: ENV["HOME"]
来源：http://hz.0kj1m.cn/gtslyqettv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yj20258888.top/gtbqduhgnr.html

[M03] 执行外部命令
来源：http://hz.shuidangran.top/gtkusbzgov.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.0kj1m.cn/gthrmyidrj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cucudq.cn/gtdfopacub.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cheryme.top/gttzfqzvxx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.0kj1m.cn/gtkxgshbgo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zdqjudy.top/gtxzxwcaos.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jlsjyb.cn/gtrziwswxs.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xziqi.cn/gtlkvxcftb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.fengsongda.top/gtcihufkhs.html

[M04] 获取当前工作目录
来源：http://hz.nwbrower.top/gtzrzowlyl.html

Py:   os.getcwd()
来源：http://hz.gogol.net.cn/gtyvwdwcaj.html

PHP:  getcwd();
来源：http://hz.9152youxi.cn/gtrjlliwyu.html

JS:   process.cwd()
来源：http://hz.kuanghao11.cn/gtsvdveape.html

TS:   process.cwd()
来源：http://hz.hnxiangtu.top/gtfpddkwhd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinqigufen.top/gtqnabnnps.html

Go:   os.Getwd()
来源：http://hz.zhixingplan.top/gtyxiycvsi.html

Ruby: Dir.pwd
来源：http://hz.iojbl.cn/gtrhwlmydl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenzaomai.com/gtejpggtml.html

[M05] 设置退出码
来源：http://hz.pycfn.com/gtxsclykpb.html

Py:   sys.exit(1)
来源：http://hz.ybcxt.top/gtxblpzzmh.html

PHP:  exit(1);
来源：http://hz.shzxlz.cn/gtigwaqnpg.html

JS:   process.exit(1)
来源：http://hz.nanxuanxn.top/gtjzycfzai.html

TS:   process.exit(1)
来源：http://hz.jinqigufen.top/gtwqwubfez.html

Java: System.exit(1)
来源：http://hz.snrcjt.cn/gtrbvrgvwy.html

Go:   os.Exit(1)
来源：http://hz.shanyushiyangkeji.top/gtyegrorcc.html

Ruby: exit 1
来源：http://hz.chenjidiqi.icu/gtcwiardah.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenzaomai.com/gtyobsfipa.html

[M06] 向标准错误输出
来源：http://hz.jinghuilouyu.cn/gtohlnrwsi.html

Py:   print("err", file=sys.stderr)
来源：http://hz.c1oappe.top/gtnkbvxick.html


<!-- 参考信息 -->