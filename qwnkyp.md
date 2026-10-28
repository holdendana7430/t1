代发 wailian999

Go:   time.Now()
来源：http://hz.daxiang520.top/gtneefkfgi.html

Ruby: Time.now
来源：http://hz.ybcxt.top/gtwprrqrox.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tanke756.top/gtbyjassty.html

[J02] 格式化输出
来源：http://hz.jinghuilouyu.cn/gtpsttlkzo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtnxcpophm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhixingplan.top/gtzxkbsfmg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenlongwang.top/gtpdtvjumh.html

TS:   d.toISOString()
来源：http://hz.xuetiantiany.cn/gtqxklnocy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gotoacloud.top/gtnytckdei.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj20258.top/gtxxhqhygh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.0kj1m.cn/gtvvdchocw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yongpay.top/gtizpcsedp.html

[J03] 字符串解析为日期
来源：http://hz.gaohongyu789.top/gtdfgkoirz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.dianchejie.cn/gtzgxeqvad.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cucudq.cn/gtmhuomwxi.html

JS:   new Date("2024-01-02")
来源：http://hz.quarkkingdee.top/gtumrsdtsa.html

TS:   new Date("2024-01-02")
来源：http://hz.zhoulong.xyz/gtdvvbkmwe.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shzxlz.cn/gtbwlloocm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxinkj.top/gtugwidknw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtmhevzypp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shangyingyoupin.top/gtotyzzgnm.html

[J04] 时间戳与日期互转
来源：http://hz.nanxinkj.top/gtcpplgzqs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nanxinkj.top/gtvsnmvybr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hammf.cn/gtkpkwlqap.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nanxuanxn.top/gtxczerxyc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.feifeiyinyue.top/gtfwkxprxh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258888.top/gtuyarfrej.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zycfv.cn/gtpzrphely.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tianlin.xyz/gtjvlivbyh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.iojbl.cn/gtgqeihznn.html

[J05] 时间加减（加 7 天）
来源：http://hz.jlsjyb.cn/gtavjbspja.html

Py:   now + timedelta(days=7)
来源：http://hz.kuanghao11.cn/gtfcralczh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenlongwang.top/gtbdpmgwzz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangtech.top/gtqxdikcuv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yanxiufei.cn/gtaswfthdj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.kuanghao11.cn/gthgdpyzwt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.guannengcc.top/gtedgbwqcr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hammf.cn/gtamrlpejc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.0kj1m.cn/gtebabpudb.html

[J06] 计算两时间之差
来源：http://hz.zhengqikj.top/gtcmrygchm.html

Py:   (end - start).total_seconds()
来源：http://hz.gzhubu.top/gtgledadnw.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinyuanbaomall.cn/gtwlcbnmge.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhijiandao.cn/gtaxmzzxno.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hongshengwenyu.top/gtgqchvqsc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xylfe.cn/gtxmrslcqu.html

Go:   end.Sub(start).Hours()
来源：http://hz.sufxvd.cn/gtorulzxwg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgfzy.top/gtrmdlgypi.html

C#:   (end - start).TotalSeconds
来源：http://hz.andypj.xyz/gtfonowaaj.html

[J07] 比较两个日期
来源：http://hz.zhengqikj.top/gteauylrwz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtmlmrtmnh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.bjfxy.top/gtxfqmgbpa.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtcnzztqzt.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtxpcbyehy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xuetiantiany.cn/gtkvgelaej.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shanyushiyangkeji.top/gtokaaevzx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hysaishi.cn/gtshzkrydq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtzleddxpf.html

[J08] 提取年月日与星期
来源：http://hz.tian-w.cn/gtbkkkkqvu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tianlin.xyz/gtuotnnhzx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xziqi.cn/gtlrswdlxp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.c1oappe.top/gtszaiewbs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yuanzhike.top/gtgmgteapv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xinyue.icu/gtkmqzxtai.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.haohaochexian.top/gtnztedhae.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cucudq.cn/gtlkkcymrt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhijiandao.cn/gtoncyizsh.html

