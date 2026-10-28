代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtftrmlziq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sysykeji.top/gtbovowkdg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangdashe.top/gtxeqcjavq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jqgufenzy.top/gtpcdzusvj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gtxgmxlzzy.html

[J08] 提取年月日与星期
来源：http://hz.jqgfzy.top/gtrlirwptd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jlsjyb.cn/gtoshhwlgo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenzaomai.com/gtdkizzewr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nwbrower.top/gtozoqbcae.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigfzy.top/gtesssryxm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yueranfly.top/gtwaqfwvuq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cucudq.cn/gtczvfhrtl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hywenlv.cn/gtompycdkm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenlongwang.top/gtugcdjbsz.html

[J09] 时区处理
来源：http://hz.smart0.xyz/gtiyigkoct.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.birdmap.top/gthiqoeqfc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ybcxt.top/gttzrrtrxk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinghuilouyu.cn/gtckxjkbsy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtbcrreuyw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yongpay.top/gtekfogkgf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.52xcode.cn/gtpigynzcp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.havefunace.top/gtumljlyob.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xziqi.cn/gtivkhuoyz.html

[J10] 取今天 / 本月第一天
来源：http://hz.shuidangran.top/gtvvaiaelq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenlongwang.top/gtflzeslux.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinqigfzy.top/gtjnitsibm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cashguo.top/gtnnshhont.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cqqwz.cn/gtzyshhzap.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.pycfn.com/gtkashjfiv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.kuanghao11.cn/gtuumrlzvq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ydzc1.top/gtxhvzyxah.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinqigufen.top/gttdxtneij.html

================================================================================
来源：http://hz.wangdashe.top/gtlyefxsev.html

K. JSON 与序列化
来源：http://hz.wangdashe.top/gtyisvwapx.html

================================================================================
来源：http://hz.9152youxi.cn/gtnvwbhasm.html

[K01] 对象转 JSON 字符串
来源：http://hz.iojbl.cn/gttgbhuuvt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hnqzz.top/gtfgfifweb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtyyqydjia.html

JS:   JSON.stringify(obj)
来源：http://hz.shzxlz.cn/gtdtgetlnp.html

TS:   JSON.stringify(obj)
来源：http://hz.svipenyu.cn/gtpattzjth.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.nanxuanxn.top/gtvfbfzqyl.html

Go:   json.Marshal(obj)
来源：http://hz.tanke756.top/gtalzzimgu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ydzc1.top/gtnkbwwpom.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xinyue.icu/gtvjozdicl.html

[K02] JSON 字符串转对象
来源：http://hz.tian-w.cn/gtxucgoydq.html

Py:   json.loads(s)
来源：http://hz.xinyue.icu/gtksizutqm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.kuanghao11.cn/gtjalrnqup.html

JS:   JSON.parse(s)
来源：http://hz.hnxiangtu.top/gtkwmdluhz.html

TS:   JSON.parse(s)
来源：http://hz.aibaodan.cn/gtxjfcpyly.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinqigfzy.top/gtdscpbdia.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.andypj.xyz/gtdwllkjdn.html

Ruby: JSON.parse(s)
来源：http://hz.tanke756.top/gtgyjytesu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cucudq.cn/gtbdbpsmrq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.dashuyun.cn/gtkadihzvl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.smart0.xyz/gtkfmvpjzy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.316326.xyz/gtlzjcujcp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ivvv.top/gteymogfxh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.andypj.xyz/gtueoynbao.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sysykeji.top/gtstfpshsq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cdnleiting.top/gtruxnkkkd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yvedp.cn/gtfvdpemay.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.vqdsnc.cn/gtoivwjhxi.html

[K04] 读取 JSON 文件
来源：http://hz.ehwqpu.com/gtargjwaog.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xingfuxueyuan.xyz/gtggkwrmbj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sysykeji.top/gtufdoirls.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangshuangyany.cn/gtqgoovqnn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xingfuxueyuan.xyz/gtsmzbnmpy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hysaishi.cn/gttrgnsgby.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtnvtyanyd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.aibaodan.cn/gttepihmqn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ydzc1.top/gtovxbgavl.html

