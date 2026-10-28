代发 wailian999

Ruby: s.scan(/error/i)
来源：http://hz.redwolf501.top/gtbivnczas.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.daria6918.cn/gtzklbuoaj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sysykeji.top/gtcrvpmtmp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ywan-chungtsiang.top/gtnahyclpz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guannengcc.top/gtxmwxdybi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fengsongda.top/gtrznjnxte.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tanke756.top/gtzounquvb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuetiantiany.cn/gthzjrxolu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuetiantiany.cn/gtoadngycp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinghuilouyu.cn/gtiqrxbfuo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daxiang520.top/gttkhqhvqf.html

================================================================================
来源：http://hz.nanxuanxn.top/gtznoxyqjj.html

J. 日期与时间
来源：http://hz.chenlongwang.top/gtfzjmhjlf.html

================================================================================
来源：http://hz.birdmap.top/gtoecjcjro.html

[J01] 获取当前时间
来源：http://hz.sufxvd.cn/gtrmpbzzph.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.wangdashe.top/gtxppcwedn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.snrcjt.cn/gtpprvulmj.html

JS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gtemmgjazm.html

TS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gtpdquazsl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gaohongyu789.top/gtqkkmodzv.html

Go:   time.Now()
来源：http://hz.fzhhl.top/gtjmfwihpa.html

Ruby: Time.now
来源：http://hz.yuxming.cn/gtfzehpxyz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.smart0.xyz/gtjjavtmyl.html

[J02] 格式化输出
来源：http://hz.shanyushiyangkeji.top/gtprzhfdet.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yvedp.cn/gtyxafotyc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sysykeji.top/gtuizxirao.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.52xcode.cn/gtxmonzsko.html

TS:   d.toISOString()
来源：http://hz.pengpengdd.cyou/gtbhofgyki.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tianlin.xyz/gtttiidcuo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hysaishi.cn/gtyymunmih.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yonumen.top/gtxwqzowet.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.316326.xyz/gtbghicwaf.html

[J03] 字符串解析为日期
来源：http://hz.sysykeji.top/gtrrohgcqs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.316326.xyz/gtexjttidh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.c1oappe.top/gtyiydoubr.html

JS:   new Date("2024-01-02")
来源：http://hz.snrcjt.cn/gtvwvcfaot.html

TS:   new Date("2024-01-02")
来源：http://hz.guannengcc.top/gtuwkfrild.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtxbrrsgmk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cheryme.top/gthrqzuhlu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtroqqyyqx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.9152youxi.cn/gtyvrgdrqd.html

[J04] 时间戳与日期互转
来源：http://hz.gzhubu.top/gtnoeijpcc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigufen.top/gttefttiqf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.snrcjt.cn/gtkgnwhttr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.daxiang520.top/gtuwckqjvv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.aibaodan.cn/gtmdejdkxx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sysykeji.top/gtwqhedqni.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jlsjyb.cn/gtvbiewowa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xziqi.cn/gtwnqnqdbx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jianghu66.top/gteqiipoiz.html

[J05] 时间加减（加 7 天）
来源：http://hz.hnxiangtu.top/gtobwnfghb.html

Py:   now + timedelta(days=7)
来源：http://hz.haohaochexian.top/gtgjpfltqt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hysaishi.cn/gtsylvunlw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gtpmwfhctj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtwmthfoim.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aizwys.cn/gtqbhtmgrs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shanyushiyangkeji.top/gtcddmzjrw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ehwqpu.com/gttwxjgvpw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fengsongda.top/gtoaqpigdf.html

[J06] 计算两时间之差
来源：http://hz.smart0.xyz/gtrjeabtwi.html

Py:   (end - start).total_seconds()
来源：http://hz.zhongyouzk.top/gtxhyxyatg.html

PHP:  $end->diff($start)->days;
来源：http://hz.cheryme.top/gtpnsjjgej.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenzaomai.com/gtqmkmagco.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigufen.top/gtusdgitto.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jianghu66.top/gtpzispwdz.html

