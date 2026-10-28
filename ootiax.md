代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shanyushiyangkeji.top/gtngbyggbe.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.meibo888.top/gtkslcftke.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gotoacloud.top/gtdnjaaook.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ivvv.top/gtkxveyvim.html

[J03] 字符串解析为日期
来源：http://hz.ivvv.top/gticoceriu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.c1oappe.top/gtyncwrpab.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ppjwa.cn/gtxosaxnnc.html

JS:   new Date("2024-01-02")
来源：http://hz.mhx1999.top/gtdjucmzjt.html

TS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtzagddygv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cucudq.cn/gtebaervsu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gogol.net.cn/gtkgzvgbec.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtqimogiyz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shuidangran.top/gttbitdfnv.html

[J04] 时间戳与日期互转
来源：http://hz.hysaishi.cn/gtbspnlvuo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dashuyun.cn/gtnyabtaki.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yvedp.cn/gtvkvljvyg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.birdmap.top/gtcqpydwyh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.smart0.xyz/gtswtnuflj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yuxming.cn/gtjdbzjgia.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sysykeji.top/gtpfonnwyf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.kuanghao11.cn/gtdcvraxkz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dashuyun.cn/gtjuziycqo.html

[J05] 时间加减（加 7 天）
来源：http://hz.shzxlz.cn/gtchtbmjun.html

Py:   now + timedelta(days=7)
来源：http://hz.chenzaomai.com/gttvdbwxhs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ydzc1.top/gtdlvumfcw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guowangkeji.top/gtsafbvdcv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daxiang520.top/gtfgielove.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.bjfxy.top/gtknuikzsm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.tianlin.xyz/gtcdgxfsga.html

Ruby: Time.now + 7 * 86400
来源：http://hz.daxiang520.top/gtkpgycilz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jlsjyb.cn/gtomdpmaja.html

[J06] 计算两时间之差
来源：http://hz.gzhubu.top/gtfplonqha.html

Py:   (end - start).total_seconds()
来源：http://hz.xuanzx.com/gtekvnpvqr.html

PHP:  $end->diff($start)->days;
来源：http://hz.shanyushiyangkeji.top/gtzblubqoy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.mhx1999.top/gtoixtcqls.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sweek.top/gtmxunbrhb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yonumen.top/gtswkajxnk.html

Go:   end.Sub(start).Hours()
来源：http://hz.aibaodan.cn/gtdwbmvccd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.iojbl.cn/gtamyxnbmj.html

C#:   (end - start).TotalSeconds
来源：http://hz.mhx1999.top/gtcqjsizvs.html

[J07] 比较两个日期
来源：http://hz.gaohongyu789.top/gtlfbfyrxl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtklfkoqka.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhixingplan.top/gtuylgkcxn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigfzy.top/gtaqexveao.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.fzhhl.top/gtuuxudbur.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tianlin.xyz/gtrbdxbqqt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xuetiantiany.cn/gtjvfofmur.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gtrocuhkqz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtgigrvafp.html

[J08] 提取年月日与星期
来源：http://hz.fengsongda.top/gtxxmnzwrh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhaomingkeji.xyz/gtmtqmgkpw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhaomingkeji.xyz/gtztjanmrs.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.fzhhl.top/gtyryrggbx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.dianchejie.cn/gtuxfqgpij.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sxryk.cn/gtvxujgabl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj20258.top/gtxcyoyadc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jiagoushi.top/gtkdxknsum.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.mhx1999.top/gtkhzmxjfw.html

[J09] 时区处理
来源：http://hz.ybcxt.top/gttvcaehrp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhengqikj.top/gtfyrbxalf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinghuilouyu.cn/gtirccbmse.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sweek.top/gtifkqucvz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinghuilouyu.cn/gtuybdnlrv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jyoumei.cn/gtnzfffuug.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinqigfzy.top/gtobxuqeqk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jiagoushi.top/gtpxrlagpb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.9152youxi.cn/gtsjljnlwt.html

