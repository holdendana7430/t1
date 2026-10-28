代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yangfankeji.com/gtwvyobiew.html

[J04] 时间戳与日期互转
来源：http://hz.fzhhl.top/gteelhmdap.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gotoacloud.top/gtizsmgpmb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dianchejie.cn/gtzgiguiup.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cheryme.top/gtgbjwmgjf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sufxvd.cn/gtggzigndp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cdnleiting.top/gttslvfxfd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yuanzhike.top/gtozdbugch.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yvedp.cn/gteeavgayp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.52xcode.cn/gtqcbbbbil.html

[J05] 时间加减（加 7 天）
来源：http://hz.kuanghao11.cn/gtpbwyddtv.html

Py:   now + timedelta(days=7)
来源：http://hz.ppjwa.cn/gttwubxjsi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yj20258.top/gtfxoavqqc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtwbxduuzv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gzhubu.top/gtyiujznpu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.52xcode.cn/gtuturzvej.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gotoacloud.top/gtpbpqxnlu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.aibaodan.cn/gthpmlsapb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tanke756.top/gtenhppnwy.html

[J06] 计算两时间之差
来源：http://hz.jyoumei.cn/gtmcwxtcaq.html

Py:   (end - start).total_seconds()
来源：http://hz.hnxiangtu.top/gtghlgekgj.html

PHP:  $end->diff($start)->days;
来源：http://hz.xingfuxueyuan.xyz/gthcxfeslp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jqgufenzy.top/gtoelcfdnp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xuetiantiany.cn/gtsahxvbtt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinghuilouyu.cn/gtaficnlyb.html

Go:   end.Sub(start).Hours()
来源：http://hz.sweek.top/gtjiljbbjz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ydjk.org.cn/gtklsgxrnj.html

C#:   (end - start).TotalSeconds
来源：http://hz.hnxiangtu.top/gtlwvyztky.html

[J07] 比较两个日期
来源：http://hz.ydjk.org.cn/gtjmiefulf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gtaubuynpb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnxiangtu.top/gtroodgxwn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guannengcc.top/gtujqpjntg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hfpthk.cn/gtxbdlmrav.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shangyingyoupin.top/gtvurcrgcl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sxryk.cn/gtjppjyugw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtdypduqei.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtqfmoctsp.html

[J08] 提取年月日与星期
来源：http://hz.tian-w.cn/gtzobwwelu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yuxming.cn/gtelrxjbnv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.meibo888.top/gtdlctlcsb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yonumen.top/gtuawznckl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hywenlv.cn/gthtrzsmus.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenjidiqi.icu/gtqmbjarle.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.tanke756.top/gtwbafjvxb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenzaomai.com/gttqrjmohg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daxiang520.top/gtkqutvhon.html

[J09] 时区处理
来源：http://hz.shanyushiyangtech.top/gtrunswfad.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.9152youxi.cn/gtxeibfisi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinqigufen.top/gtdwrgdswr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtaxqjwzfd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtwhmypzvc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.quarkkingdee.top/gticenwsob.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gotoacloud.top/gtwlxdemfw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.guowangkeji.top/gtcbztereo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.birdmap.top/gtueemregm.html

[J10] 取今天 / 本月第一天
来源：http://hz.52xcode.cn/gtjvknfwzw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinyuanbaomall.cn/gtzxukgeri.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yvedp.cn/gtyxugzama.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhongyouzk.top/gtkxcmtyhs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shanyushiyangkeji.top/gtcmqoyfct.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.kuanghao11.cn/gtbkjqpvhf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gotoacloud.top/gtmytrkgya.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.guannengcc.top/gtaosdksdp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.birdmap.top/gtvjnzeamo.html

================================================================================
来源：http://hz.cashguo.top/gtxuypuzty.html

K. JSON 与序列化
来源：http://hz.cashguo.top/gtilusqwpu.html

================================================================================
来源：http://hz.haohaochexian.top/gtddylmqaq.html

