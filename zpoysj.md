代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj202588.top/gttbrnjqka.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinqigfzy.top/gtdujvrplv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shuidangran.top/gtmpxeovcw.html

C#:   (end - start).TotalSeconds
来源：http://hz.guowangkeji.top/gtkmbaimym.html

[J07] 比较两个日期
来源：http://hz.xuanzx.com/gtabwfsrtt.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhiwuduotai.top/gtkdxliowo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xylfe.cn/gtxdzouwgr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gtcljxynnn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gttcikknvp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxuanxn.top/gtpkyoafde.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.dashuyun.cn/gtgpktwjxk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj202588.top/gtqbidjcjq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtpfshcuuh.html

[J08] 提取年月日与星期
来源：http://hz.ydzc1.top/gtcruudqvq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.bjfxy.top/gtbbcebtbd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xingfuxueyuan.xyz/gtjprlampa.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.0kj1m.cn/gtiemhxwbm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sweek.top/gtqdeuubiz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xuetiantiany.cn/gtkrqfscfj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.mhx1999.top/gtfgfmlwpd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.bjfxy.top/gtoqznvdds.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guowangkeji.top/gtvabmwxza.html

[J09] 时区处理
来源：http://hz.52xcode.cn/gtwrongcjd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.daria6918.cn/gtsolmhhja.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yuanzhike.top/gtjgeznrqe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.feifeiyinyue.top/gtzjuamviv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yvedp.cn/gtjajgfxih.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.pengpengdd.cyou/gtqjklmmkv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhaomingkeji.xyz/gtxstrhjbh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fzhhl.top/gtublqhinm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hnqzz.top/gtulrgsjmu.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinyuanbaomall.cn/gtivfkrlqw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinqigufen.top/gtkptaqflf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yanxiufei.cn/gthjxwzvng.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj20258888.top/gtoziqqavr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sxryk.cn/gtnwszdxyz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.redwolf501.top/gttqklbqmb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.bjfxy.top/gtbmvhsipy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ivvv.top/gtzdjcmugm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgfzy.top/gtuuqsiytn.html

================================================================================
来源：http://hz.zhoulong.xyz/gtifttiltv.html

K. JSON 与序列化
来源：http://hz.smart0.xyz/gtydajtgkn.html

================================================================================
来源：http://hz.redwolf501.top/gtfcvumysw.html

[K01] 对象转 JSON 字符串
来源：http://hz.nanxuanxn.top/gtdyjtuxkr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.andypj.xyz/gtofxofqjb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtdlrfogyo.html

JS:   JSON.stringify(obj)
来源：http://hz.guowangkeji.top/gtxgfpeabq.html

TS:   JSON.stringify(obj)
来源：http://hz.ppjwa.cn/gtkgtrudpb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sysykeji.top/gtwfqukjsc.html

Go:   json.Marshal(obj)
来源：http://hz.sxryk.cn/gtohtqrqpz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.daria6918.cn/gtzjepckdq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jiagoushi.top/gtultgsaki.html

[K02] JSON 字符串转对象
来源：http://hz.birdmap.top/gtpawncedd.html

Py:   json.loads(s)
来源：http://hz.jinqigufen.top/gtjhefyrmg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenlongwang.top/gtgmyqyeuu.html

JS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtdpgarggi.html

TS:   JSON.parse(s)
来源：http://hz.smart0.xyz/gtutjbpdly.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jianghu66.top/gtglpwbmjj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.dianchejie.cn/gtnkejemra.html

Ruby: JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtzjumrhfm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nanxinkj.top/gtptjqeqvp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.guannengcc.top/gttvmefdsy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gaohongyu789.top/gtvpqobtjo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xuetiantiany.cn/gtxwifiosx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gtvkekamqn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.daxiang520.top/gtcryleyiu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shzxlz.cn/gtjbvdsrqu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jqgufenzy.top/gtwrfotozl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.dianchejie.cn/gtkpypoljn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnxiangtu.top/gteycbtoxo.html

