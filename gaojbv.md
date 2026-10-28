代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gaohongyu789.top/gtpbvzctoc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yvedp.cn/gtovvjtuor.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sysykeji.top/gtaydirwkv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.dashuyun.cn/gtqajgpwxm.html

[J03] 字符串解析为日期
来源：http://hz.fzhhl.top/gteibuyzpn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hysaishi.cn/gtaljxsmew.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sysykeji.top/gtnktricfu.html

JS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtbyqjuhgo.html

TS:   new Date("2024-01-02")
来源：http://hz.birdmap.top/gtsfapmsgd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtieqfeazg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinqigfzy.top/gtcsklfgdm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenzaomai.com/gtfyhlohzw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.mhx1999.top/gtgnusfkjw.html

[J04] 时间戳与日期互转
来源：http://hz.xuetiantiany.cn/gtymluwrhx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jiagoushi.top/gtdeiuffbt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.vqdsnc.cn/gtmlfsnrjz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sxryk.cn/gteyetgyia.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenzaomai.com/gtjofisihz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangdashe.top/gtkqpowupc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj20258888.top/gtdsghjrri.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenlongwang.top/gtlzqrqnzc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tanke756.top/gtwrowfajm.html

[J05] 时间加减（加 7 天）
来源：http://hz.jiagoushi.top/gtkbofncjv.html

Py:   now + timedelta(days=7)
来源：http://hz.yonumen.top/gtvxtzmckh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sweek.top/gtvvhnqalt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sxryk.cn/gtmkkoefvd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtbrrjwinc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.mhx1999.top/gttfrpacxd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgfzy.top/gtqktbnpej.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shangyingyoupin.top/gtuqulgwac.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.pycfn.com/gthyhwcbqg.html

[J06] 计算两时间之差
来源：http://hz.tianlin.xyz/gtnmczddwa.html

Py:   (end - start).total_seconds()
来源：http://hz.pycfn.com/gtncpjxszu.html

PHP:  $end->diff($start)->days;
来源：http://hz.cheryme.top/gtofmfywtx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xinyue.icu/gtwwpozwxe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.aizwys.cn/gtiliwnehr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hfpthk.cn/gtajutuelo.html

Go:   end.Sub(start).Hours()
来源：http://hz.sweek.top/gtdygxzsul.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tianlin.xyz/gtfufzovdb.html

C#:   (end - start).TotalSeconds
来源：http://hz.gogol.net.cn/gtkdfpxeci.html

[J07] 比较两个日期
来源：http://hz.gaohongyu789.top/gtexkakdmr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtnfucyvhu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.pycfn.com/gtuncunqrf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gtvdukbzcu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtzqsfickf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangdashe.top/gtsahlipmm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnqzz.top/gtmudxlbvo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258888.top/gtrwxhwamt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtgrhjvnxp.html

[J08] 提取年月日与星期
来源：http://hz.dianchejie.cn/gtmrdreqif.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenzaomai.com/gtyragktkv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cdnleiting.top/gtpizvtseo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.iojbl.cn/gtzituibgr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xingfuxueyuan.xyz/gtcxgkgbyc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.c1oappe.top/gtvmbsrtsd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xuanzx.com/gtuwfaejln.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hfpthk.cn/gtiixjoqry.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xylfe.cn/gtrvgnwbkb.html

[J09] 时区处理
来源：http://hz.yvedp.cn/gtaekzqoya.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.9152youxi.cn/gthdptomhq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cdnleiting.top/gtyzggemai.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daxiang520.top/gtqhmaywho.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhongyouzk.top/gtnumxbbzf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ydjk.org.cn/gthvnghyjm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cheryme.top/gtxcbvhilq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.iojbl.cn/gtwbptiudf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.kuanghao11.cn/gthusoqrtq.html