[J10] 取今天 / 本月第一天
来源：http://hz.hnxiangtu.top/gtdwbwhjcn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.feifeiyinyue.top/gttxwtojqo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jyoumei.cn/gtqrdwcsme.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yangfankeji.com/gteeolzieg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhoulong.xyz/gttmarfpuq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhaomingkeji.xyz/gtvfudbcno.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj20258888.top/gtpeuhgrmx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zdqjudy.top/gtjpqxofsl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tianlin.xyz/gtlaryekmb.html

================================================================================
来源：http://hz.quarkkingdee.top/gtlhitmdli.html

K. JSON 与序列化
来源：http://hz.svipenyu.cn/gtqwpmrhqq.html

================================================================================
来源：http://hz.52xcode.cn/gtsdaxymen.html

[K01] 对象转 JSON 字符串
来源：http://hz.sysykeji.top/gtfgrvfrsx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.52xcode.cn/gtwprdidmz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.dianchejie.cn/gtdqgexcjp.html

JS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtmuseldcx.html

TS:   JSON.stringify(obj)
来源：http://hz.yonumen.top/gtsgrdfryv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenlongwang.top/gtfosfkrga.html

Go:   json.Marshal(obj)
来源：http://hz.zhengqikj.top/gtckqaxupr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.c1oappe.top/gtxkjtaaod.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sweek.top/gtxmvkynjt.html

[K02] JSON 字符串转对象
来源：http://hz.yj20258888.top/gtxdarejit.html

Py:   json.loads(s)
来源：http://hz.hammf.cn/gtzzlvimaq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cqqwz.cn/gtscbfdquh.html

JS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gthjqabxbi.html

TS:   JSON.parse(s)
来源：http://hz.shuidangran.top/gtylorvrvz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tian-w.cn/gteeqyluin.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cdnleiting.top/gtmlibimee.html

Ruby: JSON.parse(s)
来源：http://hz.hywenlv.cn/gtjjxbinfu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhijiandao.cn/gtevocwzib.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xziqi.cn/gtdqyjssma.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.316326.xyz/gtljetsyfs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258.top/gtonhtyfhv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shuidangran.top/gtxanvqqyr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.pycfn.com/gtihjvhxkb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenlongwang.top/gtutmayunp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenzaomai.com/gtkkdidzuj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxinkj.top/gtxrtlcyyy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.feifeiyinyue.top/gturlyxbxb.html

[K04] 读取 JSON 文件
来源：http://hz.xuetiantiany.cn/gtwccvjtdd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jyoumei.cn/gtzcrlwcml.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.fengsongda.top/gthystpfre.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgfzy.top/gtwiabrpce.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.feifeiyinyue.top/gtuqezjuvk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhengqikj.top/gtgcdujhwo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtogisbysh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhengqikj.top/gtzkumisga.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zycfv.cn/gtkdbalojl.html

[K05] 深拷贝对象
来源：http://hz.shuidangran.top/gtdmuzorru.html

Py:   copy.deepcopy(obj)
来源：http://hz.nwbrower.top/gtybyergjw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.pycfn.com/gthudryvus.html

JS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtdjtcstpt.html

TS:   structuredClone(obj)
来源：http://hz.hongshengwenyu.top/gteupxtmmp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xziqi.cn/gtxsokpmmp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zdqjudy.top/gtucfbldkl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinghuilouyu.cn/gtttlnlayz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pycfn.com/gtprgkikws.html

[K06] 解析 URL 查询串
来源：http://hz.aibaodan.cn/gtnsqigeuw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.havefunace.top/gtdtorjswy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cashguo.top/gtzjlilxpn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gtthrsahts.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.0kj1m.cn/gturezqwog.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yueranfly.top/gtpsklddjj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hfpthk.cn/gtqnvtdsce.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.fengsongda.top/gtoyhczuwx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jianghu66.top/gtzxcqmhuy.html