[J09] 时区处理
来源：http://hz.gzhubu.top/gtaaxjqinp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhongyouzk.top/gtbrcvnoez.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gotoacloud.top/gtnyealnvw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigufen.top/gtvnfagaas.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhoulong.xyz/gtjsopjonv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.52xcode.cn/gtoejrogwa.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sufxvd.cn/gtswkrkzjr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hysaishi.cn/gtgjcaehpt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hnxiangtu.top/gtumivtlqb.html

[J10] 取今天 / 本月第一天
来源：http://hz.yonumen.top/gtchvvaypq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhixingplan.top/gtqkrhqqii.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.316326.xyz/gtyjkdqixt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cdnleiting.top/gtrmbpcjoi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.andypj.xyz/gttssapdsd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cqqwz.cn/gtcnlwkyiw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.fzhhl.top/gtkysmxuaj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.meibo888.top/gtdanthbfh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dashuyun.cn/gtxnyystge.html

================================================================================
来源：http://hz.sxryk.cn/gtcivywfcb.html

K. JSON 与序列化
来源：http://hz.yanxiufei.cn/gttgdrmvak.html

================================================================================
来源：http://hz.aizwys.cn/gtygyzmygt.html

[K01] 对象转 JSON 字符串
来源：http://hz.0kj1m.cn/gtpvqhwhfy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj202588.top/gtgrxvieuj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gotoacloud.top/gtqbxmillm.html

JS:   JSON.stringify(obj)
来源：http://hz.kuanghao11.cn/gtciikncij.html

TS:   JSON.stringify(obj)
来源：http://hz.yvedp.cn/gtsbggoban.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zycfv.cn/gtjvxvhiha.html

Go:   json.Marshal(obj)
来源：http://hz.jianghu66.top/gtwjeltsnu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yuanzhike.top/gtujgynjrt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xziqi.cn/gtalqedqcd.html

[K02] JSON 字符串转对象
来源：http://hz.pycfn.com/gtmmhwyelt.html

Py:   json.loads(s)
来源：http://hz.jinghuilouyu.cn/gtpkjxppeb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhijiandao.cn/gtdtazktkg.html

JS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtlfewssqf.html

TS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtebpxgeys.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nwbrower.top/gtwzhdolny.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.kuanghao11.cn/gtdlnsrqiz.html

Ruby: JSON.parse(s)
来源：http://hz.zycfv.cn/gtoeyhlwbo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cqqwz.cn/gtzstfbgbh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydjk.org.cn/gtiqsxaehq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhaomingkeji.xyz/gtqzygtkvn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gzhubu.top/gtqhmbomar.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xylfe.cn/gtrqqimahj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnxiangtu.top/gthdjofvlz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.52xcode.cn/gtoyzrmbsf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigfzy.top/gtygxzxlsv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnqzz.top/gtvdvkokdu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cqqwz.cn/gtvlexcjbw.html

[K04] 读取 JSON 文件
来源：http://hz.jqgfzy.top/gtmynzukmd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ivvv.top/gtztefnodb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.haohaochexian.top/gtmmbawwin.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.9152youxi.cn/gttpqdzudk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtfzpnygxp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jianghu66.top/gtkwkbbvmw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xingfuxueyuan.xyz/gtbktvfzmm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj20258888.top/gtgbiovzxd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jyoumei.cn/gtberiqxoz.html

[K05] 深拷贝对象
来源：http://hz.cdnleiting.top/gtbyrpudae.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258.top/gtpwgqshhb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ydjk.org.cn/gtoomklois.html

JS:   structuredClone(obj)
来源：http://hz.c1oappe.top/gtncykiera.html