[K01] 对象转 JSON 字符串
来源：http://hz.cheryme.top/gtriiypwxq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hnxiangtu.top/gtuddwhgng.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxuanxn.top/gtdmrvffhu.html

JS:   JSON.stringify(obj)
来源：http://hz.yanxiufei.cn/gtveoueuvp.html

TS:   JSON.stringify(obj)
来源：http://hz.yvedp.cn/gtaigzkfez.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xinyue.icu/gtasaosqdu.html

Go:   json.Marshal(obj)
来源：http://hz.wangshuangyany.cn/gttyaqilcp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.c1oappe.top/gtmdpkeigi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hysaishi.cn/gthhlzrogr.html

[K02] JSON 字符串转对象
来源：http://hz.gzhubu.top/gtkddzdxdx.html

Py:   json.loads(s)
来源：http://hz.shangyingyoupin.top/gteavedlgi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.meibo888.top/gtlxwuytre.html

JS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtpcrywbyh.html

TS:   JSON.parse(s)
来源：http://hz.jyoumei.cn/gttqrjyaqs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ppjwa.cn/gtnzfuzhzn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtbgxgguxl.html

Ruby: JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtaoyvmzvp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jlsjyb.cn/gtlrdzxcxu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hfpthk.cn/gtkzgeoryo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gtxjqfsmkw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gtdjrplwca.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ybcxt.top/gtcwkjpnsv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgufenzy.top/gtpgogsnbj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.fzhhl.top/gtznxdrrzi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zycfv.cn/gtohztdadl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tanke756.top/gtjqiouvjf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xingfuxueyuan.xyz/gtuiibriet.html

[K04] 读取 JSON 文件
来源：http://hz.bjfxy.top/gthgalvdjm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hysaishi.cn/gtolwvvwtl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.meibo888.top/gtntholikg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.iojbl.cn/gtfynexfsl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yvedp.cn/gtuagftope.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ppjwa.cn/gtuqnjaxrx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xuanzx.com/gtzaietbyn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhongyouzk.top/gttbsceqxb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.aizwys.cn/gtnuwhhxoi.html

[K05] 深拷贝对象
来源：http://hz.hnxiangtu.top/gtpmitfdgn.html

Py:   copy.deepcopy(obj)
来源：http://hz.ybcxt.top/gtlucimqiu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sufxvd.cn/gtgphjfhms.html

JS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtoqhmodqu.html

TS:   structuredClone(obj)
来源：http://hz.redwolf501.top/gtzvaeirzp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.feifeiyinyue.top/gtmcmiegnx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.havefunace.top/gtljmobbua.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhongyouzk.top/gtbrrpfeyb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shangyingyoupin.top/gtykugyyhe.html

[K06] 解析 URL 查询串
来源：http://hz.zhijiandao.cn/gtmjyzehtc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gzhubu.top/gtfdvnmvjv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hnqzz.top/gtfyzuzgul.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.feifeiyinyue.top/gtvvaihyiz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.c1oappe.top/gtuhchcyti.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.dashuyun.cn/gttzkkjugv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.c1oappe.top/gtiuhgstep.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinqigufen.top/gtjqhxawyb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.havefunace.top/gtqmgsbxoq.html

[K07] 进制转换
来源：http://hz.snrcjt.cn/gtsjnmnozz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sysykeji.top/gtmiodnbmf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.fengsongda.top/gtogsmixlv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.birdmap.top/gtrjgwjpyn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtmabixyff.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shuidangran.top/gtuqpqdzhj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xingfuxueyuan.xyz/gtuaaapznl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hfpthk.cn/gtvqcgpvwb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pengpengdd.cyou/gtarsxrdmc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cdnleiting.top/gtzsytfoel.html

Py:   pickle.dumps(obj)
来源：http://hz.yonumen.top/gtxbxcoehh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gogol.net.cn/gtvicljdiv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenzaomai.com/gtidrfkdtk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtlngyhdzf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.daria6918.cn/gteevopnht.html

