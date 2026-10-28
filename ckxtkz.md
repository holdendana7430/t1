代发 wailian999

Py:   (end - start).total_seconds()
来源：http://hz.sweek.top/gttndtzsyf.html

PHP:  $end->diff($start)->days;
来源：http://hz.hfpthk.cn/gtotsruxzf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ivvv.top/gtdsfctluv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xuanzx.com/gtupajpbkj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jianghu66.top/gtbmcauqfl.html

Go:   end.Sub(start).Hours()
来源：http://hz.yongpay.top/gtrxlazyaq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.dianchejie.cn/gtowlyamum.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydjk.org.cn/gtcrttjifp.html

[J07] 比较两个日期
来源：http://hz.chenjidiqi.icu/gtiyilxgnf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtrevzhzxy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.smart0.xyz/gtkqpgjntm.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.birdmap.top/gtrdufesmo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.iojbl.cn/gtwncubmrc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ywan-chungtsiang.top/gtrgxkyrrv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hongshengwenyu.top/gtpesovwdi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtgnvlhxvf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtwqpytxzk.html

[J08] 提取年月日与星期
来源：http://hz.fzhhl.top/gtgvtyvlwg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cdnleiting.top/gtnxyyytqw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cucudq.cn/gtcyifwdwp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigfzy.top/gtbxhruolr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shuidangran.top/gtxhmakujv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jyoumei.cn/gtugyokmsv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sufxvd.cn/gthptgpqcn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shanyushiyangtech.top/gtjwmordyd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhaomingkeji.xyz/gtllbfyicj.html

[J09] 时区处理
来源：http://hz.zdqjudy.top/gtjmknpwgk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gaohongyu789.top/gtkivybbvx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.snrcjt.cn/gthxlhsxgh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shangyingyoupin.top/gtexwjsnvg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtbdbhvlye.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xziqi.cn/gtgiqjgvhv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.bjfxy.top/gtgzbdewtn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cqqwz.cn/gtvhdnqeog.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinyuanbaomall.cn/gtgjcnaqmw.html

[J10] 取今天 / 本月第一天
来源：http://hz.andypj.xyz/gtvsrdckyp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuxming.cn/gtqgmgxwnf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.9152youxi.cn/gtybghnmxr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.feifeiyinyue.top/gtczdyokaw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenjidiqi.icu/gtltpkbmkt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cashguo.top/gthkyapazo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.fzhhl.top/gtnrnkiuju.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.svipenyu.cn/gtnutwnzjw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj202588.top/gtwvdmyuaa.html

================================================================================
来源：http://hz.9152youxi.cn/gtluswfvrh.html

K. JSON 与序列化
来源：http://hz.chenjidiqi.icu/gtkcexnayr.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtnsgftwtq.html

[K01] 对象转 JSON 字符串
来源：http://hz.mhx1999.top/gtsgsxwejn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cucudq.cn/gtjhlrzduf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yueranfly.top/gtyyolskzh.html

JS:   JSON.stringify(obj)
来源：http://hz.redwolf501.top/gtmmjubied.html

TS:   JSON.stringify(obj)
来源：http://hz.cucudq.cn/gtbaphopah.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zycfv.cn/gtkblbnmls.html

Go:   json.Marshal(obj)
来源：http://hz.xziqi.cn/gtohagbspu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nanxinkj.top/gtahvxikfr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydzc1.top/gtkyhtnpkx.html

[K02] JSON 字符串转对象
来源：http://hz.smart0.xyz/gtoguqylee.html

Py:   json.loads(s)
来源：http://hz.tianlin.xyz/gtguplunnw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinqigfzy.top/gtwyqteoub.html

JS:   JSON.parse(s)
来源：http://hz.hnqzz.top/gtsbbcmcyc.html

TS:   JSON.parse(s)
来源：http://hz.xuanzx.com/gtbxlqmmru.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tian-w.cn/gtjoinppfg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.daria6918.cn/gtqbncipdj.html