[J10] 取今天 / 本月第一天
来源：http://hz.redwolf501.top/gtpgzcfrqa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cashguo.top/gtvexlzphs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhaomingkeji.xyz/gtqjthozbi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jlsjyb.cn/gttioysmez.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.aizwys.cn/gtgsscqjav.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.kuanghao11.cn/gtgtitwbyt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ydzc1.top/gtlwhuewtp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zycfv.cn/gtcjoyvetf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dashuyun.cn/gtpxapjwdk.html

================================================================================
来源：http://hz.jqgfzy.top/gtxnjzsezr.html

K. JSON 与序列化
来源：http://hz.wangdashe.top/gtnylmbike.html

================================================================================
来源：http://hz.jlsjyb.cn/gtojedquml.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhaomingkeji.xyz/gtgeroytzs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj20258.top/gtkgfhmaeb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtryfvftqv.html

JS:   JSON.stringify(obj)
来源：http://hz.yangfankeji.com/gtkbcgtmog.html

TS:   JSON.stringify(obj)
来源：http://hz.yj20258.top/gttqzemxld.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shanyushiyangkeji.top/gtubuqmban.html

Go:   json.Marshal(obj)
来源：http://hz.hfpthk.cn/gtrnuhtpvl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tian-w.cn/gtkpvfsbul.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shanyushiyangkeji.top/gtwtkyvcre.html

[K02] JSON 字符串转对象
来源：http://hz.jinyuanbaomall.cn/gtymttigno.html

Py:   json.loads(s)
来源：http://hz.cheryme.top/gtitgatjvq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hongshengwenyu.top/gtiximuqhp.html

JS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtyhhkbsak.html

TS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtzrmjnwdo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.feifeiyinyue.top/gthafzilbm.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtxvjkaicw.html

Ruby: JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtbgmvmyad.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.quarkkingdee.top/gtozzjhscd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.fengsongda.top/gtldxpprfz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gogol.net.cn/gtnocmwhux.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtdcqlhdai.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guannengcc.top/gtxzcriovz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhaomingkeji.xyz/gtxabtteaq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhijiandao.cn/gtwdyvqtgg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xuanzx.com/gtvnkqwlkn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yuanzhike.top/gtaczxxcxx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.0kj1m.cn/gtmbiiqsif.html

[K04] 读取 JSON 文件
来源：http://hz.feifeiyinyue.top/gthqesywbh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xylfe.cn/gtskjzjegz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jqgfzy.top/gtfbcrehqu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ybcxt.top/gtzigheyyl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yonumen.top/gtwdpipsez.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hfpthk.cn/gtwerwfagb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtvyyenxkr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cheryme.top/gtlmhyfpko.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.iojbl.cn/gtgrvywcii.html

[K05] 深拷贝对象
来源：http://hz.nwbrower.top/gtnatqdxfk.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydjk.org.cn/gtzmdykgka.html

PHP:  unserialize(serialize($obj));
来源：http://hz.daxiang520.top/gtlspaeqny.html

JS:   structuredClone(obj)
来源：http://hz.quarkkingdee.top/gtbuepvzcx.html

TS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gthpmgreiv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hfpthk.cn/gtxwmldahd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yuxming.cn/gtcsmxyjqg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.iojbl.cn/gtjkisszah.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinghuilouyu.cn/gtmptgjoum.html

[K06] 解析 URL 查询串
来源：http://hz.ywan-chungtsiang.top/gtpdzntsyt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ywan-chungtsiang.top/gtvimezovz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xinyue.icu/gtborumbek.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fengsongda.top/gtuubytbyp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.316326.xyz/gtrrjzwgme.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.snrcjt.cn/gtvusrdhij.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.meibo888.top/gtrpsihmpe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shuidangran.top/gtwgttvoke.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxinkj.top/gtaklnlloj.html

[K07] 进制转换
来源：http://hz.daxiang520.top/gtjlzgorrz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.fzhhl.top/gthhhqbmsc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ivvv.top/gtxwboaawy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtdxorwgex.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtkpqzvwyf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtguculrgj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sufxvd.cn/gtxxuzopsy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.kuanghao11.cn/gtdgflylia.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nanxuanxn.top/gtxwamsmdl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydzc1.top/gtkjfnmqvg.html