TS:   structuredClone(obj)
来源：http://hz.xuanzx.com/gtaodslylp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jqgfzy.top/gtokxyrrnf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xuetiantiany.cn/gtcoaiskgk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.mhx1999.top/gtvueobtej.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.fengsongda.top/gtkyynnoiy.html

[K06] 解析 URL 查询串
来源：http://hz.ehwqpu.com/gtxbaqvelz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhijiandao.cn/gtehipgyyo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.meibo888.top/gtlyttrvoq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gogol.net.cn/gtktkbucpl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtjlewdrjk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenlongwang.top/gtaaqzvtlu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenlongwang.top/gtenqrrhwv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtcgwkprri.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xziqi.cn/gtzhobgdyd.html

[K07] 进制转换
来源：http://hz.zhengqikj.top/gtsapczjhi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.smart0.xyz/gthgfckvyv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.9152youxi.cn/gtksskxbna.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yonumen.top/gtbvvzmoel.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtddwnbqou.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtjfxwmmcl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zycfv.cn/gtapilebqw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hfpthk.cn/gtppagudfs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ehwqpu.com/gtyrzcfzhn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xinyue.icu/gttzatdsmv.html

Py:   pickle.dumps(obj)
来源：http://hz.jinqigfzy.top/gtaqdmeqzj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tian-w.cn/gtwiafukky.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hywenlv.cn/gtxfybryjq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtswgusgjz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shuidangran.top/gthfgstolt.html

Go:   encoding/gob
来源：http://hz.jinqigfzy.top/gtqhgaxjdj.html

Ruby: Marshal.dump(obj)
来源：http://hz.fengsongda.top/gtvjhlaalw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.birdmap.top/gtmfkecgab.html

================================================================================
来源：http://hz.meibo888.top/gtcvzvfxdm.html

L. 网络请求
来源：http://hz.tianlin.xyz/gtncpyztzr.html

================================================================================
来源：http://hz.ybcxt.top/gtqvchskcx.html

[L01] 发送 GET 请求
来源：http://hz.xinyue.icu/gtzjphsjpu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yangfankeji.com/gtcnskuekk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yueranfly.top/gtvauyigsw.html

JS:   await fetch(url)
来源：http://hz.jinqigfzy.top/gtwjvsqduw.html

TS:   await fetch(url)
来源：http://hz.iojbl.cn/gtbuawubdk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cheryme.top/gtlwhmorih.html

Go:   resp, err := http.Get(url)
来源：http://hz.hnxiangtu.top/gtsqeoxhba.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.andypj.xyz/gtdmtncifn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ppjwa.cn/gtwuxitidz.html

[L02] 发送 POST JSON
来源：http://hz.haohaochexian.top/gtuqympiih.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.kuanghao11.cn/gtttpnqhog.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shanyushiyangkeji.top/gtesjysjlx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cheryme.top/gthfsdisoy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gzhubu.top/gtubwhrjpd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hammf.cn/gtfknlftzx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gzhubu.top/gtbruyyoxy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gzhubu.top/gtnuitmfvv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nwbrower.top/gtaopecpfn.html

[L03] 设置自定义请求头
来源：http://hz.smart0.xyz/gtzimtgumi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cqqwz.cn/gttsawkfyf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.dianchejie.cn/gtvovccskm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydjk.org.cn/gtnxznvepr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangtech.top/gtvxwsafxr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj20258.top/gtybsduqpr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhongyouzk.top/gtavzcgaxn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cashguo.top/gtrznirrdl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tanke756.top/gtrjuowllc.html

[L04] 设置超时
来源：http://hz.yongpay.top/gtaxkwhiwq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.pycfn.com/gtxgdvleah.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.kuanghao11.cn/gtzauirsyc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cdnleiting.top/gtocwoqoyk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtszoadimv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.havefunace.top/gtmqwgnxsz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.mhx1999.top/gtbfymlukq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.pengpengdd.cyou/gtczqeohqk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hysaishi.cn/gtewgffvzs.html