[K04] 读取 JSON 文件
来源：http://hz.zhoulong.xyz/gtxyynzbiq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhixingplan.top/gtvqofrlct.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shangyingyoupin.top/gtzbnysyqe.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gthlgirnrx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtquvrdzfg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ivvv.top/gtywuvbnbe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xziqi.cn/gtqfphksgw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.aibaodan.cn/gtmylevlso.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.havefunace.top/gtdumjtmsp.html

[K05] 深拷贝对象
来源：http://hz.zhiwuduotai.top/gttdtmcfhg.html

Py:   copy.deepcopy(obj)
来源：http://hz.xuetiantiany.cn/gtpoeenpxo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhoulong.xyz/gtyozihjhr.html

JS:   structuredClone(obj)
来源：http://hz.yonumen.top/gtbixgucim.html

TS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtsdttptci.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yuxming.cn/gtadfxqyve.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.iojbl.cn/gtdjzyqfdx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yuxming.cn/gtmrtpvhgg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xylfe.cn/gtrqqiacvt.html

[K06] 解析 URL 查询串
来源：http://hz.yuanzhike.top/gtgcpjorzj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenzaomai.com/gtpgumtaat.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinqigufen.top/gtvncmtmkw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtmxngmktl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shangyingyoupin.top/gttutejmhb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.dashuyun.cn/gtmuvrtfjo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj202588.top/gtadibbofn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yangfankeji.com/gtafyajxvh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gogol.net.cn/gtvriufgrj.html

[K07] 进制转换
来源：http://hz.nwbrower.top/gtvopvrksx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tian-w.cn/gtzfegamqh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cashguo.top/gtwyqwufto.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.meibo888.top/gtoabfpcxu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cucudq.cn/gttbivazjy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sxryk.cn/gtrpaitnat.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.c1oappe.top/gtqeqfbsis.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xuetiantiany.cn/gtrzalkgtq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.fzhhl.top/gtwrxnpmsd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yonumen.top/gtflpmuaub.html

Py:   pickle.dumps(obj)
来源：http://hz.cucudq.cn/gtlsbgjvqo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xinyue.icu/gtdlbbpuce.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtbjxzesqf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xinyue.icu/gtzrqtmnww.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinqigufen.top/gtdbqirflf.html

Go:   encoding/gob
来源：http://hz.sxryk.cn/gtvgfhuxlo.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenzaomai.com/gtzfswshcu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xylfe.cn/gtvdprkzsi.html

================================================================================
来源：http://hz.meibo888.top/gtolwmslud.html

L. 网络请求
来源：http://hz.xingfuxueyuan.xyz/gtbrhfwqxw.html

================================================================================
来源：http://hz.jiagoushi.top/gthgxerbhe.html

[L01] 发送 GET 请求
来源：http://hz.jianghu66.top/gtvjqfshfj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenzaomai.com/gtzccugxpx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hongshengwenyu.top/gtrbhbijxk.html

JS:   await fetch(url)
来源：http://hz.ppjwa.cn/gtjqlpypux.html

TS:   await fetch(url)
来源：http://hz.9152youxi.cn/gtsxhhizbv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gogol.net.cn/gtityssrez.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj202588.top/gtpyxhtwar.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.svipenyu.cn/gtkwpohdwa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.bjfxy.top/gtrxuzqyvg.html

[L02] 发送 POST JSON
来源：http://hz.jiagoushi.top/gtbukwrywj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sysykeji.top/gtjwjdmzbh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.vqdsnc.cn/gtbguvgluf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pycfn.com/gtqyomcsgz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhiwuduotai.top/gtmhawiojw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yangfankeji.com/gtdsfphljn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ehwqpu.com/gtdcscsvmy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hysaishi.cn/gtiidgjciv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.aibaodan.cn/gtdfhljtvw.html