Go:   end.Sub(start).Hours()
来源：http://hz.shangyingyoupin.top/gtvfzrveld.html

Ruby: end - start                 # 返回秒数
来源：http://hz.dashuyun.cn/gteufmwozn.html

C#:   (end - start).TotalSeconds
来源：http://hz.guowangkeji.top/gtxpssmhnx.html

[J07] 比较两个日期
来源：http://hz.chenlongwang.top/gtnxbkaior.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhijiandao.cn/gtdijvhxvg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.gaohongyu789.top/gtfrzroell.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.aibaodan.cn/gtotmmbpnh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.andypj.xyz/gtqrmqlfic.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenlongwang.top/gtkpcumtls.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hysaishi.cn/gtiaorkrjo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtymdrwruk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtqrplvbyh.html

[J08] 提取年月日与星期
来源：http://hz.yangfankeji.com/gtcplakqfm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cqqwz.cn/gtelwinxwg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xziqi.cn/gtmszvlqry.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.snrcjt.cn/gttktbflid.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangkeji.top/gtglengicu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ydjk.org.cn/gtrwmiltqa.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xinyue.icu/gtgmrnrspq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenlongwang.top/gtptqeabbs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinyuanbaomall.cn/gtwmgxtagk.html

[J09] 时区处理
来源：http://hz.jinghuilouyu.cn/gtshhwpcwg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.wangshuangyany.cn/gtptqcuggb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cheryme.top/gttiagsyfh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gteucgdtrm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zdqjudy.top/gtvraeofgk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.0kj1m.cn/gtpnwxtmqz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.daxiang520.top/gtjoydleqk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinghuilouyu.cn/gtwtaojuxk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinghuilouyu.cn/gtaosjyrtq.html

[J10] 取今天 / 本月第一天
来源：http://hz.gogol.net.cn/gtqnefdpaq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zycfv.cn/gtiageyvwz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ppjwa.cn/gtxoxtagsd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ydjk.org.cn/gtngurqpfa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj20258.top/gttiwkwwwe.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shangyingyoupin.top/gtnkuhhgsn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinghuilouyu.cn/gtvvcoyfyd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zdqjudy.top/gtsgwtrlvt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xylfe.cn/gtaaqlnhvb.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtwbdtblii.html

K. JSON 与序列化
来源：http://hz.yongpay.top/gtybxyoiem.html

================================================================================
来源：http://hz.316326.xyz/gtckbcgkbi.html

[K01] 对象转 JSON 字符串
来源：http://hz.nanxinkj.top/gthzsiyarw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ppjwa.cn/gtyfjlrsjc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jiagoushi.top/gtdzvfrtfu.html

JS:   JSON.stringify(obj)
来源：http://hz.hammf.cn/gtylenieos.html

TS:   JSON.stringify(obj)
来源：http://hz.yj20258888.top/gtkswnnvdr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.mhx1999.top/gturjfknsw.html

Go:   json.Marshal(obj)
来源：http://hz.daria6918.cn/gtxvjjamjw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zdqjudy.top/gtocipjjgu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ppjwa.cn/gtwlnmcgds.html

[K02] JSON 字符串转对象
来源：http://hz.gogol.net.cn/gtdkziypjg.html

Py:   json.loads(s)
来源：http://hz.pengpengdd.cyou/gtvlqqgqnd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gotoacloud.top/gtgkyilfdj.html

JS:   JSON.parse(s)
来源：http://hz.yuxming.cn/gthklipaca.html

TS:   JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtzjflhrjz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cdnleiting.top/gtfiabdnfm.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.wangshuangyany.cn/gtrrfpswko.html

