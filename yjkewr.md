代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.kuanghao11.cn/gtkqywbrdu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinghuilouyu.cn/gttyshibvv.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj202588.top/gtdhpxstkz.html

Py:   now + timedelta(days=7)
来源：http://hz.sweek.top/gtrhqidcfg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jlsjyb.cn/gtzepgncrf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cashguo.top/gthlliubht.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ehwqpu.com/gtovxkewvd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tian-w.cn/gthfgesovz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shuidangran.top/gtbohuxkuq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jiagoushi.top/gtjnfkwfgp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.guowangkeji.top/gtcvdiuszk.html

[J06] 计算两时间之差
来源：http://hz.snrcjt.cn/gtgdlopimy.html

Py:   (end - start).total_seconds()
来源：http://hz.havefunace.top/gtjourcscd.html

PHP:  $end->diff($start)->days;
来源：http://hz.sufxvd.cn/gtbvyyleba.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.redwolf501.top/gtinhgfoub.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xziqi.cn/gtexkarddw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jqgfzy.top/gtifmbeyip.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnqzz.top/gtkgqnpvtr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hywenlv.cn/gthynbxhcc.html

C#:   (end - start).TotalSeconds
来源：http://hz.yangfankeji.com/gtevqbskji.html

[J07] 比较两个日期
来源：http://hz.tianlin.xyz/gtagetkycl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtchpfzlgr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ydjk.org.cn/gtjxhroiqi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtonkzzbmp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gtlbcpdkbk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhijiandao.cn/gtrqshmwsc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hammf.cn/gtfnspleqc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gttczwpvcj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtxfexdrrg.html

[J08] 提取年月日与星期
来源：http://hz.sweek.top/gtgbkkobpj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.wangshuangyany.cn/gtwzqkfnxp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yueranfly.top/gturwlrfeq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yonumen.top/gtwkssnnfq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hongshengwenyu.top/gtmkppdsxh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.pycfn.com/gtitxmjlxb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jyoumei.cn/gtvstorgaq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.smart0.xyz/gtuervcyez.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.316326.xyz/gtsfsylupv.html

[J09] 时区处理
来源：http://hz.guannengcc.top/gtgrispjgc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zycfv.cn/gtqowofzdo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.kuanghao11.cn/gtpxgmicfq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ivvv.top/gtphxgkaye.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtndhqyzjw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.pycfn.com/gtnadhuzho.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zdqjudy.top/gtvbuhdlgi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.pycfn.com/gtlwypnxzb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dianchejie.cn/gtevclqpef.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj202588.top/gtjqfztymr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tian-w.cn/gtfpvxuuud.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhiwuduotai.top/gtybvldjzo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yueranfly.top/gtcdmkdbeh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.haohaochexian.top/gtwtucxstx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgufenzy.top/gtomciljrj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ehwqpu.com/gtmlyjhpwn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj202588.top/gtrqxmipoj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xylfe.cn/gtzapeftmd.html

================================================================================
来源：http://hz.kuanghao11.cn/gttbkzacrg.html

K. JSON 与序列化
来源：http://hz.zhengqikj.top/gtokydbodk.html

================================================================================
来源：http://hz.yanxiufei.cn/gtnhlharln.html

[K01] 对象转 JSON 字符串
来源：http://hz.sysykeji.top/gtasprppjb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.guannengcc.top/gtqfwncuxe.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.wangdashe.top/gthmrlczgn.html

JS:   JSON.stringify(obj)
来源：http://hz.hnqzz.top/gtjlthhsmr.html

TS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtbzscqlum.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.redwolf501.top/gtbwrjfsag.html

Go:   json.Marshal(obj)
来源：http://hz.birdmap.top/gtzuptdest.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.fzhhl.top/gtaajwmqvx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cdnleiting.top/gttbokbpsj.html

[K02] JSON 字符串转对象
来源：http://hz.316326.xyz/gtwpemukmd.html