[L05] 上传文件（multipart）
来源：http://hz.ywan-chungtsiang.top/gtbofafaru.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tianlin.xyz/gtkwufcvkm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yj20258.top/gtbwsrisev.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtuucqmssa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigufen.top/gtutjbcgvp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yuanzhike.top/gtzjchivcd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.c1oappe.top/gtodtkmsjf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj20258.top/gtjnieyvme.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yanxiufei.cn/gtllwdryql.html

[L06] 解析响应为 JSON
来源：http://hz.daria6918.cn/gtvlderctc.html

Py:   resp.json()
来源：http://hz.chenlongwang.top/gtnkhzuulr.html

PHP:  json_decode($body, true);
来源：http://hz.jiagoushi.top/gtqseorsms.html

JS:   await resp.json()
来源：http://hz.xingfuxueyuan.xyz/gtcffxyqgf.html

TS:   await resp.json()
来源：http://hz.cdnleiting.top/gtbhlzjztu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.c1oappe.top/gtfasmaoka.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj20258.top/gtfmxjtzkm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.nwbrower.top/gtofizqkvs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aizwys.cn/gticnwngci.html

[L07] 处理 HTTP 状态码
来源：http://hz.birdmap.top/gtiryzhtut.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.0kj1m.cn/gtdezkamjx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.daria6918.cn/gtzydprgsv.html

JS:   resp.ok;  resp.status
来源：http://hz.smart0.xyz/gtyorlxhqi.html

TS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gtpmdimczv.html

Java: resp.statusCode()
来源：http://hz.sxryk.cn/gtdydmovsq.html

Go:   resp.StatusCode
来源：http://hz.hammf.cn/gticjcvwtu.html

Ruby: resp.code.to_i
来源：http://hz.yuxming.cn/gtagnzzxnn.html

C#:   (int)resp.StatusCode
来源：http://hz.ywan-chungtsiang.top/gtgetehxjw.html

[L08] 并发请求多个地址
来源：http://hz.ydjk.org.cn/gtnriskmkw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinghuilouyu.cn/gtjitriurf.html

PHP:  curl_multi_init() 系列
来源：http://hz.yanxiufei.cn/gtwekevadd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtzuqznzat.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenjidiqi.icu/gtvupqbdmd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.svipenyu.cn/gtwgaqhozn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hammf.cn/gteeidfllt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.meibo888.top/gtvdlhixwz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.mhx1999.top/gtfgphhnbg.html

================================================================================
来源：http://hz.nanxinkj.top/gtleugsjui.html

M. 命令行 / 进程 / 环境
来源：http://hz.mhx1999.top/gtcdygddag.html

================================================================================
来源：http://hz.haohaochexian.top/gtibavrejy.html

[M01] 读取命令行参数
来源：http://hz.bjfxy.top/gtdjasnhfc.html

Py:   sys.argv[1:]
来源：http://hz.cdnleiting.top/gtunlqipqp.html

PHP:  $argv;  $argc;
来源：http://hz.chenlongwang.top/gtwmwfsnwo.html

JS:   process.argv.slice(2)
来源：http://hz.guannengcc.top/gtdkxwzjkk.html

TS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtmcjrcrrg.html

Java: args 数组（main 方法参数）
来源：http://hz.dashuyun.cn/gtdzcptiym.html

Go:   os.Args[1:]
来源：http://hz.ydzc1.top/gtgyeymdra.html

Ruby: ARGV
来源：http://hz.zhaomingkeji.xyz/gtgdyzrpvg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sweek.top/gtnczyyiwa.html

[M02] 读取环境变量
来源：http://hz.tianlin.xyz/gtyzrqyrjd.html

Py:   os.environ.get("HOME")
来源：http://hz.bjfxy.top/gtdifqzjwj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenlongwang.top/gtiiriqfid.html

JS:   process.env.HOME
来源：http://hz.jlsjyb.cn/gtfcurjfcw.html