Ruby: JSON.parse(s)
来源：http://hz.yvedp.cn/gtesnertpe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yongpay.top/gtnmmkgcsh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zycfv.cn/gtzmudvkjq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.fzhhl.top/gtirftdiya.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ybcxt.top/gtrqsjxlfl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtgbhkuxge.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ehwqpu.com/gtjaejqcel.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.iojbl.cn/gtbvgsqvxl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sufxvd.cn/gtgcvvlrhw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.aizwys.cn/gttkpamrdp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.316326.xyz/gtpcixetac.html

[K04] 读取 JSON 文件
来源：http://hz.nanxuanxn.top/gtbwtbhpni.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yonumen.top/gthzczhnti.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zycfv.cn/gtorbmjgwn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtjwdjwohk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinyuanbaomall.cn/gtbebexjqu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.daria6918.cn/gtxxspyrmf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tanke756.top/gthvfccush.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhixingplan.top/gtjaxhlllx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.9152youxi.cn/gtqcxrumjh.html

[K05] 深拷贝对象
来源：http://hz.cheryme.top/gtctymxyyp.html

Py:   copy.deepcopy(obj)
来源：http://hz.hongshengwenyu.top/gttabivqkn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhiwuduotai.top/gtscujmkdw.html

JS:   structuredClone(obj)
来源：http://hz.snrcjt.cn/gtpoghcelz.html

TS:   structuredClone(obj)
来源：http://hz.hywenlv.cn/gtcalqyarn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinqigufen.top/gtrihyylrm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zdqjudy.top/gtlwdoxvce.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.haohaochexian.top/gtuyrzhpaq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cashguo.top/gtchwoujga.html

[K06] 解析 URL 查询串
来源：http://hz.chenlongwang.top/gticyvatzi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtokatejuu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj202588.top/gtzdwtaccf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtutzqbdcr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangshuangyany.cn/gtgylgwlio.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fengsongda.top/gtbcsolxwz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jianghu66.top/gtvbmunbdj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.snrcjt.cn/gthkkkurxu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.pycfn.com/gtwsmqhole.html

[K07] 进制转换
来源：http://hz.sxryk.cn/gtwqxiepsc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yueranfly.top/gtqmhhyort.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sxryk.cn/gtwnacqaeu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtjmfefrsl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtttybdfel.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtrkyviabo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.52xcode.cn/gtptuoskrg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gotoacloud.top/gtxoyhtnfr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtadljkvqj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhaomingkeji.xyz/gttgdxdaij.html

Py:   pickle.dumps(obj)
来源：http://hz.hysaishi.cn/gtsomqkydy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sufxvd.cn/gtcnmgouwb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.wangdashe.top/gtbgvpqzbe.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yvedp.cn/gtnyneajkd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.316326.xyz/gtbwempusm.html

Go:   encoding/gob
来源：http://hz.gzhubu.top/gtawuijkyj.html

Ruby: Marshal.dump(obj)
来源：http://hz.jyoumei.cn/gtevpzptwq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zycfv.cn/gtaploaqgd.html

================================================================================
来源：http://hz.hammf.cn/gtifevqela.html

L. 网络请求
来源：http://hz.yvedp.cn/gtyscwirld.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwfbytezz.html

[L01] 发送 GET 请求
来源：http://hz.tanke756.top/gtlnfluaiw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinyuanbaomall.cn/gtqvonwbya.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xylfe.cn/gtnaaoiqhc.html

JS:   await fetch(url)
来源：http://hz.ppjwa.cn/gtoddunnhs.html

TS:   await fetch(url)
来源：http://hz.ydzc1.top/gtfcgmuwtu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.daxiang520.top/gtjwdkxzdy.html

Go:   resp, err := http.Get(url)
来源：http://hz.nwbrower.top/gtvfasyspy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.smart0.xyz/gtfsxebddg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tianlin.xyz/gtdoryhlef.html