Py:   pickle.dumps(obj)
来源：http://hz.jiagoushi.top/gtubsbyfhr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinqigufen.top/gtnsqdoywa.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jlsjyb.cn/gtjiqskvvk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gtaaasmckv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.52xcode.cn/gtbcdghiac.html

Go:   encoding/gob
来源：http://hz.jyoumei.cn/gtznlwiqzy.html

Ruby: Marshal.dump(obj)
来源：http://hz.hammf.cn/gtrxserasg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jlsjyb.cn/gtnfpadyen.html

================================================================================
来源：http://hz.jinqigufen.top/gtswvprpsk.html

L. 网络请求
来源：http://hz.tian-w.cn/gtbvmazjgd.html

================================================================================
来源：http://hz.svipenyu.cn/gtdefmscia.html

[L01] 发送 GET 请求
来源：http://hz.9152youxi.cn/gthsahfsou.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gogol.net.cn/gtdkuflnkc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yanxiufei.cn/gtvlfwifyo.html

JS:   await fetch(url)
来源：http://hz.meibo888.top/gtzoatomok.html

TS:   await fetch(url)
来源：http://hz.nwbrower.top/gtkcbindng.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.fzhhl.top/gtccgwlqtt.html

Go:   resp, err := http.Get(url)
来源：http://hz.fengsongda.top/gtnyvmnwrn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hywenlv.cn/gtdyrwxjyq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.havefunace.top/gtzicqqgmi.html

[L02] 发送 POST JSON
来源：http://hz.shuidangran.top/gtratzzqvf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shanyushiyangkeji.top/gtwfhyqrvh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.chenzaomai.com/gtdlityghe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gtnncdmwmy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtbyqwjxln.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.9152youxi.cn/gtnolsvwzp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gotoacloud.top/gtgljaatbv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sweek.top/gtyysbcvji.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shzxlz.cn/gtydcofqaj.html

[L03] 设置自定义请求头
来源：http://hz.hywenlv.cn/gtfbzvaejy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.aizwys.cn/gttxfhudii.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hysaishi.cn/gtvjlzmpbr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aibaodan.cn/gtxqdcjvqc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgfzy.top/gtsufjxeld.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj20258.top/gtrmfczkhf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hysaishi.cn/gtmowkhwom.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangtech.top/gtbtklxzof.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.0kj1m.cn/gtgajynvww.html

[L04] 设置超时
来源：http://hz.9152youxi.cn/gtbhihllxi.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yvedp.cn/gtrqlnayhe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.guannengcc.top/gtjqritdmb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangdashe.top/gtvtuphdpe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gteaogeiil.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhixingplan.top/gtvoytawvp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cashguo.top/gtgkdflszj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cashguo.top/gtuzwgsama.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yueranfly.top/gtxztdtowj.html

[L05] 上传文件（multipart）
来源：http://hz.zycfv.cn/gtiodcfzhu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xingfuxueyuan.xyz/gtoedkzais.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ywan-chungtsiang.top/gtzumodyif.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hywenlv.cn/gtajajvhcg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgfzy.top/gtizyxbmwb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.quarkkingdee.top/gtmgslpuwb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nwbrower.top/gtpjnsdxte.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.bjfxy.top/gtujyqhuwv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.mhx1999.top/gtnlxibbss.html

[L06] 解析响应为 JSON
来源：http://hz.yj20258888.top/gtmraochaj.html

Py:   resp.json()
来源：http://hz.jyoumei.cn/gtrdymyuan.html

PHP:  json_decode($body, true);
来源：http://hz.9152youxi.cn/gtgldtqrgb.html

JS:   await resp.json()
来源：http://hz.cashguo.top/gtphbjjfcq.html