Py:   json.loads(s)
来源：http://hz.jinghuilouyu.cn/gtezmylaem.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangshuangyany.cn/gtnkvwkszn.html

JS:   JSON.parse(s)
来源：http://hz.iojbl.cn/gtxscepyyf.html

TS:   JSON.parse(s)
来源：http://hz.zhixingplan.top/gtwgbyixbn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.havefunace.top/gtcnenhdim.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.bjfxy.top/gtewfsemvl.html

Ruby: JSON.parse(s)
来源：http://hz.nwbrower.top/gtikicodvq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.fengsongda.top/gtdlqxfoht.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yonumen.top/gtlzkmhccp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yanxiufei.cn/gtbvdvfqrs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtmpkcnbyw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigufen.top/gtnzppcydu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtefwvrvjo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhaomingkeji.xyz/gthrjcouwm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jiagoushi.top/gtvrauvcky.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hammf.cn/gtdoqbunka.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cucudq.cn/gtzfenntcc.html

[K04] 读取 JSON 文件
来源：http://hz.52xcode.cn/gtuldtuodr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sysykeji.top/gtgrovaeiw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tanke756.top/gtpvyvwjgd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258888.top/gtfqjiazyh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xuetiantiany.cn/gtjghdveya.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.snrcjt.cn/gtxlyuszhx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.c1oappe.top/gtdljtokgk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinghuilouyu.cn/gthqwhzqtu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yanxiufei.cn/gtwrexbfxb.html

[K05] 深拷贝对象
来源：http://hz.yongpay.top/gtzhaivsub.html

Py:   copy.deepcopy(obj)
来源：http://hz.52xcode.cn/gteziqmjxt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.quarkkingdee.top/gthpbhkhli.html

JS:   structuredClone(obj)
来源：http://hz.jqgufenzy.top/gtunzypkzy.html

TS:   structuredClone(obj)
来源：http://hz.svipenyu.cn/gtbuwibytn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.iojbl.cn/gtadgorcpu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ppjwa.cn/gtltkezurq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.iojbl.cn/gtnqrkulaf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.meibo888.top/gtaieuzjaj.html

[K06] 解析 URL 查询串
来源：http://hz.iojbl.cn/gtevwxvbsn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hammf.cn/gtpgghjuep.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yueranfly.top/gtlvbplltt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hfpthk.cn/gtuokmafmg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenjidiqi.icu/gtuymdkizg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.feifeiyinyue.top/gtxkajhtqs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shuidangran.top/gtuascyhqy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.redwolf501.top/gtcvckgond.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.dashuyun.cn/gtyhccxrae.html

[K07] 进制转换
来源：http://hz.sweek.top/gtcwscsjbe.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yonumen.top/gtowkktmhb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yangfankeji.com/gtfygyfnrh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtkepbkyer.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtwhhgnaxg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtyoyvalim.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xuanzx.com/gtvlrajazt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.quarkkingdee.top/gtfdrgznbx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jqgufenzy.top/gtdnfdbdse.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ybcxt.top/gtldeukklg.html

Py:   pickle.dumps(obj)
来源：http://hz.aibaodan.cn/gtuehpaicc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.svipenyu.cn/gtyhebkcpr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtiuznrqfk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gtxyhctnmt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cucudq.cn/gtiiwqlgzs.html

Go:   encoding/gob
来源：http://hz.snrcjt.cn/gtxvmqggvt.html

Ruby: Marshal.dump(obj)
来源：http://hz.guannengcc.top/gtresqubqt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xziqi.cn/gtcqxcbpgd.html

================================================================================
来源：http://hz.xuetiantiany.cn/gttumhfxbq.html

L. 网络请求
来源：http://hz.shangyingyoupin.top/gtcirrlxks.html

================================================================================
来源：http://hz.yj20258.top/gtyncbxepg.html