[L02] 发送 POST JSON
来源：http://hz.hongshengwenyu.top/gtydthcsrx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj202588.top/gtxrucwzbi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ywan-chungtsiang.top/gtxsgmwkie.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shuidangran.top/gtdfqkioqo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gtekencgeq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhaomingkeji.xyz/gttyikeyjl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.birdmap.top/gttmonrjko.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jianghu66.top/gtuaqtvbap.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.feifeiyinyue.top/gtgvstpwbv.html

[L03] 设置自定义请求头
来源：http://hz.hongshengwenyu.top/gtukzvuakl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hnxiangtu.top/gtlisiizhi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shangyingyoupin.top/gtmelbtuoi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jianghu66.top/gtxgirmojy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigufen.top/gtfxwynwfe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinqigfzy.top/gtwujnwwgy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.fzhhl.top/gtufkzdray.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shangyingyoupin.top/gtprpuznaj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zycfv.cn/gtbmremvmz.html

[L04] 设置超时
来源：http://hz.shuidangran.top/gthyrxvbip.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yvedp.cn/gtgurpwhkh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xingfuxueyuan.xyz/gtyzvosqlr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuetiantiany.cn/gtikftuicv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hysaishi.cn/gtmytyniwk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tian-w.cn/gtxgtijdyd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj202588.top/gtoqzutcpc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.vqdsnc.cn/gtclgjqyzg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sxryk.cn/gtrxzpatcc.html

[L05] 上传文件（multipart）
来源：http://hz.hysaishi.cn/gtekdybiso.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.0kj1m.cn/gtfxufntms.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.birdmap.top/gtahwbxbdu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtyhxyuhey.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuanzhike.top/gtphoxnoac.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tianlin.xyz/gtlvzezgqx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hongshengwenyu.top/gthkmppztq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.52xcode.cn/gtihrprrij.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.kuanghao11.cn/gtzoghijni.html

[L06] 解析响应为 JSON
来源：http://hz.pycfn.com/gtpatasvho.html

Py:   resp.json()
来源：http://hz.quarkkingdee.top/gtpxzswsib.html

PHP:  json_decode($body, true);
来源：http://hz.hysaishi.cn/gtiamgvtcv.html

JS:   await resp.json()
来源：http://hz.gaohongyu789.top/gtldwgfnjc.html

TS:   await resp.json()
来源：http://hz.gzhubu.top/gtrpzpgwmo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yangfankeji.com/gtnihvdcsu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tian-w.cn/gtrfguhjgz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.guannengcc.top/gtilggxelh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.dianchejie.cn/gtphcvvxnq.html

[L07] 处理 HTTP 状态码
来源：http://hz.cucudq.cn/gtqjtbsyem.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.c1oappe.top/gtxnavuuht.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.mhx1999.top/gtockekthp.html

JS:   resp.ok;  resp.status
来源：http://hz.fengsongda.top/gtbxdilpiu.html

TS:   resp.ok;  resp.status
来源：http://hz.316326.xyz/gtfbqhwjfo.html

Java: resp.statusCode()
来源：http://hz.zhongyouzk.top/gtzoynrckt.html

Go:   resp.StatusCode
来源：http://hz.sxryk.cn/gtsmcwlvos.html

Ruby: resp.code.to_i
来源：http://hz.fzhhl.top/gtpcfjefjd.html

C#:   (int)resp.StatusCode
来源：http://hz.shzxlz.cn/gtqifkmptt.html

[L08] 并发请求多个地址
来源：http://hz.hammf.cn/gtldlhjshc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.birdmap.top/gtxgbfzgvr.html

PHP:  curl_multi_init() 系列
来源：http://hz.kuanghao11.cn/gtyfyaofdm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nwbrower.top/gtqgxejzpr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gtkcfwpskw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daxiang520.top/gtqkiwlteq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zycfv.cn/gtcaadzbbf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.snrcjt.cn/gtlplntbgf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.meibo888.top/gtkhaayaal.html