Ruby: JSON.parse(s)
来源：http://hz.guannengcc.top/gtbyeiadaq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ehwqpu.com/gtaaiukxap.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jlsjyb.cn/gtfnitgilt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cucudq.cn/gtzosqthva.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtseckfkpy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gttghhorkp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinghuilouyu.cn/gtxoanahcz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nanxinkj.top/gtarcpffva.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ivvv.top/gtvybpsofi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jlsjyb.cn/gtcrbgsbmq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tian-w.cn/gtvtdkvpyj.html

[K04] 读取 JSON 文件
来源：http://hz.chenjidiqi.icu/gtndqsoewh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cashguo.top/gtqfjtcuvf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinqigfzy.top/gtwvncbmoe.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.birdmap.top/gtjocpkrhb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fengsongda.top/gtztqluvuy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhongyouzk.top/gtlioznnpd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhixingplan.top/gtovaovfhl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zycfv.cn/gtunmmuami.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shanyushiyangtech.top/gtazdnjkej.html

[K05] 深拷贝对象
来源：http://hz.52xcode.cn/gtswsdfizs.html

Py:   copy.deepcopy(obj)
来源：http://hz.iojbl.cn/gtrozrhvjc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jlsjyb.cn/gtmeetygva.html

JS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gtchsiptfc.html

TS:   structuredClone(obj)
来源：http://hz.zycfv.cn/gtttgnxopv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cqqwz.cn/gttkgpjpfx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenjidiqi.icu/gtpepzweri.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yueranfly.top/gtyejmnmnc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pycfn.com/gtllxrabku.html

[K06] 解析 URL 查询串
来源：http://hz.jyoumei.cn/gtvfuepyxq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.guowangkeji.top/gtahgfpjyq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinghuilouyu.cn/gthbuibdpt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.0kj1m.cn/gtcjmaflne.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj202588.top/gtmwuokcfo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhijiandao.cn/gttmhpqyvb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.bjfxy.top/gtqvvppgsz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yonumen.top/gtoyrwzogo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.svipenyu.cn/gtsimkdoyg.html

[K07] 进制转换
来源：http://hz.chenzaomai.com/gtzwpsjbhz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenlongwang.top/gtobztaetf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydjk.org.cn/gtyqqfncic.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtwhxkblxu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtkaqdgojh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gtdfmobbgr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.feifeiyinyue.top/gtsaqkwfdo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yangfankeji.com/gtpodwyoxw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhengqikj.top/gttrtomfgz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.smart0.xyz/gtjsreihjx.html

Py:   pickle.dumps(obj)
来源：http://hz.ppjwa.cn/gttebmlwax.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.316326.xyz/gtvghzrxwx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhaomingkeji.xyz/gtaudeyuhg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.meibo888.top/gtyeplkzcn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yonumen.top/gtwzjqlvbn.html

Go:   encoding/gob
来源：http://hz.zycfv.cn/gtpghrwldx.html

Ruby: Marshal.dump(obj)
来源：http://hz.dashuyun.cn/gtudulhyom.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yuxming.cn/gtuoptrsdl.html

================================================================================
来源：http://hz.wangdashe.top/gtoyrqeaoh.html

L. 网络请求
来源：http://hz.ywan-chungtsiang.top/gtebslgjwo.html

================================================================================
来源：http://hz.cashguo.top/gtxsoddasw.html

[L01] 发送 GET 请求
来源：http://hz.daria6918.cn/gtdmwxette.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daxiang520.top/gteayxkpon.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yueranfly.top/gttnornoeq.html

JS:   await fetch(url)
来源：http://hz.shanyushiyangkeji.top/gtfvqbclmc.html

TS:   await fetch(url)
来源：http://hz.sweek.top/gtrcqydezr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.dashuyun.cn/gthgqpbasv.html

Go:   resp, err := http.Get(url)
来源：http://hz.jyoumei.cn/gtokfatpbt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ehwqpu.com/gtixzonfzw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gotoacloud.top/gtlmpnmubg.html