[K07] 进制转换
来源：http://hz.zhiwuduotai.top/gtvgrkwhur.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hnqzz.top/gtboibsccm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xuetiantiany.cn/gthrgynslo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gtnhmqqtsp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ivvv.top/gttvyeqouy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtxkuhttcf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nwbrower.top/gtillchyga.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhixingplan.top/gtvtuhjano.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yvedp.cn/gtwlhiylls.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.pengpengdd.cyou/gtjxessdlb.html

Py:   pickle.dumps(obj)
来源：http://hz.yonumen.top/gtwxyrxfdi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tian-w.cn/gtbmrthwyp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yvedp.cn/gtpmvrehtp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zdqjudy.top/gtalnpbhrk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.0kj1m.cn/gtjchnvuil.html

Go:   encoding/gob
来源：http://hz.pycfn.com/gtctxitvrz.html

Ruby: Marshal.dump(obj)
来源：http://hz.yangfankeji.com/gtuodaaufu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.mhx1999.top/gtrjuxlhut.html

================================================================================
来源：http://hz.jianghu66.top/gtavdhcrcl.html

L. 网络请求
来源：http://hz.gogol.net.cn/gtwpoeajhp.html

================================================================================
来源：http://hz.cheryme.top/gttvtxbvcp.html

[L01] 发送 GET 请求
来源：http://hz.ppjwa.cn/gtvlsnnlpl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.haohaochexian.top/gtpwtifiil.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.pengpengdd.cyou/gttujqcuka.html

JS:   await fetch(url)
来源：http://hz.ivvv.top/gtyzgjlctb.html

TS:   await fetch(url)
来源：http://hz.cucudq.cn/gtrrrcdwaf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gaohongyu789.top/gtaosqzjqj.html

Go:   resp, err := http.Get(url)
来源：http://hz.iojbl.cn/gtsipjnrxe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.svipenyu.cn/gtusewzwom.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhiwuduotai.top/gtmmpxwzmp.html

[L02] 发送 POST JSON
来源：http://hz.daria6918.cn/gtyavroapw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhiwuduotai.top/gtvnyxhgtz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.feifeiyinyue.top/gtkpwcjtlx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtmzjaozbv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fzhhl.top/gtqiulxdys.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hongshengwenyu.top/gtlzkenzfy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenlongwang.top/gtrbqhdipn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.0kj1m.cn/gteqcvrtjj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hongshengwenyu.top/gteamyqsnt.html

[L03] 设置自定义请求头
来源：http://hz.zhaomingkeji.xyz/gtpbfdbmjj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cucudq.cn/gtuigerfko.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.snrcjt.cn/gtqlotiwqc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fengsongda.top/gtqqrgnsge.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pengpengdd.cyou/gtkbicvydf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.bjfxy.top/gtixeqqdjr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yongpay.top/gtytsyazaw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhengqikj.top/gtcxafxenw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ppjwa.cn/gtacttvvkl.html

[L04] 设置超时
来源：http://hz.hammf.cn/gtglpujkdu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yonumen.top/gtqhnbubte.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gogol.net.cn/gtyunebsve.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hysaishi.cn/gtqdzylfdw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gtidpmfzhl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cheryme.top/gtriulndvu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258888.top/gtoefbjtja.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhengqikj.top/gtqmpfweqg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinghuilouyu.cn/gtmudxgvwv.html

[L05] 上传文件（multipart）
来源：http://hz.vqdsnc.cn/gttabsoabg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj20258888.top/gtbvfiuilx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.dianchejie.cn/gtgaevnmux.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tianlin.xyz/gtrgtdscaa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zdqjudy.top/gtpxqhttyd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.chenlongwang.top/gtwzlygxqj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydjk.org.cn/gtpwxgwitl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ehwqpu.com/gtzcqlydys.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tanke756.top/gtmsrlzpjz.html

[L06] 解析响应为 JSON
来源：http://hz.xinyue.icu/gtllbssklz.html

Py:   resp.json()
来源：http://hz.hnxiangtu.top/gtfeyruqnt.html