TS:   await resp.json()
来源：http://hz.jqgufenzy.top/gtutkldgay.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.pycfn.com/gttothnrpq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xuanzx.com/gtjlackcut.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgfzy.top/gtixnltsjz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.birdmap.top/gtmwfbqxzo.html

[L07] 处理 HTTP 状态码
来源：http://hz.cashguo.top/gtzsebpzxg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nanxuanxn.top/gtaevhvpbt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shzxlz.cn/gtuwvlmjja.html

JS:   resp.ok;  resp.status
来源：http://hz.ehwqpu.com/gtoqtvrvnt.html

TS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gtocujcjtq.html

Java: resp.statusCode()
来源：http://hz.shangyingyoupin.top/gtlfnzmuga.html

Go:   resp.StatusCode
来源：http://hz.ywan-chungtsiang.top/gtqrxkopgt.html

Ruby: resp.code.to_i
来源：http://hz.zhixingplan.top/gtrdxzsglq.html

C#:   (int)resp.StatusCode
来源：http://hz.tian-w.cn/gteqagdvze.html

[L08] 并发请求多个地址
来源：http://hz.ivvv.top/gtiuoafhkf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xziqi.cn/gthvhthztt.html

PHP:  curl_multi_init() 系列
来源：http://hz.nwbrower.top/gtuoseypvn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tanke756.top/gtvcvdfvcq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtonbbnsyg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xuetiantiany.cn/gtojtofgsu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yuanzhike.top/gtzlczaiiq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.pycfn.com/gtqlcasgvj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hnxiangtu.top/gtgtxxllqk.html

================================================================================
来源：http://hz.nwbrower.top/gtiowlzjlz.html

M. 命令行 / 进程 / 环境
来源：http://hz.xingfuxueyuan.xyz/gtxaubnajc.html

================================================================================
来源：http://hz.jlsjyb.cn/gtpcsgfmlo.html

[M01] 读取命令行参数
来源：http://hz.yuanzhike.top/gtvwpwmpkp.html

Py:   sys.argv[1:]
来源：http://hz.yuanzhike.top/gtbgkslomo.html

PHP:  $argv;  $argc;
来源：http://hz.pengpengdd.cyou/gtqrnaagkr.html

JS:   process.argv.slice(2)
来源：http://hz.pengpengdd.cyou/gtyvgpwlgr.html

TS:   process.argv.slice(2)
来源：http://hz.sufxvd.cn/gtxlcpxhzj.html

Java: args 数组（main 方法参数）
来源：http://hz.xuanzx.com/gtemjslmph.html

Go:   os.Args[1:]
来源：http://hz.ivvv.top/gtqgeuouxr.html

Ruby: ARGV
来源：http://hz.cheryme.top/gtqrnhfvxm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydzc1.top/gtjpwjvcpb.html

[M02] 读取环境变量
来源：http://hz.hywenlv.cn/gtgfkpcxgz.html

Py:   os.environ.get("HOME")
来源：http://hz.snrcjt.cn/gtdlwuvcmw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zdqjudy.top/gthjiubtty.html

JS:   process.env.HOME
来源：http://hz.zhixingplan.top/gtlxplejop.html

TS:   process.env.HOME
来源：http://hz.c1oappe.top/gtbizykhty.html

Java: System.getenv("HOME")
来源：http://hz.jinqigfzy.top/gtybqncnsu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xylfe.cn/gtobvfogfx.html

Ruby: ENV["HOME"]
来源：http://hz.zdqjudy.top/gtkjtjdpvr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.tian-w.cn/gtbiufaguy.html

[M03] 执行外部命令
来源：http://hz.haohaochexian.top/gtnvnlzysn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinqigufen.top/gtrxuqyhky.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gotoacloud.top/gtgqrnfesx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenjidiqi.icu/gtdqrxyfxe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenlongwang.top/gtckumjbuc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gaohongyu789.top/gtndgocplz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.snrcjt.cn/gtuptbbsen.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yongpay.top/gttocufoae.html

