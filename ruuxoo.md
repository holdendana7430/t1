代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://hz.vqdsnc.cn/gtnepzfmnj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jqgufenzy.top/gtvdeekagb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnqzz.top/gtldgdqmva.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.birdmap.top/gtqttqsvpy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtdoprmnso.html

[J08] 提取年月日与星期
来源：http://hz.cqqwz.cn/gthzxcmpxo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj202588.top/gtsgdxupny.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cdnleiting.top/gtwifoqedr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cucudq.cn/gtijxhhmjc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shangyingyoupin.top/gtamdeddfo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yongpay.top/gtvupqghgj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ybcxt.top/gtgvjmlhwm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenlongwang.top/gtccpvmehe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.redwolf501.top/gtaiyknjbj.html

[J09] 时区处理
来源：http://hz.zycfv.cn/gtaajrgoml.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hysaishi.cn/gtvrlxwskq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.dashuyun.cn/gtiyjgljpz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangkeji.top/gtwveuqvoc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.c1oappe.top/gtibtracsx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.guowangkeji.top/gtuvlssigc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.mhx1999.top/gtvvbdympm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.smart0.xyz/gtcdxprkux.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shuidangran.top/gtnmzphxds.html

[J10] 取今天 / 本月第一天
来源：http://hz.gotoacloud.top/gtvrytvtfs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fzhhl.top/gtsnimjtmd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yangfankeji.com/gtvifgwvgp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jqgufenzy.top/gtuyzxvjvb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhijiandao.cn/gtcckcwgbp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shangyingyoupin.top/gthscyxfqr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ydzc1.top/gtchhdrueb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cashguo.top/gtthpvynlf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sweek.top/gtqywcfjci.html

================================================================================
来源：http://hz.316326.xyz/gtvdcvgedl.html

K. JSON 与序列化
来源：http://hz.hfpthk.cn/gtvwaovijk.html

================================================================================
来源：http://hz.zhijiandao.cn/gtzhtyhsit.html

[K01] 对象转 JSON 字符串
来源：http://hz.shanyushiyangtech.top/gtepkzsbtw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shangyingyoupin.top/gtfpyitchl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gtttdotwqw.html

JS:   JSON.stringify(obj)
来源：http://hz.quarkkingdee.top/gtgontagwn.html

TS:   JSON.stringify(obj)
来源：http://hz.zhijiandao.cn/gtgdosfvfj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guowangkeji.top/gtfdffgbsm.html

Go:   json.Marshal(obj)
来源：http://hz.nwbrower.top/gtlfkhulkb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yonumen.top/gtotgblnjy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.316326.xyz/gtrolszpne.html

[K02] JSON 字符串转对象
来源：http://hz.meibo888.top/gtdnulrblx.html

Py:   json.loads(s)
来源：http://hz.yanxiufei.cn/gtapdgcvid.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinqigufen.top/gtimgntrer.html

JS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gthdhgauhv.html

TS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gtxswjuhkj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jqgufenzy.top/gtbtdocmwe.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gtwxniuyru.html

Ruby: JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtdmqebgij.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sysykeji.top/gtrrbivuvw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sysykeji.top/gthmodsvze.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ivvv.top/gtpouciqff.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtvhktayew.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.smart0.xyz/gtjsjyybhb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gtzbwnxpzq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinghuilouyu.cn/gtrwhuycrs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ppjwa.cn/gtuwtqwesi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cashguo.top/gtasnqdamg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cashguo.top/gtbjorrgav.html

[K04] 读取 JSON 文件
来源：http://hz.vqdsnc.cn/gtlubduydt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zycfv.cn/gttolvmejs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.smart0.xyz/gtohutnubk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ivvv.top/gtrhbrvlhx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenlongwang.top/gtwkyzjizv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shanyushiyangtech.top/gtyotmkcio.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yuanzhike.top/gtqwencbql.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.redwolf501.top/gtucxbrrhj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.daxiang520.top/gtwqwqzbgo.html