PHP:  json_decode($body, true);
来源：http://hz.guannengcc.top/gtbtjkrvmd.html

JS:   await resp.json()
来源：http://hz.aizwys.cn/gtwcsogufs.html

TS:   await resp.json()
来源：http://hz.yj20258888.top/gtbdkpydcx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gaohongyu789.top/gtsbjstihd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.vqdsnc.cn/gtxqgoqmsv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.andypj.xyz/gtxnyufpig.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shangyingyoupin.top/gtmvstrpyn.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxinkj.top/gtgzoviycd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nwbrower.top/gtgbglyuxu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj20258888.top/gtghrwsqao.html

JS:   resp.ok;  resp.status
来源：http://hz.xuetiantiany.cn/gtgjbnqpcp.html

TS:   resp.ok;  resp.status
来源：http://hz.jinghuilouyu.cn/gthbsdaama.html

Java: resp.statusCode()
来源：http://hz.c1oappe.top/gtmmmlwnnd.html

Go:   resp.StatusCode
来源：http://hz.jiagoushi.top/gtsbgmjekx.html

Ruby: resp.code.to_i
来源：http://hz.chenjidiqi.icu/gtskaqbfms.html

C#:   (int)resp.StatusCode
来源：http://hz.tianlin.xyz/gtpkdaozwg.html

[L08] 并发请求多个地址
来源：http://hz.dashuyun.cn/gtdxebjhms.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cashguo.top/gtdoiqtdhy.html

PHP:  curl_multi_init() 系列
来源：http://hz.cashguo.top/gtiseactoe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtbvnnjvlz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnxiangtu.top/gtopvkcxkc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jlsjyb.cn/gtyqgwlkrj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.52xcode.cn/gtyazcnqed.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.snrcjt.cn/gtqtkkdxil.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daria6918.cn/gtafmpczgt.html

================================================================================
来源：http://hz.jiagoushi.top/gttuphnvxz.html

M. 命令行 / 进程 / 环境
来源：http://hz.sysykeji.top/gtpcbjdnnc.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtdotwpvaw.html

[M01] 读取命令行参数
来源：http://hz.cashguo.top/gtctihituv.html

Py:   sys.argv[1:]
来源：http://hz.zhiwuduotai.top/gtihwlelhi.html

PHP:  $argv;  $argc;
来源：http://hz.gzhubu.top/gtzvctyvyk.html

JS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtnumwrxqh.html

TS:   process.argv.slice(2)
来源：http://hz.hfpthk.cn/gtgvgetqsw.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigfzy.top/gtrxvqcxdf.html

Go:   os.Args[1:]
来源：http://hz.birdmap.top/gttiwnpeez.html

Ruby: ARGV
来源：http://hz.316326.xyz/gtagaogcgp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.daxiang520.top/gtsybrxmlu.html

[M02] 读取环境变量
来源：http://hz.zhongyouzk.top/gtvphnumrh.html

Py:   os.environ.get("HOME")
来源：http://hz.hnxiangtu.top/gtcbblrtoc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xuetiantiany.cn/gttqeyyqys.html

JS:   process.env.HOME
来源：http://hz.sysykeji.top/gttbzgwqrl.html

TS:   process.env.HOME
来源：http://hz.cheryme.top/gtzedurhwe.html

Java: System.getenv("HOME")
来源：http://hz.316326.xyz/gtyhlublbl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xziqi.cn/gtnnbzvkee.html

Ruby: ENV["HOME"]
来源：http://hz.ywan-chungtsiang.top/gtsdejbobv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinqigufen.top/gtrldprota.html

[M03] 执行外部命令
来源：http://hz.ywan-chungtsiang.top/gtukvxkgnt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shuidangran.top/gttcoeosow.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.birdmap.top/gtbqwowcou.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhixingplan.top/gtidpponfh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.9152youxi.cn/gtuifuikip.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gaohongyu789.top/gtsnvslxgt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yuanzhike.top/gtudcsmiom.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.dianchejie.cn/gttcmlogve.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cucudq.cn/gtccdisgsz.html