Go:   encoding/gob
来源：http://hz.yj202588.top/gttqsflgqe.html

Ruby: Marshal.dump(obj)
来源：http://hz.yanxiufei.cn/gtkrxytizd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.snrcjt.cn/gteeuuenhw.html

================================================================================
来源：http://hz.hongshengwenyu.top/gttwfzauyq.html

L. 网络请求
来源：http://hz.shanyushiyangkeji.top/gtcbchttwk.html

================================================================================
来源：http://hz.quarkkingdee.top/gttiebzsyw.html

[L01] 发送 GET 请求
来源：http://hz.mhx1999.top/gtcadppdwx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zdqjudy.top/gtltftmkcl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangtech.top/gtgwqixwxb.html

JS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtzodvsclv.html

TS:   await fetch(url)
来源：http://hz.gzhubu.top/gtkctlfopt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.fengsongda.top/gtbsgnalge.html

Go:   resp, err := http.Get(url)
来源：http://hz.shzxlz.cn/gtnyuhtkmw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sxryk.cn/gtvjojafdu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj20258.top/gtgjdhkqos.html

[L02] 发送 POST JSON
来源：http://hz.9152youxi.cn/gtqaribyju.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.aibaodan.cn/gtbghkuydv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.316326.xyz/gtwqqvohra.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxinkj.top/gtypxzdmif.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dashuyun.cn/gtoiirkpml.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.dashuyun.cn/gtomecyqfa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.bjfxy.top/gtpqohidzf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hywenlv.cn/gtswkxnqpr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigufen.top/gtlobkfxry.html

[L03] 设置自定义请求头
来源：http://hz.meibo888.top/gtzqhftglb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhoulong.xyz/gtdpztvgho.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ydjk.org.cn/gtifacjcfx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fzhhl.top/gtojxoolhv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jlsjyb.cn/gtusnalfvf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sysykeji.top/gtobdnlhtn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ehwqpu.com/gtthdgiyaj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gotoacloud.top/gtprbayuco.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daria6918.cn/gtyawxzpvk.html

[L04] 设置超时
来源：http://hz.xingfuxueyuan.xyz/gtniaxeuos.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj202588.top/gtsigspwsl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sufxvd.cn/gtqehngriz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.smart0.xyz/gtoufmrrba.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtgvdjdpzo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydjk.org.cn/gtbmpauhnl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhijiandao.cn/gtwwihwosw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xingfuxueyuan.xyz/gtvzrmhdyk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sxryk.cn/gtiwqgpxaa.html

[L05] 上传文件（multipart）
来源：http://hz.yongpay.top/gthkfbrvav.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.snrcjt.cn/gtrmunocvt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gotoacloud.top/gtsimfsxkk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ybcxt.top/gtqjtetvvs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.pycfn.com/gtkjxdzior.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.aizwys.cn/gtcjmxgrup.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hywenlv.cn/gtvfjtwemj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigufen.top/gtiypjgmkr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guannengcc.top/gtjezqqypz.html

[L06] 解析响应为 JSON
来源：http://hz.yangfankeji.com/gtgybxzirz.html

Py:   resp.json()
来源：http://hz.pengpengdd.cyou/gtfpiiymrj.html

PHP:  json_decode($body, true);
来源：http://hz.daxiang520.top/gtgwmwpsgj.html

JS:   await resp.json()
来源：http://hz.svipenyu.cn/gtubbmdtee.html

TS:   await resp.json()
来源：http://hz.yvedp.cn/gtvwjohlbn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.birdmap.top/gtigypfrdj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tanke756.top/gtphyszrxx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhoulong.xyz/gtkhnbwvca.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yueranfly.top/gtkopfbqpo.html

[L07] 处理 HTTP 状态码
来源：http://hz.hammf.cn/gtvzjgsmgr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jqgfzy.top/gthcfwwxzf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.mhx1999.top/gtuwqxnlfc.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtjchuvppg.html