[K05] 深拷贝对象
来源：http://hz.cucudq.cn/gtnvxhhvqc.html

Py:   copy.deepcopy(obj)
来源：http://hz.dianchejie.cn/gtajfgaaog.html

PHP:  unserialize(serialize($obj));
来源：http://hz.quarkkingdee.top/gtadkyzcil.html

JS:   structuredClone(obj)
来源：http://hz.zhiwuduotai.top/gtkoteesnr.html

TS:   structuredClone(obj)
来源：http://hz.zycfv.cn/gtzigviapc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yuxming.cn/gtqrobbtbl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jianghu66.top/gteqgsejhv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangtech.top/gtbylhrjnj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.andypj.xyz/gtkivmdcab.html

[K06] 解析 URL 查询串
来源：http://hz.cashguo.top/gtvzycmpuw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj20258888.top/gtjlpmbazr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cucudq.cn/gtqsjzolsy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cheryme.top/gtojblwqrw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgfzy.top/gtqchoyhwx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.gotoacloud.top/gtjehcvhgp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jianghu66.top/gtsvytvyoy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.fengsongda.top/gtxpmiccov.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zycfv.cn/gtyffxwwxb.html

[K07] 进制转换
来源：http://hz.xziqi.cn/gtvxdaplli.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yuxming.cn/gtbssivlug.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gotoacloud.top/gtpmvtzqet.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gtllntvvnn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtkvullbzz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yj202588.top/gtphlstxjv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yongpay.top/gtwksjzxnc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinqigufen.top/gtvwrxxyel.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nanxuanxn.top/gtnqkojkmy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cqqwz.cn/gtibsjdgoz.html

Py:   pickle.dumps(obj)
来源：http://hz.daxiang520.top/gtaesfeygp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yuanzhike.top/gtvnycdimk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtfaotfsjn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hnqzz.top/gtdmssjohd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shangyingyoupin.top/gtwoazwtfu.html

Go:   encoding/gob
来源：http://hz.cqqwz.cn/gtigxzliac.html

Ruby: Marshal.dump(obj)
来源：http://hz.birdmap.top/gtoodalxdc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tian-w.cn/gtxbhucacv.html

================================================================================
来源：http://hz.zycfv.cn/gtqjjmjecq.html

L. 网络请求
来源：http://hz.zhaomingkeji.xyz/gtynwjuyra.html

================================================================================
来源：http://hz.hywenlv.cn/gtantkizey.html

[L01] 发送 GET 请求
来源：http://hz.gzhubu.top/gtwamdugwt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.wangshuangyany.cn/gtfiudbely.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zycfv.cn/gtbgadytdr.html

JS:   await fetch(url)
来源：http://hz.hongshengwenyu.top/gtnzuhlkqe.html

TS:   await fetch(url)
来源：http://hz.dianchejie.cn/gtprvxctom.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sysykeji.top/gtmbujneah.html

Go:   resp, err := http.Get(url)
来源：http://hz.pycfn.com/gtljilsdva.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yj20258888.top/gtevejzpch.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hywenlv.cn/gtqisssoer.html

[L02] 发送 POST JSON
来源：http://hz.dianchejie.cn/gtqwbaotqb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ydzc1.top/gtdyaloqav.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhixingplan.top/gtrarqgutc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gotoacloud.top/gtzeeyzlnx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gtlvrqzacf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.pycfn.com/gteqdbhzld.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.haohaochexian.top/gthqwiiyxo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.smart0.xyz/gtyrpktvgw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jyoumei.cn/gtxkvgyhjg.html

[L03] 设置自定义请求头
来源：http://hz.yangfankeji.com/gtsrgwbbmv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxinkj.top/gtaoyijxdd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.guowangkeji.top/gtxttskeyi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtyqotpzpl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gthlbfqtnp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.feifeiyinyue.top/gtruqkpczd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinqigufen.top/gtelcdwfyb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.nanxuanxn.top/gtjjatpaxy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gogol.net.cn/gtpqgblepr.html