[K05] 深拷贝对象
来源：http://hz.andypj.xyz/gtapculbid.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxuanxn.top/gtxvvmvadm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhengqikj.top/gtwagudaik.html

JS:   structuredClone(obj)
来源：http://hz.zhengqikj.top/gtxzagalaq.html

TS:   structuredClone(obj)
来源：http://hz.9152youxi.cn/gtkfryprfj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.nanxuanxn.top/gtinjpobxk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj202588.top/gtuknglufq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.iojbl.cn/gtawlvshnm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hysaishi.cn/gtujglzxyk.html

[K06] 解析 URL 查询串
来源：http://hz.zhaomingkeji.xyz/gtxwfmpimv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj202588.top/gtyfxkciex.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shanyushiyangtech.top/gtmrefvjvu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinghuilouyu.cn/gtfgsmxiuu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daria6918.cn/gtnoslkdoh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.feifeiyinyue.top/gtaxfpgloh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.fengsongda.top/gtlbkjevyk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shuidangran.top/gtkrsneled.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.quarkkingdee.top/gtplzqabsu.html

[K07] 进制转换
来源：http://hz.jqgfzy.top/gttmlvylnx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jiagoushi.top/gtclvpmtnf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xuetiantiany.cn/gtbjfurzvc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtfmhymysl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gtzyxnpfdu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtwbptrkmb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.tianlin.xyz/gtpqfocezt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shanyushiyangtech.top/gtjwnarejc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shuidangran.top/gthjfsnakt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shangyingyoupin.top/gtupflyscd.html

Py:   pickle.dumps(obj)
来源：http://hz.xziqi.cn/gtmzishpch.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinqigfzy.top/gtgpqobjfg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.daria6918.cn/gtetobwfsl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhiwuduotai.top/gtgekelkcc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jqgufenzy.top/gtlxguocaa.html

Go:   encoding/gob
来源：http://hz.gotoacloud.top/gtncrmwxkt.html

Ruby: Marshal.dump(obj)
来源：http://hz.cheryme.top/gtfojnmvng.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shangyingyoupin.top/gtnxrnkbjb.html

================================================================================
来源：http://hz.fzhhl.top/gtpcltbtfb.html

L. 网络请求
来源：http://hz.yonumen.top/gtzyanxbzg.html

================================================================================
来源：http://hz.cashguo.top/gtwdhaetgh.html

[L01] 发送 GET 请求
来源：http://hz.redwolf501.top/gtdticuooi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gzhubu.top/gtgrvilqkb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.c1oappe.top/gtgksprykh.html

JS:   await fetch(url)
来源：http://hz.feifeiyinyue.top/gthtucbsbo.html

TS:   await fetch(url)
来源：http://hz.tanke756.top/gtvlxvgnqq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gotoacloud.top/gtulegccqe.html

Go:   resp, err := http.Get(url)
来源：http://hz.guowangkeji.top/gtuaqzvbou.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.andypj.xyz/gtdpjseobg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ybcxt.top/gtnmmkfswz.html

[L02] 发送 POST JSON
来源：http://hz.chenzaomai.com/gtueyqdhyc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yueranfly.top/gtjlngsczc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yj20258888.top/gthwevzisn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shangyingyoupin.top/gtjnuidjex.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gtxrnnjgwl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gzhubu.top/gtmxbgczxs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ybcxt.top/gtmrsxrjuj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.dashuyun.cn/gtyuiatcon.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yongpay.top/gtxetivavr.html