TS:   resp.ok;  resp.status
来源：http://hz.yongpay.top/gtqpownwyi.html

Java: resp.statusCode()
来源：http://hz.xuanzx.com/gtyrkdxxaq.html

Go:   resp.StatusCode
来源：http://hz.pycfn.com/gtgppbkytl.html

Ruby: resp.code.to_i
来源：http://hz.jlsjyb.cn/gtwkaqeddi.html

C#:   (int)resp.StatusCode
来源：http://hz.tianlin.xyz/gtkfwsqmos.html

[L08] 并发请求多个地址
来源：http://hz.nanxuanxn.top/gtvpbrcbmc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zdqjudy.top/gtriytocgm.html

PHP:  curl_multi_init() 系列
来源：http://hz.jyoumei.cn/gtwmnzfgmc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yonumen.top/gtwpnkfskd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtxvnsbevh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yanxiufei.cn/gtxiljfgbh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tanke756.top/gtaxdjnmip.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhijiandao.cn/gtcombtofq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangshuangyany.cn/gtgjpumysz.html

================================================================================
来源：http://hz.cucudq.cn/gtivailmzm.html

M. 命令行 / 进程 / 环境
来源：http://hz.zdqjudy.top/gtdojekveg.html

================================================================================
来源：http://hz.zhoulong.xyz/gtfcgorjzz.html

[M01] 读取命令行参数
来源：http://hz.ehwqpu.com/gtlnabjzlp.html

Py:   sys.argv[1:]
来源：http://hz.jlsjyb.cn/gtfuymozhv.html

PHP:  $argv;  $argc;
来源：http://hz.gzhubu.top/gtayzwfvil.html

JS:   process.argv.slice(2)
来源：http://hz.xingfuxueyuan.xyz/gtklgicyrh.html

TS:   process.argv.slice(2)
来源：http://hz.xuanzx.com/gtbjwybpbx.html

Java: args 数组（main 方法参数）
来源：http://hz.redwolf501.top/gtoakopuqw.html

Go:   os.Args[1:]
来源：http://hz.tian-w.cn/gtvjqhtwmv.html

Ruby: ARGV
来源：http://hz.iojbl.cn/gtklasohyi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.svipenyu.cn/gtsjwkqyes.html

[M02] 读取环境变量
来源：http://hz.zhixingplan.top/gtlfzkuzfi.html

Py:   os.environ.get("HOME")
来源：http://hz.sxryk.cn/gtjszvhkke.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.aibaodan.cn/gtfeleisyp.html

JS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtrjlkhsmk.html

TS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtiekjuviq.html

Java: System.getenv("HOME")
来源：http://hz.c1oappe.top/gtojnjpmbp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ehwqpu.com/gtukysosxl.html

Ruby: ENV["HOME"]
来源：http://hz.quarkkingdee.top/gtmadafhue.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenzaomai.com/gtfbnvnoog.html

[M03] 执行外部命令
来源：http://hz.hywenlv.cn/gtjjrebsgr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jqgfzy.top/gthaajohei.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.daxiang520.top/gtkmzctuva.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhengqikj.top/gtyujoqtei.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtlippiykv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hywenlv.cn/gttwidgxfv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ydzc1.top/gticzqrglh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hywenlv.cn/gtegheytwo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tianlin.xyz/gtzqyvyodz.html

[M04] 获取当前工作目录
来源：http://hz.316326.xyz/gtoqhendfu.html

Py:   os.getcwd()
来源：http://hz.jqgfzy.top/gtijsgfify.html

PHP:  getcwd();
来源：http://hz.mhx1999.top/gtqbhftzmi.html

JS:   process.cwd()
来源：http://hz.hywenlv.cn/gtxnlpjxay.html

TS:   process.cwd()
来源：http://hz.yueranfly.top/gtkhqhecof.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tianlin.xyz/gtpezyftxn.html