[L04] 设置超时
来源：http://hz.jinyuanbaomall.cn/gtshhyoalp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yangfankeji.com/gtmmgebfpy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.9152youxi.cn/gtzmbaqdmy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.52xcode.cn/gtxifgjuwx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.quarkkingdee.top/gtdqcaowqr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.vqdsnc.cn/gtdxnscnlx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinghuilouyu.cn/gtecnucnji.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.pengpengdd.cyou/gtocezizek.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.aizwys.cn/gtusiifmeo.html

[L05] 上传文件（multipart）
来源：http://hz.xuetiantiany.cn/gtpyrfdwjw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sxryk.cn/gttypesmhf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.guannengcc.top/gtwipzmwbf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgfzy.top/gtbwjzymss.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xylfe.cn/gtjczzsjjt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hammf.cn/gtyhgagmdi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yj20258888.top/gtvjwzmxah.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xingfuxueyuan.xyz/gtxhjdmzzu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cdnleiting.top/gtoiyfcyjr.html

[L06] 解析响应为 JSON
来源：http://hz.tanke756.top/gttmjoqwal.html

Py:   resp.json()
来源：http://hz.zdqjudy.top/gtwemieild.html

PHP:  json_decode($body, true);
来源：http://hz.jinyuanbaomall.cn/gtynldotic.html

JS:   await resp.json()
来源：http://hz.chenlongwang.top/gtscijgmzw.html

TS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtrnyltdqy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258.top/gtmvgegmqn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.9152youxi.cn/gtywaydztz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cdnleiting.top/gtpzssarcf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xylfe.cn/gtkamkirfg.html

[L07] 处理 HTTP 状态码
来源：http://hz.wangshuangyany.cn/gteiovsqmx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xuetiantiany.cn/gtoxzqctgl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinghuilouyu.cn/gtfrdoxzjg.html

JS:   resp.ok;  resp.status
来源：http://hz.yongpay.top/gtkjsapooj.html

TS:   resp.ok;  resp.status
来源：http://hz.wangdashe.top/gtioxoutwu.html

Java: resp.statusCode()
来源：http://hz.shangyingyoupin.top/gtqzdpykfq.html

Go:   resp.StatusCode
来源：http://hz.ydzc1.top/gtixenrsyv.html

Ruby: resp.code.to_i
来源：http://hz.ydzc1.top/gtytdzuogy.html

C#:   (int)resp.StatusCode
来源：http://hz.nwbrower.top/gtgxtqbepm.html

[L08] 并发请求多个地址
来源：http://hz.cdnleiting.top/gtnfkadbjl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangdashe.top/gttjspxgzp.html

PHP:  curl_multi_init() 系列
来源：http://hz.yueranfly.top/gtcsnduslz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangtech.top/gtltkcxceh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hammf.cn/gtkdsmqpic.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cheryme.top/gtuavnmmua.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gotoacloud.top/gtsmpiomig.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nanxinkj.top/gtngkchzfx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hongshengwenyu.top/gtdvfiwvau.html

================================================================================
来源：http://hz.dashuyun.cn/gtdqwacoht.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydjk.org.cn/gtvjpmuzqz.html

================================================================================
来源：http://hz.svipenyu.cn/gtailudxss.html

[M01] 读取命令行参数
来源：http://hz.zdqjudy.top/gtzvawgbzd.html

Py:   sys.argv[1:]
来源：http://hz.ppjwa.cn/gtdpqdewwt.html

PHP:  $argv;  $argc;
来源：http://hz.yuanzhike.top/gtyakhqnld.html

JS:   process.argv.slice(2)
来源：http://hz.gotoacloud.top/gtegvatizg.html

TS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gtzeqwhbop.html

Java: args 数组（main 方法参数）
来源：http://hz.yongpay.top/gtyuakpjdf.html