[L02] 发送 POST JSON
来源：http://hz.xziqi.cn/gtvezfjdrq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hysaishi.cn/gtxessjsoi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yj20258.top/gtbdaajttb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guowangkeji.top/gtzssizfcc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zycfv.cn/gtexcpnnfx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gzhubu.top/gtdnwmacln.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cucudq.cn/gthkvglhad.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.havefunace.top/gtplzmehum.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nanxuanxn.top/gtcjjsuvxu.html

[L03] 设置自定义请求头
来源：http://hz.chenlongwang.top/gtgrgfbamq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.daria6918.cn/gtkiquyotq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.daxiang520.top/gtgssbpzpn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.0kj1m.cn/gtuqvvklay.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.birdmap.top/gtqbyztodz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.birdmap.top/gtwskukmrv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tian-w.cn/gtegvnyvgt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.snrcjt.cn/gtmybmvoxz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuxming.cn/gtzgngaddi.html

[L04] 设置超时
来源：http://hz.9152youxi.cn/gtggxgetnt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgufenzy.top/gtxfpkpfdh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sufxvd.cn/gtjpyhkvsd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xziqi.cn/gtnmokahis.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gtykddvwqh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhijiandao.cn/gtayzspboo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.guannengcc.top/gtefnmilks.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yuanzhike.top/gtragehshy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenlongwang.top/gthvwphbxc.html

[L05] 上传文件（multipart）
来源：http://hz.sweek.top/gtisinzwfe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.chenzaomai.com/gtwshsigfm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zdqjudy.top/gtvdzrtdsb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cashguo.top/gtacndmkht.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtadtndten.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.c1oappe.top/gtgcvvrvcu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tian-w.cn/gtfafrcgfy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhaomingkeji.xyz/gtpztbgqkn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guowangkeji.top/gtrqqxodol.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigfzy.top/gtsviuzdgh.html

Py:   resp.json()
来源：http://hz.hfpthk.cn/gtrasbxbsa.html

PHP:  json_decode($body, true);
来源：http://hz.yj20258.top/gtfmyigwuv.html

JS:   await resp.json()
来源：http://hz.yueranfly.top/gtpdkbtuim.html

TS:   await resp.json()
来源：http://hz.nwbrower.top/gtoqnxyzpp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gzhubu.top/gtzrjjbmfx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sysykeji.top/gtjispxzta.html

Ruby: JSON.parse(resp.body)
来源：http://hz.wangdashe.top/gtekmoilcs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.bjfxy.top/gtxwfwquek.html

[L07] 处理 HTTP 状态码
来源：http://hz.hammf.cn/gtjxerwiuy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xuetiantiany.cn/gtetmocwlz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jyoumei.cn/gtvruagpix.html

JS:   resp.ok;  resp.status
来源：http://hz.cqqwz.cn/gtkeljbwbn.html

TS:   resp.ok;  resp.status
来源：http://hz.tanke756.top/gtkhdssacw.html

Java: resp.statusCode()
来源：http://hz.ehwqpu.com/gtbfhsfzqq.html

Go:   resp.StatusCode
来源：http://hz.jinyuanbaomall.cn/gtsivxyvqp.html

Ruby: resp.code.to_i
来源：http://hz.52xcode.cn/gthwlvkgws.html

C#:   (int)resp.StatusCode
来源：http://hz.chenlongwang.top/gtrdxfninf.html

[L08] 并发请求多个地址
来源：http://hz.9152youxi.cn/gtrtassbac.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.9152youxi.cn/gthcmhpqyn.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinqigfzy.top/gtzlnudvrc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtmtxkpkor.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtvvylhekx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xingfuxueyuan.xyz/gtqmhpiopd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.mhx1999.top/gtztnaggzm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sufxvd.cn/gtizfyqrip.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj20258.top/gtqolwpfza.html

================================================================================
来源：http://hz.jyoumei.cn/gtnfyjjuts.html

M. 命令行 / 进程 / 环境
来源：http://hz.fzhhl.top/gtylunautq.html