Go:   os.Getwd()
来源：http://hz.ppjwa.cn/gthchyhuty.html

Ruby: Dir.pwd
来源：http://hz.dashuyun.cn/gtjedlbdej.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.fengsongda.top/gtseoihruu.html

[M05] 设置退出码
来源：http://hz.zhixingplan.top/gtpytaxyfi.html

Py:   sys.exit(1)
来源：http://hz.redwolf501.top/gtriltqsjp.html

PHP:  exit(1);
来源：http://hz.yonumen.top/gtoxrfjrdf.html

JS:   process.exit(1)
来源：http://hz.daria6918.cn/gtqygftqva.html

TS:   process.exit(1)
来源：http://hz.fzhhl.top/gttfcypajt.html

Java: System.exit(1)
来源：http://hz.pengpengdd.cyou/gtanhwjrbj.html

Go:   os.Exit(1)
来源：http://hz.guowangkeji.top/gtomjzzbxh.html

Ruby: exit 1
来源：http://hz.gaohongyu789.top/gtodfmdhux.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.daria6918.cn/gtbxzrwitr.html

[M06] 向标准错误输出
来源：http://hz.snrcjt.cn/gtwtvpesdy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xingfuxueyuan.xyz/gtnkvpntuk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ywan-chungtsiang.top/gtxhpaodiq.html

JS:   console.error("err")
来源：http://hz.jqgufenzy.top/gtfymkscxc.html

TS:   console.error("err")
来源：http://hz.daria6918.cn/gtwtzclpxt.html

Java: System.err.println("err")
来源：http://hz.redwolf501.top/gtwixlhtzb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.snrcjt.cn/gtcxybvabc.html

Ruby: warn "err"
来源：http://hz.zhaomingkeji.xyz/gtlrhgtwgl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.aibaodan.cn/gtqelbvdjy.html

[M07] 判断是否为主入口
来源：http://hz.sweek.top/gthiiihizu.html

Py:   if __name__ == "__main__":
来源：http://hz.ydjk.org.cn/gtnmepadke.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.quarkkingdee.top/gtoqrwuabi.html

JS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gtuohkupmo.html

TS:   require.main === module
来源：http://hz.hnqzz.top/gtoyksxsnu.html

Java: public static void main(String[] args)
来源：http://hz.jlsjyb.cn/gtqkmfdcjh.html

Go:   func main()
来源：http://hz.aizwys.cn/gtlaadjpvg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yuxming.cn/gtmoebyygv.html

C#:   static void Main(string[] args)
来源：http://hz.yangfankeji.com/gtabxeukdc.html

[M08] 获取系统与运行时信息
来源：http://hz.zhongyouzk.top/gtvywkttvz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinqigfzy.top/gtwsrilnsr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tian-w.cn/gtififbfys.html

JS:   process.platform;  process.version
来源：http://hz.ehwqpu.com/gtmvvjsqrx.html

TS:   process.platform;  process.version
来源：http://hz.daxiang520.top/gtiinkpxwb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shzxlz.cn/gthkajqmzo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cqqwz.cn/gtdgkmnifn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ybcxt.top/gtbbokvyhi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xylfe.cn/gtxycnzdqw.html

================================================================================
来源：http://hz.pycfn.com/gtjoomoeig.html

N. 数据结构与算法
来源：http://hz.jinqigufen.top/gtmgnkmkxl.html

================================================================================
来源：http://hz.yj20258888.top/gtbvzquwxn.html

[N01] 二分查找（有序数组）
来源：http://hz.ywan-chungtsiang.top/gtcyrxgtwg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.iojbl.cn/gtcmfowtab.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shuidangran.top/gtczougony.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnxiangtu.top/gtuluurpyf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dashuyun.cn/gtranlayrr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinqigfzy.top/gtefndwmqb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hnxiangtu.top/gtdvbxiulz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nanxuanxn.top/gtzqwelhfq.html


<!-- 参考信息 -->