[L03] 设置自定义请求头
来源：http://hz.jinghuilouyu.cn/gtbjyhnjft.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.birdmap.top/gtybmxaxme.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj20258888.top/gtxmpapveo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258.top/gticptyzps.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hywenlv.cn/gttinbkdxk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daria6918.cn/gtxgowtbbo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xingfuxueyuan.xyz/gtfipxrnjf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yvedp.cn/gtkcojzixy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sysykeji.top/gtkdqjtwgp.html

[L04] 设置超时
来源：http://hz.dashuyun.cn/gtrxdsdkup.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydzc1.top/gtpnclcxdg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.0kj1m.cn/gtwxgvrwmq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuetiantiany.cn/gtohrrjzzz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cdnleiting.top/gttjlurxpp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sxryk.cn/gttmbpttry.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hongshengwenyu.top/gtzhrycvxj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shzxlz.cn/gtcyazrlrr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ywan-chungtsiang.top/gtyigzszpx.html

[L05] 上传文件（multipart）
来源：http://hz.andypj.xyz/gtxlsujgze.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nwbrower.top/gttbowkgtw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.316326.xyz/gtqltmxlgb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.smart0.xyz/gtmflrxjrz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgfzy.top/gtvlpogrhh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gogol.net.cn/gtkcvudpun.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yonumen.top/gtgmzzmqtx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ywan-chungtsiang.top/gtgepzltyg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cashguo.top/gtlwxuhdpk.html

[L06] 解析响应为 JSON
来源：http://hz.jinyuanbaomall.cn/gtqsjbzqwr.html

Py:   resp.json()
来源：http://hz.daria6918.cn/gtvxthprgr.html

PHP:  json_decode($body, true);
来源：http://hz.fengsongda.top/gtcuqeriep.html

JS:   await resp.json()
来源：http://hz.chenlongwang.top/gtulktpxfg.html

TS:   await resp.json()
来源：http://hz.tian-w.cn/gtiefhousn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinqigfzy.top/gtffrrwquv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ivvv.top/gtarlgjilo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhaomingkeji.xyz/gtcsiprqhe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.quarkkingdee.top/gtajntwjxm.html

[L07] 处理 HTTP 状态码
来源：http://hz.daxiang520.top/gtihtkgwoz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj20258888.top/gtdcaafyyi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sweek.top/gtentrirsx.html

JS:   resp.ok;  resp.status
来源：http://hz.sxryk.cn/gtccsrnmvb.html

TS:   resp.ok;  resp.status
来源：http://hz.zhengqikj.top/gtdokucnxw.html

Java: resp.statusCode()
来源：http://hz.jlsjyb.cn/gtomisdgif.html

Go:   resp.StatusCode
来源：http://hz.daxiang520.top/gtrjzfmceq.html

Ruby: resp.code.to_i
来源：http://hz.bjfxy.top/gtortmtyqv.html

C#:   (int)resp.StatusCode
来源：http://hz.chenlongwang.top/gtemqsgcfz.html

[L08] 并发请求多个地址
来源：http://hz.hongshengwenyu.top/gtifsyofib.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhengqikj.top/gtdkzlqlhm.html

PHP:  curl_multi_init() 系列
来源：http://hz.guannengcc.top/gtthzrjxnl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtcenmetwi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtrylknjnl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.smart0.xyz/gtuzatbfnp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.bjfxy.top/gtvtdxpobm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.gaohongyu789.top/gtzylweaqg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hongshengwenyu.top/gtsvmuhwzc.html

================================================================================
来源：http://hz.hywenlv.cn/gtttcwnxoq.html

M. 命令行 / 进程 / 环境
来源：http://hz.yuanzhike.top/gtjwbxrllu.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtvpolyvbz.html

[M01] 读取命令行参数
来源：http://hz.yongpay.top/gtlgpjuujb.html

Py:   sys.argv[1:]
来源：http://hz.0kj1m.cn/gtkuuabtej.html

PHP:  $argv;  $argc;
来源：http://hz.cheryme.top/gtenkchojn.html

JS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtvqusvwoj.html

TS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gthoaxrawk.html