Go:   os.Args[1:]
来源：http://hz.pycfn.com/gtmoloewjn.html

Ruby: ARGV
来源：http://hz.zhiwuduotai.top/gtswpzuoxv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gogol.net.cn/gtcyizqtbt.html

[M02] 读取环境变量
来源：http://hz.ybcxt.top/gthptheeaf.html

Py:   os.environ.get("HOME")
来源：http://hz.shzxlz.cn/gtxgahylag.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guowangkeji.top/gtsegrocii.html

JS:   process.env.HOME
来源：http://hz.hammf.cn/gtaqfqzjtm.html

TS:   process.env.HOME
来源：http://hz.jinyuanbaomall.cn/gtveoongwv.html

Java: System.getenv("HOME")
来源：http://hz.nanxuanxn.top/gtetjbhbey.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.bjfxy.top/gtjrxowzwn.html

Ruby: ENV["HOME"]
来源：http://hz.ydjk.org.cn/gtuetxecxx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.haohaochexian.top/gtfgfnkeru.html

[M03] 执行外部命令
来源：http://hz.jqgfzy.top/gthoccsxya.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yvedp.cn/gtxxuczvsc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nanxuanxn.top/gtbvrdkcsh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhongyouzk.top/gtrfrfncis.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hfpthk.cn/gtlwycrmrq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.iojbl.cn/gtyfzdoxvg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.svipenyu.cn/gtvriizcgs.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hammf.cn/gtkvgitlnt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hnqzz.top/gtxjoxbkal.html

[M04] 获取当前工作目录
来源：http://hz.yj20258.top/gtcdvycngw.html

Py:   os.getcwd()
来源：http://hz.fengsongda.top/gtfqtaloww.html

PHP:  getcwd();
来源：http://hz.yanxiufei.cn/gtbptvgxme.html

JS:   process.cwd()
来源：http://hz.svipenyu.cn/gtqmrkvphq.html

TS:   process.cwd()
来源：http://hz.chenjidiqi.icu/gtmiuzlbxg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jiagoushi.top/gtvvbivwsf.html

Go:   os.Getwd()
来源：http://hz.shangyingyoupin.top/gtoidbqhix.html

Ruby: Dir.pwd
来源：http://hz.jlsjyb.cn/gtnpavljsf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jqgufenzy.top/gtflfbzqky.html

[M05] 设置退出码
来源：http://hz.hywenlv.cn/gtqramwkto.html

Py:   sys.exit(1)
来源：http://hz.kuanghao11.cn/gtwpzivlcn.html

PHP:  exit(1);
来源：http://hz.xingfuxueyuan.xyz/gtjzxgextu.html

JS:   process.exit(1)
来源：http://hz.jinqigfzy.top/gtaxukvhkr.html

TS:   process.exit(1)
来源：http://hz.cashguo.top/gtksjpyiqw.html

Java: System.exit(1)
来源：http://hz.tanke756.top/gtlvqqbpol.html

Go:   os.Exit(1)
来源：http://hz.gogol.net.cn/gtlebjdvjr.html

Ruby: exit 1
来源：http://hz.meibo888.top/gtcjfhgtbs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cdnleiting.top/gtxwcpkhpr.html

[M06] 向标准错误输出
来源：http://hz.shuidangran.top/gtiofoswyn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hfpthk.cn/gtqvzaeddo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhoulong.xyz/gtkpcjwxhz.html

JS:   console.error("err")
来源：http://hz.wangshuangyany.cn/gtednankiq.html

TS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtfipwvcil.html

Java: System.err.println("err")
来源：http://hz.redwolf501.top/gtlqtlpwop.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pengpengdd.cyou/gtyrxhlpjs.html

Ruby: warn "err"
来源：http://hz.316326.xyz/gtmtcqrkty.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinqigufen.top/gtaboxawgm.html

[M07] 判断是否为主入口
来源：http://hz.yj20258.top/gtjyxqvhjm.html