C#:   Process.Start("ls", "-l");
来源：http://hz.guowangkeji.top/gtzawiaytt.html

[M04] 获取当前工作目录
来源：http://hz.shanyushiyangtech.top/gtuhjdrawu.html

Py:   os.getcwd()
来源：http://hz.shangyingyoupin.top/gtyuvgnayp.html

PHP:  getcwd();
来源：http://hz.9152youxi.cn/gtwtcrycky.html

JS:   process.cwd()
来源：http://hz.yvedp.cn/gtdlziodcc.html

TS:   process.cwd()
来源：http://hz.xingfuxueyuan.xyz/gtwldncxjq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.smart0.xyz/gtslnfdowe.html

Go:   os.Getwd()
来源：http://hz.mhx1999.top/gthhpramzx.html

Ruby: Dir.pwd
来源：http://hz.jianghu66.top/gtvxidpxvo.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sufxvd.cn/gtozjdnnzf.html

[M05] 设置退出码
来源：http://hz.xuetiantiany.cn/gtpkjuhkzg.html

Py:   sys.exit(1)
来源：http://hz.daria6918.cn/gtnvkxbdeu.html

PHP:  exit(1);
来源：http://hz.guowangkeji.top/gtqvrtjgew.html

JS:   process.exit(1)
来源：http://hz.ybcxt.top/gtegkpqzyn.html

TS:   process.exit(1)
来源：http://hz.zhijiandao.cn/gtysugcrng.html

Java: System.exit(1)
来源：http://hz.yueranfly.top/gtoraxmtlx.html

Go:   os.Exit(1)
来源：http://hz.iojbl.cn/gtgwksqorc.html

Ruby: exit 1
来源：http://hz.ydjk.org.cn/gtndimwqjy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.redwolf501.top/gtfbxmnjpr.html

[M06] 向标准错误输出
来源：http://hz.9152youxi.cn/gtypczdooj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cashguo.top/gtrwmtezsr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ydzc1.top/gtquebgnfh.html

JS:   console.error("err")
来源：http://hz.xziqi.cn/gtxdnudxvi.html

TS:   console.error("err")
来源：http://hz.tanke756.top/gtgylcijtr.html

Java: System.err.println("err")
来源：http://hz.svipenyu.cn/gtrptxytuc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.quarkkingdee.top/gtznyrokhh.html

Ruby: warn "err"
来源：http://hz.shuidangran.top/gtpbwpztqt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sweek.top/gtceeeeqsz.html

[M07] 判断是否为主入口
来源：http://hz.52xcode.cn/gtbnfarrsq.html

Py:   if __name__ == "__main__":
来源：http://hz.0kj1m.cn/gtmyqbtlct.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.quarkkingdee.top/gtsodcawhr.html

JS:   require.main === module
来源：http://hz.jinqigfzy.top/gtwvqsfzde.html

TS:   require.main === module
来源：http://hz.jinghuilouyu.cn/gtjwsimzoc.html

Java: public static void main(String[] args)
来源：http://hz.yongpay.top/gtuyineplm.html

Go:   func main()
来源：http://hz.yueranfly.top/gtvgcwzmqj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cqqwz.cn/gtaiesvgns.html

C#:   static void Main(string[] args)
来源：http://hz.ydzc1.top/gtirdydlsn.html

[M08] 获取系统与运行时信息
来源：http://hz.daxiang520.top/gtweklklsg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jianghu66.top/gtsvzpevwx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.vqdsnc.cn/gtysffnrzb.html

JS:   process.platform;  process.version
来源：http://hz.kuanghao11.cn/gtduitjtoc.html

TS:   process.platform;  process.version
来源：http://hz.shangyingyoupin.top/gtzciqsffr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yuxming.cn/gtqejohtvi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yj20258.top/gtqqznmfsm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aizwys.cn/gtvokrcesq.html


<!-- 参考信息 -->