[L01] 发送 GET 请求
来源：http://hz.cdnleiting.top/gtemskkdvc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.bjfxy.top/gtsixymjlj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.bjfxy.top/gtlzftkjpv.html

JS:   await fetch(url)
来源：http://hz.sxryk.cn/gtworktlyb.html

TS:   await fetch(url)
来源：http://hz.zhixingplan.top/gtiafjodpr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydzc1.top/gthvhnktxs.html

Go:   resp, err := http.Get(url)
来源：http://hz.daxiang520.top/gtwyxhgfyl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nwbrower.top/gtqzxdjpis.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shuidangran.top/gtyvhxpbql.html

[L02] 发送 POST JSON
来源：http://hz.hammf.cn/gtlsvrlzty.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgufenzy.top/gtwkusndsi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hnqzz.top/gtjbwyypho.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gtkojfbkll.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cdnleiting.top/gtwgfbgljv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258.top/gtupnvtwgx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenlongwang.top/gtmylzkouf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxuanxn.top/gttphlvloi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zdqjudy.top/gtkoacqjax.html

[L03] 设置自定义请求头
来源：http://hz.chenlongwang.top/gtmvljeepc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhiwuduotai.top/gtcutajdfm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jlsjyb.cn/gthpqlnxfm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sufxvd.cn/gtzclxvkpv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.52xcode.cn/gtkrjvgowk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhoulong.xyz/gtwfsooqis.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhaomingkeji.xyz/gtlfjuvtmo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.snrcjt.cn/gtohuwmcuy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.guowangkeji.top/gtiejuqvne.html

[L04] 设置超时
来源：http://hz.redwolf501.top/gtrnrbrcge.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xylfe.cn/gtfqtcdcsv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daria6918.cn/gtqsepddxu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhengqikj.top/gtqwklzvbh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenlongwang.top/gtembrprww.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.birdmap.top/gtihkbwemz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yangfankeji.com/gtpulnfgbu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.birdmap.top/gtetsckcfr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhixingplan.top/gtfstmpilo.html

[L05] 上传文件（multipart）
来源：http://hz.xziqi.cn/gtoexlctka.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.0kj1m.cn/gtjnqckcuc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.bjfxy.top/gtkscelfzt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gtryeaqveo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xziqi.cn/gtxvenbyak.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.redwolf501.top/gtayiafynl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hfpthk.cn/gttmcaerxa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.havefunace.top/gtkitoikuf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.kuanghao11.cn/gtzkhkbpam.html

[L06] 解析响应为 JSON
来源：http://hz.ehwqpu.com/gtbmqavswp.html

Py:   resp.json()
来源：http://hz.zhaomingkeji.xyz/gtvmirdygm.html

PHP:  json_decode($body, true);
来源：http://hz.pycfn.com/gtpnybpduf.html

JS:   await resp.json()
来源：http://hz.daria6918.cn/gteosbwdhx.html

TS:   await resp.json()
来源：http://hz.fzhhl.top/gtfbgilbia.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nwbrower.top/gtdjzzqzug.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cdnleiting.top/gtbiboptnl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhoulong.xyz/gtxxykpckp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jyoumei.cn/gtwnuajfay.html

[L07] 处理 HTTP 状态码
来源：http://hz.daria6918.cn/gtqjhqwhcp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhoulong.xyz/gtlkspiijd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj20258888.top/gtmklrjdoi.html

JS:   resp.ok;  resp.status
来源：http://hz.yvedp.cn/gteuivufbf.html

TS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtivajaecd.html

Java: resp.statusCode()
来源：http://hz.ywan-chungtsiang.top/gtnvkycddj.html

Go:   resp.StatusCode
来源：http://hz.tanke756.top/gtidwzzkff.html

Ruby: resp.code.to_i
来源：http://hz.birdmap.top/gtpafqynca.html

C#:   (int)resp.StatusCode
来源：http://hz.hnqzz.top/gtvyhkquhk.html