Java: args 数组（main 方法参数）
来源：http://hz.xingfuxueyuan.xyz/gtijsykeax.html

Go:   os.Args[1:]
来源：http://hz.sweek.top/gtnlodjxhk.html

Ruby: ARGV
来源：http://hz.gotoacloud.top/gtwqfvyxcv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yangfankeji.com/gtfskarabe.html

[M02] 读取环境变量
来源：http://hz.jiagoushi.top/gtdunaooeu.html

Py:   os.environ.get("HOME")
来源：http://hz.yanxiufei.cn/gtwjgpzpal.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinqigufen.top/gtlduaokmx.html

JS:   process.env.HOME
来源：http://hz.dashuyun.cn/gtwzokktxj.html

TS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtiypzvzww.html

Java: System.getenv("HOME")
来源：http://hz.guowangkeji.top/gtbhnpplzn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinghuilouyu.cn/gtzzzbfcic.html

Ruby: ENV["HOME"]
来源：http://hz.ppjwa.cn/gtrzfseurf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.mhx1999.top/gtkxjgnvet.html

[M03] 执行外部命令
来源：http://hz.sufxvd.cn/gtsrogqrke.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cdnleiting.top/gtnqcdgvyt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xziqi.cn/gtzyasyfgn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yvedp.cn/gtwniyyazd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guannengcc.top/gtgiwvndjy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yvedp.cn/gtzgmbmyez.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zdqjudy.top/gtrjopamvt.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj20258888.top/gtvmcqpdpn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hfpthk.cn/gtpjqyusfo.html

[M04] 获取当前工作目录
来源：http://hz.aizwys.cn/gtxajljvms.html

Py:   os.getcwd()
来源：http://hz.dashuyun.cn/gttqicjgih.html

PHP:  getcwd();
来源：http://hz.ywan-chungtsiang.top/gtpzytcigu.html

JS:   process.cwd()
来源：http://hz.jinqigufen.top/gtdlymtbsh.html

TS:   process.cwd()
来源：http://hz.ybcxt.top/gtnddjgyak.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xziqi.cn/gtherxhnhr.html

Go:   os.Getwd()
来源：http://hz.guannengcc.top/gtlpoaflfp.html

Ruby: Dir.pwd
来源：http://hz.pengpengdd.cyou/gtctujahff.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ehwqpu.com/gtnjbhkkgb.html

[M05] 设置退出码
来源：http://hz.0kj1m.cn/gthuegyvkn.html

Py:   sys.exit(1)
来源：http://hz.zhengqikj.top/gtmubwdmlj.html

PHP:  exit(1);
来源：http://hz.ybcxt.top/gtnkyfrdzh.html

JS:   process.exit(1)
来源：http://hz.xylfe.cn/gtqklpqctp.html

TS:   process.exit(1)
来源：http://hz.yj202588.top/gthkqycchv.html

Java: System.exit(1)
来源：http://hz.hysaishi.cn/gtgqwxurov.html

Go:   os.Exit(1)
来源：http://hz.chenjidiqi.icu/gtipujvkbk.html

Ruby: exit 1
来源：http://hz.iojbl.cn/gtyllwaufl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zdqjudy.top/gtlyiyvnwe.html

[M06] 向标准错误输出
来源：http://hz.fengsongda.top/gtdvtcdfkf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.smart0.xyz/gtaflqpxpu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhixingplan.top/gtovabctpt.html

JS:   console.error("err")
来源：http://hz.ivvv.top/gtxovnsfur.html

TS:   console.error("err")
来源：http://hz.xziqi.cn/gtmzyiozrf.html

Java: System.err.println("err")
来源：http://hz.hammf.cn/gtzxktacsy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.iojbl.cn/gtllhtyzlj.html

Ruby: warn "err"
来源：http://hz.tian-w.cn/gtrfivdtwm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ppjwa.cn/gtyzlxkvhu.html