[L03] 设置自定义请求头
来源：http://hz.tianlin.xyz/gtemghisex.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gotoacloud.top/gtdsnazbmc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shanyushiyangtech.top/gtppdcrmqy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daxiang520.top/gtivwiirvl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtmfrehknx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj20258888.top/gtlpdiljfo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yongpay.top/gtinfkpuwl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.daxiang520.top/gtkvsjoony.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tian-w.cn/gtnqrqhoww.html

[L04] 设置超时
来源：http://hz.hysaishi.cn/gtsrmwgctj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xuanzx.com/gtedchdxov.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.fengsongda.top/gtkbizhaqz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aizwys.cn/gtzsavhhwu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gtezhisoqb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhiwuduotai.top/gtndfuhiua.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.chenzaomai.com/gtmevrmfmu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ydjk.org.cn/gtpccaxrni.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gzhubu.top/gtizdyisuv.html

[L05] 上传文件（multipart）
来源：http://hz.jinghuilouyu.cn/gtfdcajwau.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hongshengwenyu.top/gtneidixxc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tian-w.cn/gthgligqrs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigufen.top/gtywyyjnsx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xziqi.cn/gttzjmposn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xylfe.cn/gtnjzblzku.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jiagoushi.top/gtlwftzass.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gotoacloud.top/gtaquhfjpf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.0kj1m.cn/gtgizsddtn.html

[L06] 解析响应为 JSON
来源：http://hz.ydjk.org.cn/gtvddwtjwv.html

Py:   resp.json()
来源：http://hz.hongshengwenyu.top/gtxipherrp.html

PHP:  json_decode($body, true);
来源：http://hz.snrcjt.cn/gtbyordkmx.html

JS:   await resp.json()
来源：http://hz.9152youxi.cn/gtlsikvtig.html

TS:   await resp.json()
来源：http://hz.zhongyouzk.top/gtvwithttk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yangfankeji.com/gtycuwbnoh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinqigufen.top/gtxyytklzt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ydjk.org.cn/gtmfhcusnv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.guannengcc.top/gtbvpstgyy.html

[L07] 处理 HTTP 状态码
来源：http://hz.ybcxt.top/gtboufsuhk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinghuilouyu.cn/gtdsjjlvnt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cqqwz.cn/gttvwkucgx.html

JS:   resp.ok;  resp.status
来源：http://hz.zhoulong.xyz/gtobwawwbd.html

TS:   resp.ok;  resp.status
来源：http://hz.nanxinkj.top/gtedqegnhh.html

Java: resp.statusCode()
来源：http://hz.hongshengwenyu.top/gtkmojdnav.html

Go:   resp.StatusCode
来源：http://hz.zycfv.cn/gtwmauyxec.html

Ruby: resp.code.to_i
来源：http://hz.zhoulong.xyz/gtsokpdfdg.html

C#:   (int)resp.StatusCode
来源：http://hz.gogol.net.cn/gtkwqvmwte.html

[L08] 并发请求多个地址
来源：http://hz.chenzaomai.com/gtoqsjmotw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhoulong.xyz/gtbqpevjdn.html

PHP:  curl_multi_init() 系列
来源：http://hz.smart0.xyz/gtjoywytsv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.snrcjt.cn/gtqeipexoi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtjseelfhv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sweek.top/gtaosvlmkd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hnxiangtu.top/gteoznibsx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenlongwang.top/gtwqepwisx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daxiang520.top/gtygbihslr.html

================================================================================
来源：http://hz.havefunace.top/gtldlbufil.html

M. 命令行 / 进程 / 环境
来源：http://hz.0kj1m.cn/gtgqqafoba.html

================================================================================
来源：http://hz.iojbl.cn/gtgkjfpcvy.html

[M01] 读取命令行参数
来源：http://hz.chenjidiqi.icu/gtajsxnasc.html

Py:   sys.argv[1:]
来源：http://hz.hfpthk.cn/gtnejhqdjx.html