[L08] 并发请求多个地址
来源：http://hz.yueranfly.top/gtcviegdza.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.mhx1999.top/gtuokxlmwd.html

PHP:  curl_multi_init() 系列
来源：http://hz.dashuyun.cn/gtdgsbtjkw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gtlbkvjkbv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gtyzfhmram.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jianghu66.top/gtwpnjloxx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jlsjyb.cn/gttmtkvcpr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenjidiqi.icu/gtlgwajrhp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dashuyun.cn/gtoivrdrgw.html

================================================================================
来源：http://hz.ehwqpu.com/gtjlkxvija.html

M. 命令行 / 进程 / 环境
来源：http://hz.snrcjt.cn/gtiuqkfbmg.html

================================================================================
来源：http://hz.cheryme.top/gtukbgzxdf.html

[M01] 读取命令行参数
来源：http://hz.nanxuanxn.top/gtmegaxedb.html

Py:   sys.argv[1:]
来源：http://hz.ybcxt.top/gtveflbgsm.html

PHP:  $argv;  $argc;
来源：http://hz.zycfv.cn/gtahvgwxbh.html

JS:   process.argv.slice(2)
来源：http://hz.ybcxt.top/gteuersgab.html

TS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtqdvpfovy.html

Java: args 数组（main 方法参数）
来源：http://hz.cdnleiting.top/gtpecsgwwr.html

Go:   os.Args[1:]
来源：http://hz.daria6918.cn/gtancbnidj.html

Ruby: ARGV
来源：http://hz.meibo888.top/gtmkbjcpdq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ppjwa.cn/gtzflndzcy.html

[M02] 读取环境变量
来源：http://hz.kuanghao11.cn/gtbbqlhlvd.html

Py:   os.environ.get("HOME")
来源：http://hz.jinqigfzy.top/gthqicrajo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.52xcode.cn/gtuzciuvyw.html

JS:   process.env.HOME
来源：http://hz.birdmap.top/gtrnaeclyb.html

TS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtvuftlfvv.html

Java: System.getenv("HOME")
来源：http://hz.fzhhl.top/gtwgggkxmg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ehwqpu.com/gthhfsisru.html

Ruby: ENV["HOME"]
来源：http://hz.svipenyu.cn/gtzqjpdpls.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ehwqpu.com/gtsjwzodpc.html

[M03] 执行外部命令
来源：http://hz.wangdashe.top/gtxhccybvx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xylfe.cn/gtagieibjn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sysykeji.top/gtxtolqiki.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cashguo.top/gtorjaectm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cheryme.top/gtevalmrrb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.mhx1999.top/gtmjyljyax.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yangfankeji.com/gtgbymvfky.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cucudq.cn/gtmtauayhk.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jlsjyb.cn/gtibzxjhxu.html

[M04] 获取当前工作目录
来源：http://hz.0kj1m.cn/gtkyaqfjhf.html

Py:   os.getcwd()
来源：http://hz.jiagoushi.top/gtzhodqtho.html

PHP:  getcwd();
来源：http://hz.xylfe.cn/gtxelmbstl.html

JS:   process.cwd()
来源：http://hz.0kj1m.cn/gtvgamgluf.html

TS:   process.cwd()
来源：http://hz.jlsjyb.cn/gtdkdayfvk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tian-w.cn/gttgpqxdlk.html

Go:   os.Getwd()
来源：http://hz.xingfuxueyuan.xyz/gtbxnqvrjj.html

Ruby: Dir.pwd
来源：http://hz.cheryme.top/gtzbidmpej.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cashguo.top/gtgptgfjnb.html

[M05] 设置退出码
来源：http://hz.nanxuanxn.top/gtcaudhtwx.html

Py:   sys.exit(1)
来源：http://hz.jiagoushi.top/gtzqkxwccg.html