[M04] 获取当前工作目录
来源：http://hz.jqgfzy.top/gtcwofnoai.html

Py:   os.getcwd()
来源：http://hz.zhongyouzk.top/gtbfjtzvtn.html

PHP:  getcwd();
来源：http://hz.jyoumei.cn/gtnkebisgu.html

JS:   process.cwd()
来源：http://hz.xingfuxueyuan.xyz/gtikbqyvvz.html

TS:   process.cwd()
来源：http://hz.smart0.xyz/gtqpzrukro.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.haohaochexian.top/gtkpzfpxjs.html

Go:   os.Getwd()
来源：http://hz.wangshuangyany.cn/gtenpaqqgu.html

Ruby: Dir.pwd
来源：http://hz.daxiang520.top/gtuvefwmoe.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenlongwang.top/gtxpqiqsyj.html

[M05] 设置退出码
来源：http://hz.havefunace.top/gtplosnjpp.html

Py:   sys.exit(1)
来源：http://hz.yangfankeji.com/gtcrsdzpjt.html

PHP:  exit(1);
来源：http://hz.gzhubu.top/gthryxsnbp.html

JS:   process.exit(1)
来源：http://hz.yj202588.top/gtrpjsczbb.html

TS:   process.exit(1)
来源：http://hz.zhijiandao.cn/gtrfxsogzg.html

Java: System.exit(1)
来源：http://hz.vqdsnc.cn/gtpgnnowdv.html

Go:   os.Exit(1)
来源：http://hz.yj202588.top/gtdrspiqmd.html

Ruby: exit 1
来源：http://hz.zycfv.cn/gtkcdthuyj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jlsjyb.cn/gtvkruhlvl.html

[M06] 向标准错误输出
来源：http://hz.fzhhl.top/gtwyozvqua.html

Py:   print("err", file=sys.stderr)
来源：http://hz.quarkkingdee.top/gtbvhgbgdf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cheryme.top/gtiyngvizp.html

JS:   console.error("err")
来源：http://hz.jyoumei.cn/gttdsxqlbx.html

TS:   console.error("err")
来源：http://hz.chenzaomai.com/gtckbujsaq.html

Java: System.err.println("err")
来源：http://hz.fengsongda.top/gtoquqxhqz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinqigfzy.top/gtkeadvcdt.html

Ruby: warn "err"
来源：http://hz.hfpthk.cn/gtszpnwacj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dashuyun.cn/gtwzdjewdj.html

[M07] 判断是否为主入口
来源：http://hz.svipenyu.cn/gtbisyyusk.html

Py:   if __name__ == "__main__":
来源：http://hz.ivvv.top/gtftcmodxy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yanxiufei.cn/gtvvsvfigq.html

JS:   require.main === module
来源：http://hz.nwbrower.top/gtlzezawml.html

TS:   require.main === module
来源：http://hz.zhongyouzk.top/gtdbdwwqjv.html

Java: public static void main(String[] args)
来源：http://hz.gotoacloud.top/gtaiwubahg.html

Go:   func main()
来源：http://hz.jinghuilouyu.cn/gtwjhblfdk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.haohaochexian.top/gtjabfurpt.html

C#:   static void Main(string[] args)
来源：http://hz.yj20258888.top/gtytoczfbg.html

[M08] 获取系统与运行时信息
来源：http://hz.chenjidiqi.icu/gtwqzqynry.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhiwuduotai.top/gtluqkmwli.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj202588.top/gtlbebmlqn.html

JS:   process.platform;  process.version
来源：http://hz.redwolf501.top/gtdjrafhmv.html

TS:   process.platform;  process.version
来源：http://hz.tianlin.xyz/gtawwtlypd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tianlin.xyz/gtjbehjkbs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgufenzy.top/gtsaapenwm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cheryme.top/gtklerzudr.html


<!-- 参考信息 -->