================================================================================
来源：http://hz.daxiang520.top/gtbfmwdcys.html

M. 命令行 / 进程 / 环境
来源：http://hz.yongpay.top/gtgjsqpqbz.html

================================================================================
来源：http://hz.tian-w.cn/gtvluzldkx.html

[M01] 读取命令行参数
来源：http://hz.ppjwa.cn/gtqqrvluok.html

Py:   sys.argv[1:]
来源：http://hz.shuidangran.top/gtqxzlsaba.html

PHP:  $argv;  $argc;
来源：http://hz.xuanzx.com/gtuwgeecbi.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtheotxvrb.html

TS:   process.argv.slice(2)
来源：http://hz.smart0.xyz/gtxlexpfzz.html

Java: args 数组（main 方法参数）
来源：http://hz.ivvv.top/gtfrshfrou.html

Go:   os.Args[1:]
来源：http://hz.nwbrower.top/gtiioavbct.html

Ruby: ARGV
来源：http://hz.wangdashe.top/gtrunzbqzr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xylfe.cn/gtyiqxbxua.html

[M02] 读取环境变量
来源：http://hz.sxryk.cn/gtyhgdjldj.html

Py:   os.environ.get("HOME")
来源：http://hz.c1oappe.top/gthmgxsjls.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj202588.top/gtjjfjmkfm.html

JS:   process.env.HOME
来源：http://hz.shanyushiyangtech.top/gtnhcjfhqw.html

TS:   process.env.HOME
来源：http://hz.cqqwz.cn/gtfcgpcblu.html

Java: System.getenv("HOME")
来源：http://hz.guannengcc.top/gtoiibyxpl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gzhubu.top/gtaxxvefju.html

Ruby: ENV["HOME"]
来源：http://hz.yuanzhike.top/gtfwxnlqbk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cdnleiting.top/gtonvaiafq.html

[M03] 执行外部命令
来源：http://hz.xylfe.cn/gtwadzudcq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj202588.top/gtynrdieai.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yvedp.cn/gthkcvkooc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cashguo.top/gtmciuxhpj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ivvv.top/gtmmhqfzut.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.52xcode.cn/gtdarednfr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jyoumei.cn/gtzfnmermp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cucudq.cn/gtcrvknnhs.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yuanzhike.top/gtdrebiotr.html

[M04] 获取当前工作目录
来源：http://hz.ehwqpu.com/gtksbeqypt.html

Py:   os.getcwd()
来源：http://hz.cucudq.cn/gtfcxsgszl.html

PHP:  getcwd();
来源：http://hz.tianlin.xyz/gtzyymtjoh.html

JS:   process.cwd()
来源：http://hz.xuanzx.com/gtfekooddw.html

TS:   process.cwd()
来源：http://hz.tianlin.xyz/gtxefmaucz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.wangshuangyany.cn/gtjjajxban.html

Go:   os.Getwd()
来源：http://hz.zhaomingkeji.xyz/gtjozapmcm.html

Ruby: Dir.pwd
来源：http://hz.dashuyun.cn/gthqojnitp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jiagoushi.top/gtkvkrmgdp.html

[M05] 设置退出码
来源：http://hz.yonumen.top/gtxiaudskx.html

Py:   sys.exit(1)
来源：http://hz.sweek.top/gteofqwbty.html

PHP:  exit(1);
来源：http://hz.yj20258888.top/gtxuyjabhm.html

JS:   process.exit(1)
来源：http://hz.xinyue.icu/gtppeksrae.html

TS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gtwwrzpchg.html

Java: System.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtwfoursjg.html

Go:   os.Exit(1)
来源：http://hz.316326.xyz/gtafscxrjo.html

Ruby: exit 1
来源：http://hz.hnqzz.top/gtuhvgpnql.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hongshengwenyu.top/gtsvbejmro.html

[M06] 向标准错误输出
来源：http://hz.xuanzx.com/gttzlxslso.html