PHP:  exit(1);
来源：http://hz.zhixingplan.top/gtctydjxjw.html

JS:   process.exit(1)
来源：http://hz.cqqwz.cn/gtoglofcey.html

TS:   process.exit(1)
来源：http://hz.wangdashe.top/gtstvmtrco.html

Java: System.exit(1)
来源：http://hz.meibo888.top/gtinkhnxdv.html

Go:   os.Exit(1)
来源：http://hz.xylfe.cn/gtdwekokzo.html

Ruby: exit 1
来源：http://hz.sufxvd.cn/gtadidqcon.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xuanzx.com/gtifdjhkcw.html

[M06] 向标准错误输出
来源：http://hz.hfpthk.cn/gtaedbjsat.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gogol.net.cn/gtwjvdppor.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhengqikj.top/gtizhrtyqm.html

JS:   console.error("err")
来源：http://hz.cdnleiting.top/gtlyuampds.html

TS:   console.error("err")
来源：http://hz.cheryme.top/gtjopdsuka.html

Java: System.err.println("err")
来源：http://hz.yvedp.cn/gtqzvsvhuj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.redwolf501.top/gtaizaurra.html

Ruby: warn "err"
来源：http://hz.xingfuxueyuan.xyz/gtaczgjzvk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.quarkkingdee.top/gtnnfotygn.html

[M07] 判断是否为主入口
来源：http://hz.yj202588.top/gtmslyivpe.html

Py:   if __name__ == "__main__":
来源：http://hz.yj202588.top/gtesdxldqi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.pycfn.com/gtcbieopwx.html

JS:   require.main === module
来源：http://hz.gaohongyu789.top/gtkggvxdlz.html

TS:   require.main === module
来源：http://hz.daria6918.cn/gtaxvhfgcy.html

Java: public static void main(String[] args)
来源：http://hz.316326.xyz/gtyfcytcmk.html

Go:   func main()
来源：http://hz.guannengcc.top/gtnqrfztop.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yj20258.top/gtdwkkjcbz.html

C#:   static void Main(string[] args)
来源：http://hz.yanxiufei.cn/gtxdwnhtkh.html

[M08] 获取系统与运行时信息
来源：http://hz.meibo888.top/gtvtldgnjt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cucudq.cn/gtlfvertpq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yanxiufei.cn/gthxsbtpyi.html

JS:   process.platform;  process.version
来源：http://hz.yuxming.cn/gtegjmlusu.html

TS:   process.platform;  process.version
来源：http://hz.hnqzz.top/gthhmnjuth.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.quarkkingdee.top/gtzncuwdmu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gaohongyu789.top/gttuwhrbuy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gogol.net.cn/gtygepmrpg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.andypj.xyz/gtmneblcmd.html

================================================================================
来源：http://hz.dianchejie.cn/gtgyueisgg.html

N. 数据结构与算法
来源：http://hz.c1oappe.top/gtlpdtbrxd.html

================================================================================
来源：http://hz.ivvv.top/gtbfsdkkxl.html

[N01] 二分查找（有序数组）
来源：http://hz.jianghu66.top/gttjfaruqc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shzxlz.cn/gtjzrtazjs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.wangdashe.top/gtysplbkou.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.c1oappe.top/gtqsjdnykg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigfzy.top/gtwhijacry.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ydzc1.top/gtcbwqewdy.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinqigfzy.top/gtumztjqem.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nanxinkj.top/gtykfinscq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.bjfxy.top/gtekytklrs.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.mhx1999.top/gtowktaaax.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.kuanghao11.cn/gtfrhnbkoi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yuxming.cn/gtvpaqmzuq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgufenzy.top/gtympjkjgr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ppjwa.cn/gtwmrllmcn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhaomingkeji.xyz/gtgixosxcy.html

Go:   slices.Sort(arr)
来源：http://hz.cheryme.top/gtellbclvi.html


<!-- 参考信息 -->