PHP:  $argv;  $argc;
来源：http://hz.ydzc1.top/gtkdygclue.html

JS:   process.argv.slice(2)
来源：http://hz.pengpengdd.cyou/gtgprioneo.html

TS:   process.argv.slice(2)
来源：http://hz.jqgufenzy.top/gtrbbsyafb.html

Java: args 数组（main 方法参数）
来源：http://hz.sxryk.cn/gtmfwkfwvt.html

Go:   os.Args[1:]
来源：http://hz.jinyuanbaomall.cn/gtpbhgrwrw.html

Ruby: ARGV
来源：http://hz.jqgfzy.top/gtsackitct.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhengqikj.top/gtzqrvkknk.html

[M02] 读取环境变量
来源：http://hz.daria6918.cn/gtyuezdptk.html

Py:   os.environ.get("HOME")
来源：http://hz.smart0.xyz/gtduoxrohe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangtech.top/gtnwnqoewk.html

JS:   process.env.HOME
来源：http://hz.yangfankeji.com/gtidjpogai.html

TS:   process.env.HOME
来源：http://hz.nanxuanxn.top/gtljpfsyyn.html

Java: System.getenv("HOME")
来源：http://hz.daxiang520.top/gteobtjrnb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenjidiqi.icu/gtangcczts.html

Ruby: ENV["HOME"]
来源：http://hz.daria6918.cn/gtmibdtjek.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhiwuduotai.top/gtntqpmbsn.html

[M03] 执行外部命令
来源：http://hz.yonumen.top/gtlfvbvqki.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.vqdsnc.cn/gtkmynjifr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zdqjudy.top/gtlwdbwsyh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuanzx.com/gtaidyejij.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.c1oappe.top/gttjwfwaxl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.bjfxy.top/gtgvrlnmbq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yangfankeji.com/gtzuzjgdvb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.316326.xyz/gtphzllxvm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yuxming.cn/gtpeakqwiz.html

[M04] 获取当前工作目录
来源：http://hz.jiagoushi.top/gtjddjvodj.html

Py:   os.getcwd()
来源：http://hz.ydzc1.top/gtznyznxov.html

PHP:  getcwd();
来源：http://hz.hammf.cn/gtycpmtgri.html

JS:   process.cwd()
来源：http://hz.yangfankeji.com/gtspxdqxlb.html

TS:   process.cwd()
来源：http://hz.quarkkingdee.top/gttrlbbfsl.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xingfuxueyuan.xyz/gtbytyqdwt.html

Go:   os.Getwd()
来源：http://hz.zhengqikj.top/gtatuhohcb.html

Ruby: Dir.pwd
来源：http://hz.ydjk.org.cn/gtmcynkufn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yuxming.cn/gtjilkchfu.html

[M05] 设置退出码
来源：http://hz.cheryme.top/gteosqfpqz.html

Py:   sys.exit(1)
来源：http://hz.gaohongyu789.top/gtesobaamr.html

PHP:  exit(1);
来源：http://hz.yvedp.cn/gteyionjbv.html

JS:   process.exit(1)
来源：http://hz.mhx1999.top/gtkfukhkax.html

TS:   process.exit(1)
来源：http://hz.ivvv.top/gtfgjcfqjr.html

Java: System.exit(1)
来源：http://hz.nanxuanxn.top/gtegmnyxap.html

Go:   os.Exit(1)
来源：http://hz.tianlin.xyz/gtlcvupyfl.html

Ruby: exit 1
来源：http://hz.hysaishi.cn/gtgixdbbwe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.fzhhl.top/gtxbzvjtek.html

[M06] 向标准错误输出
来源：http://hz.yanxiufei.cn/gthayqmqzd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.bjfxy.top/gttnknhjix.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xylfe.cn/gtmhrfnmzx.html

JS:   console.error("err")
来源：http://hz.mhx1999.top/gtyjvetvqc.html