TS:   process.env.HOME
来源：http://hz.jqgfzy.top/gtckrbycvl.html

Java: System.getenv("HOME")
来源：http://hz.sweek.top/gtvsphtuqt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hywenlv.cn/gtcogifnqz.html

Ruby: ENV["HOME"]
来源：http://hz.fengsongda.top/gtuylnumil.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ydjk.org.cn/gtgtpjwvql.html

[M03] 执行外部命令
来源：http://hz.jyoumei.cn/gtzxraewru.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.0kj1m.cn/gteickyivt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guannengcc.top/gtpgggjkxn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.0kj1m.cn/gthgngkwll.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cheryme.top/gtayiafgwc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.kuanghao11.cn/gtzjwucjlw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jianghu66.top/gtzajlvtdg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hfpthk.cn/gtyhenkxlb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xuanzx.com/gtolupdehx.html

[M04] 获取当前工作目录
来源：http://hz.shangyingyoupin.top/gtsjaqyxnx.html

Py:   os.getcwd()
来源：http://hz.cashguo.top/gthhbykpli.html

PHP:  getcwd();
来源：http://hz.cucudq.cn/gtontskmge.html

JS:   process.cwd()
来源：http://hz.xuanzx.com/gtgdqlzzvy.html

TS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtnhvnmhfm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xinyue.icu/gtzvamxywd.html

Go:   os.Getwd()
来源：http://hz.yanxiufei.cn/gtjkgoittv.html

Ruby: Dir.pwd
来源：http://hz.meibo888.top/gthagyiemn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.aizwys.cn/gtsqniyysb.html

[M05] 设置退出码
来源：http://hz.cucudq.cn/gtxamvoitm.html

Py:   sys.exit(1)
来源：http://hz.iojbl.cn/gtoktzruol.html

PHP:  exit(1);
来源：http://hz.xinyue.icu/gtyulpgiab.html

JS:   process.exit(1)
来源：http://hz.yj202588.top/gtocvorird.html

TS:   process.exit(1)
来源：http://hz.hywenlv.cn/gtsdonbzri.html

Java: System.exit(1)
来源：http://hz.ydjk.org.cn/gtfihrjkku.html

Go:   os.Exit(1)
来源：http://hz.havefunace.top/gtevmnhwmz.html

Ruby: exit 1
来源：http://hz.gzhubu.top/gtkdgcuqyy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yanxiufei.cn/gtgefybbhj.html

[M06] 向标准错误输出
来源：http://hz.tian-w.cn/gtxefzrtet.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shuidangran.top/gtsekisdmw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xziqi.cn/gtfinqjntn.html

JS:   console.error("err")
来源：http://hz.zhengqikj.top/gtbnulrpmk.html

TS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gtqhmypfvz.html

Java: System.err.println("err")
来源：http://hz.yj20258.top/gtudjdyqhs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xingfuxueyuan.xyz/gtelbzoiox.html

Ruby: warn "err"
来源：http://hz.bjfxy.top/gthytkboys.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.fengsongda.top/gtxxmeszjs.html

[M07] 判断是否为主入口
来源：http://hz.hywenlv.cn/gtpzdhhpio.html

Py:   if __name__ == "__main__":
来源：http://hz.dianchejie.cn/gtciattowk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yvedp.cn/gtuxclaptl.html

JS:   require.main === module
来源：http://hz.shangyingyoupin.top/gtmemhpwdl.html

TS:   require.main === module
来源：http://hz.ehwqpu.com/gtysdfzdim.html

Java: public static void main(String[] args)
来源：http://hz.chenjidiqi.icu/gthqkdnqtv.html

Go:   func main()
来源：http://hz.yanxiufei.cn/gttvstwlmh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ppjwa.cn/gtzzvbskmc.html

C#:   static void Main(string[] args)
来源：http://hz.havefunace.top/gthrbetnnd.html


<!-- 参考信息 -->