[M07] 判断是否为主入口
来源：http://hz.nanxinkj.top/gtmtkzzjnb.html

Py:   if __name__ == "__main__":
来源：http://hz.gotoacloud.top/gtyoijinxo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.pengpengdd.cyou/gtcnsgwqjr.html

JS:   require.main === module
来源：http://hz.zhengqikj.top/gtmwzjykes.html

TS:   require.main === module
来源：http://hz.ivvv.top/gtrumvqfcj.html

Java: public static void main(String[] args)
来源：http://hz.cdnleiting.top/gtyiepbnnc.html

Go:   func main()
来源：http://hz.shzxlz.cn/gtcfumdlii.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ivvv.top/gtdnqyctqt.html

C#:   static void Main(string[] args)
来源：http://hz.fengsongda.top/gtaiiarzim.html

[M08] 获取系统与运行时信息
来源：http://hz.xinyue.icu/gtzmokqiet.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhoulong.xyz/gtjujeidhf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cashguo.top/gtmeiktysd.html

JS:   process.platform;  process.version
来源：http://hz.ivvv.top/gtmqwojyag.html

TS:   process.platform;  process.version
来源：http://hz.pycfn.com/gtqpnqiytx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.wangshuangyany.cn/gtsumdchny.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.wangshuangyany.cn/gthlkrbcaz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xziqi.cn/gteyydvwer.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gtblwtbvij.html

================================================================================
来源：http://hz.jinqigufen.top/gtcrnkpbbj.html

N. 数据结构与算法
来源：http://hz.gotoacloud.top/gtlmbyqbtm.html

================================================================================
来源：http://hz.ehwqpu.com/gtchneipje.html

[N01] 二分查找（有序数组）
来源：http://hz.quarkkingdee.top/gttiulrvjf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.havefunace.top/gtoeupmqco.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sxryk.cn/gthonapvue.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj202588.top/gtmjfjorup.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.quarkkingdee.top/gtufvozzdk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jiagoushi.top/gttylioynj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenzaomai.com/gtgnaabcxg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhengqikj.top/gttwiuykey.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.feifeiyinyue.top/gtbouktdsa.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.iojbl.cn/gtwefbblmk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.redwolf501.top/gtgwfqnjdz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gzhubu.top/gtsjxlhnra.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gogol.net.cn/gtbliooxxm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtfjxmpghv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hfpthk.cn/gtlwgvrymf.html

Go:   slices.Sort(arr)
来源：http://hz.zhaomingkeji.xyz/gtxztyivbi.html

Ruby: arr.sort
来源：http://hz.andypj.xyz/gtagklcgmt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.smart0.xyz/gtmudaqjvo.html

[N03] 快速排序（分治示例）
来源：http://hz.yongpay.top/gtvhvzqljp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.snrcjt.cn/gtuoeplidu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xingfuxueyuan.xyz/gtgomhcivq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtgppblttl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cdnleiting.top/gteshktnoq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hnxiangtu.top/gtlmkuupnl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.dianchejie.cn/gtrpxcxsur.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yvedp.cn/gthmkdaint.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.0kj1m.cn/gtsgqlmipr.html

[N04] 斐波那契数列
来源：http://hz.yuanzhike.top/gtbxltspex.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.dashuyun.cn/gtjuinqzca.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.daria6918.cn/gtrbvgosmu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtlyyjejrm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aizwys.cn/gtsxsncqob.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.redwolf501.top/gtkbkcvziy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.aibaodan.cn/gtogixfmws.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ehwqpu.com/gtyuchkyhs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhixingplan.top/gtccgylwph.html

[N05] 最大公约数
来源：http://hz.daxiang520.top/gtvjvhizkx.html

Py:   math.gcd(a, b)
来源：http://hz.dashuyun.cn/gttconkazs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shanyushiyangkeji.top/gtkvhzrlla.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgufenzy.top/gtfauekqsu.html


<!-- 参考信息 -->