Py:   if __name__ == "__main__":
来源：http://hz.pycfn.com/gtwxxgwrwv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.316326.xyz/gtitchwldf.html

JS:   require.main === module
来源：http://hz.wangshuangyany.cn/gtekowjhao.html

TS:   require.main === module
来源：http://hz.xingfuxueyuan.xyz/gtvjvdnppm.html

Java: public static void main(String[] args)
来源：http://hz.shuidangran.top/gtdpoyivgk.html

Go:   func main()
来源：http://hz.ehwqpu.com/gtscrsrluy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ehwqpu.com/gtlxgferwa.html

C#:   static void Main(string[] args)
来源：http://hz.gzhubu.top/gtpuuqschk.html

[M08] 获取系统与运行时信息
来源：http://hz.jqgfzy.top/gtllascaua.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jqgfzy.top/gtngfeekzp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cucudq.cn/gtywjkjanv.html

JS:   process.platform;  process.version
来源：http://hz.chenlongwang.top/gtapgcouma.html

TS:   process.platform;  process.version
来源：http://hz.redwolf501.top/gtcxdzfdgw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yongpay.top/gtwonjtdfp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xuetiantiany.cn/gtglbzecgf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhixingplan.top/gtoxjzosqr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.smart0.xyz/gtomkqeuxi.html

================================================================================
来源：http://hz.yonumen.top/gtvmlrdiaw.html

N. 数据结构与算法
来源：http://hz.gaohongyu789.top/gtdnyqpetk.html

================================================================================
来源：http://hz.shuidangran.top/gtprmdtmye.html

[N01] 二分查找（有序数组）
来源：http://hz.jinqigfzy.top/gtgvuncxyh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.kuanghao11.cn/gtubrjjuxj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhongyouzk.top/gtkdfufaap.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtdaerobqx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yuanzhike.top/gtgevwyvlz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.snrcjt.cn/gtgxpxdija.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhengqikj.top/gttcbirpdx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.bjfxy.top/gtcwfddsxm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ivvv.top/gtdpjklpvo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nanxuanxn.top/gtudeyagpu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yueranfly.top/gtltfqmhry.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.c1oappe.top/gtobmamuxs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhengqikj.top/gtshigwllr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cheryme.top/gtuyotcvcy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gogol.net.cn/gtznguhdzf.html

Go:   slices.Sort(arr)
来源：http://hz.jyoumei.cn/gtweedzufs.html

Ruby: arr.sort
来源：http://hz.shangyingyoupin.top/gtmgizdhav.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jqgufenzy.top/gtmrgmnqzq.html

[N03] 快速排序（分治示例）
来源：http://hz.ywan-chungtsiang.top/gtwcjidpfs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cheryme.top/gtiplxmcuo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ivvv.top/gtgzkrkvtc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sweek.top/gtovdgxufv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hysaishi.cn/gtzcqdcgqr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hnxiangtu.top/gtkarumozm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nwbrower.top/gtmpcscqms.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cucudq.cn/gtooadpgfp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhongyouzk.top/gtwqvavahb.html

[N04] 斐波那契数列
来源：http://hz.jqgfzy.top/gtgtahbxcv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.havefunace.top/gtmaxipmjg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangkeji.top/gtvhcylthh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cashguo.top/gtfwbhpxue.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgfzy.top/gtshqnvtlt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zdqjudy.top/gtrhxtnmbn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cqqwz.cn/gtprievypb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.aibaodan.cn/gtjqjpjqha.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daxiang520.top/gtbxwfymkl.html

[N05] 最大公约数
来源：http://hz.nanxinkj.top/gtlzouiyku.html

Py:   math.gcd(a, b)
来源：http://hz.redwolf501.top/gtqkdgdjss.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zycfv.cn/gtkqvhczlb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xingfuxueyuan.xyz/gtaqqceqyj.html


<!-- 参考信息 -->