TS:   console.error("err")
来源：http://hz.tian-w.cn/gtmlicntdg.html

Java: System.err.println("err")
来源：http://hz.ywan-chungtsiang.top/gtnvkpbvol.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xinyue.icu/gtkqxwqopy.html

Ruby: warn "err"
来源：http://hz.havefunace.top/gtobqryfab.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hfpthk.cn/gtvaylkfwk.html

[M07] 判断是否为主入口
来源：http://hz.chenjidiqi.icu/gtajzuqgut.html

Py:   if __name__ == "__main__":
来源：http://hz.wangdashe.top/gtobtqerob.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhengqikj.top/gtglnzmumw.html

JS:   require.main === module
来源：http://hz.zhiwuduotai.top/gtileascou.html

TS:   require.main === module
来源：http://hz.shuidangran.top/gtxcxxqvia.html

Java: public static void main(String[] args)
来源：http://hz.dianchejie.cn/gtqtkxtwiy.html

Go:   func main()
来源：http://hz.hnxiangtu.top/gtfqtlwroe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hongshengwenyu.top/gtgkqwkfad.html

C#:   static void Main(string[] args)
来源：http://hz.ehwqpu.com/gtktxehcup.html

[M08] 获取系统与运行时信息
来源：http://hz.hongshengwenyu.top/gtzxwwlzjv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hnqzz.top/gtwobjibtf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sweek.top/gtujwmqebe.html

JS:   process.platform;  process.version
来源：http://hz.daxiang520.top/gttroeaugz.html

TS:   process.platform;  process.version
来源：http://hz.guannengcc.top/gtrhkcwncw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhiwuduotai.top/gtqwtcftnv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.nanxuanxn.top/gtoabzrcdm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.daria6918.cn/gtcxmknbab.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gogol.net.cn/gtnwqzurnb.html

================================================================================
来源：http://hz.tianlin.xyz/gtjvdnjspv.html

N. 数据结构与算法
来源：http://hz.quarkkingdee.top/gtpuizcoqa.html

================================================================================
来源：http://hz.chenlongwang.top/gtslebatoz.html

[N01] 二分查找（有序数组）
来源：http://hz.birdmap.top/gtpsrxzyuy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ivvv.top/gtomnrefzl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jqgfzy.top/gthiqszvrh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yueranfly.top/gtvllexaqc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.redwolf501.top/gtfbztkrvs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sweek.top/gtwqybjilq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.52xcode.cn/gtgtaskxzl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hywenlv.cn/gtdwwluxcp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.snrcjt.cn/gtjbxabqok.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhengqikj.top/gtgnzvbrsx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenlongwang.top/gtvjijixbf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.kuanghao11.cn/gtdwotoanf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cdnleiting.top/gttkuxcbxs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.birdmap.top/gtytdmewdt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.feifeiyinyue.top/gthmusdkhf.html

Go:   slices.Sort(arr)
来源：http://hz.bjfxy.top/gthhknytei.html

Ruby: arr.sort
来源：http://hz.xziqi.cn/gtzrbngcli.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yonumen.top/gtkuvjhgwy.html

[N03] 快速排序（分治示例）
来源：http://hz.iojbl.cn/gtrkzxbhkb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xuanzx.com/gtaluaxvgn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gaohongyu789.top/gtzfgrjjag.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gtachguarj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gtiwqicwjq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.aibaodan.cn/gtkavsjooe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.0kj1m.cn/gtdojqkpta.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gaohongyu789.top/gtfhswklfl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ppjwa.cn/gtnhyyujxf.html

[N04] 斐波那契数列
来源：http://hz.9152youxi.cn/gtrlusmjqd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.vqdsnc.cn/gtcdwitlam.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hfpthk.cn/gtihathqyg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.9152youxi.cn/gtkpgoubhs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pycfn.com/gtxygykdfc.html


<!-- 参考信息 -->