================================================================================
来源：http://hz.cqqwz.cn/gtuwhsqchv.html

[M01] 读取命令行参数
来源：http://hz.feifeiyinyue.top/gtahgmmaao.html

Py:   sys.argv[1:]
来源：http://hz.gogol.net.cn/gtfiyfbckl.html

PHP:  $argv;  $argc;
来源：http://hz.zycfv.cn/gtjojxcqap.html

JS:   process.argv.slice(2)
来源：http://hz.316326.xyz/gtdlbmbbxm.html

TS:   process.argv.slice(2)
来源：http://hz.iojbl.cn/gtbcdbewkc.html

Java: args 数组（main 方法参数）
来源：http://hz.yonumen.top/gtglmguhgb.html

Go:   os.Args[1:]
来源：http://hz.snrcjt.cn/gtvuogfzxn.html

Ruby: ARGV
来源：http://hz.birdmap.top/gtdoxjjkxo.html

C#:   args 数组（Main 方法参数）
来源：http://hz.meibo888.top/gtnmrxmexo.html

[M02] 读取环境变量
来源：http://hz.cheryme.top/gtzkihkkga.html

Py:   os.environ.get("HOME")
来源：http://hz.jianghu66.top/gttlqzouhe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinqigfzy.top/gtdmuznppv.html

JS:   process.env.HOME
来源：http://hz.52xcode.cn/gtjpehxlyu.html

TS:   process.env.HOME
来源：http://hz.sufxvd.cn/gtlgufeglu.html

Java: System.getenv("HOME")
来源：http://hz.52xcode.cn/gtgxadzfjj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yongpay.top/gtpojatjky.html

Ruby: ENV["HOME"]
来源：http://hz.jinyuanbaomall.cn/gtowykxtkp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinyuanbaomall.cn/gtmikbawqu.html

[M03] 执行外部命令
来源：http://hz.hywenlv.cn/gtoeefebbe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuxming.cn/gtqlhvlziq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guowangkeji.top/gthgtdcqjg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnqzz.top/gtaezwszxv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtssjlnmps.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhoulong.xyz/gtudgjkdst.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ehwqpu.com/gtpebfmtui.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jqgfzy.top/gtnpmdaeap.html

C#:   Process.Start("ls", "-l");
来源：http://hz.kuanghao11.cn/gtxcgagjyz.html

[M04] 获取当前工作目录
来源：http://hz.haohaochexian.top/gtjqevqhlb.html

Py:   os.getcwd()
来源：http://hz.ywan-chungtsiang.top/gtjftnikgk.html

PHP:  getcwd();
来源：http://hz.vqdsnc.cn/gtmkhrmxpt.html

JS:   process.cwd()
来源：http://hz.aizwys.cn/gtwmhpnvqb.html

TS:   process.cwd()
来源：http://hz.yuxming.cn/gthktymlgv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yanxiufei.cn/gtmatfizgr.html

Go:   os.Getwd()
来源：http://hz.jianghu66.top/gtqeulgevd.html

Ruby: Dir.pwd
来源：http://hz.mhx1999.top/gtkxbjvrvm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenjidiqi.icu/gtfklighlh.html

[M05] 设置退出码
来源：http://hz.iojbl.cn/gtsacmmlzk.html

Py:   sys.exit(1)
来源：http://hz.jinqigfzy.top/gtnmmjcunk.html

PHP:  exit(1);
来源：http://hz.zhixingplan.top/gtncsatgob.html

JS:   process.exit(1)
来源：http://hz.ybcxt.top/gtqpccouwl.html

TS:   process.exit(1)
来源：http://hz.gaohongyu789.top/gtbsijiidy.html

Java: System.exit(1)
来源：http://hz.andypj.xyz/gtqaoqfocy.html

Go:   os.Exit(1)
来源：http://hz.yongpay.top/gtptbhmnls.html


<!-- 参考信息 -->