Py:   print("err", file=sys.stderr)
来源：http://hz.chenlongwang.top/gtpztmgvjf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gzhubu.top/gtrwfenmud.html

JS:   console.error("err")
来源：http://hz.dashuyun.cn/gtarjvdgoa.html

TS:   console.error("err")
来源：http://hz.gogol.net.cn/gtxwfvctxx.html

Java: System.err.println("err")
来源：http://hz.tanke756.top/gtiziqtxej.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yonumen.top/gtyvtcexzr.html

Ruby: warn "err"
来源：http://hz.iojbl.cn/gtcxgtqfgs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.chenlongwang.top/gtqcjgzicr.html

[M07] 判断是否为主入口
来源：http://hz.jianghu66.top/gtqwqzdfvi.html

Py:   if __name__ == "__main__":
来源：http://hz.shangyingyoupin.top/gtwechmurz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hnqzz.top/gtjisaxvsf.html

JS:   require.main === module
来源：http://hz.yueranfly.top/gtuwnowtqn.html

TS:   require.main === module
来源：http://hz.wangshuangyany.cn/gthiohtefr.html

Java: public static void main(String[] args)
来源：http://hz.fzhhl.top/gtqobdkamh.html

Go:   func main()
来源：http://hz.cheryme.top/gtfzymqbjq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shanyushiyangtech.top/gthigybypv.html

C#:   static void Main(string[] args)
来源：http://hz.nanxinkj.top/gtwafepvaw.html

[M08] 获取系统与运行时信息
来源：http://hz.fengsongda.top/gtldisvjhe.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gogol.net.cn/gtunyowrog.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.52xcode.cn/gtayulaykf.html

JS:   process.platform;  process.version
来源：http://hz.hnqzz.top/gtvgvvvexg.html

TS:   process.platform;  process.version
来源：http://hz.yueranfly.top/gtmknquwrg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fengsongda.top/gtcsdtcchz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.wangshuangyany.cn/gtxiqridke.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ydjk.org.cn/gtnhekfurm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.birdmap.top/gtrehqsbbh.html

================================================================================
来源：http://hz.iojbl.cn/gtouzoiawf.html

N. 数据结构与算法
来源：http://hz.xuetiantiany.cn/gthlkyjdcv.html

================================================================================
来源：http://hz.jqgufenzy.top/gttsqgsggy.html

[N01] 二分查找（有序数组）
来源：http://hz.sweek.top/gtqfsxxppm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenjidiqi.icu/gtulzzrbxk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cheryme.top/gttncbpowp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ehwqpu.com/gtejahcjsr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtghketkcm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tianlin.xyz/gtbbpxcbcy.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinqigfzy.top/gtckvvumix.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.gzhubu.top/gtbuawygrd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.daxiang520.top/gtzkqwzawe.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.feifeiyinyue.top/gtkzuhpaas.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guowangkeji.top/gtqoyhdper.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinqigfzy.top/gtauwjleup.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gtxomkatzv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xinyue.icu/gtzeohuint.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.pengpengdd.cyou/gthebxastf.html

Go:   slices.Sort(arr)
来源：http://hz.xylfe.cn/gtxcvldisf.html

Ruby: arr.sort
来源：http://hz.jinqigfzy.top/gtjbrdzxau.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.haohaochexian.top/gtqprtzpjk.html

[N03] 快速排序（分治示例）
来源：http://hz.birdmap.top/gtnihawtfc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hywenlv.cn/gtsiztslaz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cqqwz.cn/gtanmsaetd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.bjfxy.top/gtawmgomto.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jyoumei.cn/gtznrfpzgz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhongyouzk.top/gthltkdvdt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.mhx1999.top/gtluoxsfoy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hongshengwenyu.top/gtvoqleirp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yangfankeji.com/gtvbitksse.html

[N04] 斐波那契数列
来源：http://hz.haohaochexian.top/gtopunzcsb.html


<!-- 参考信息 -->