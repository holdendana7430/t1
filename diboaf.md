代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nwbrower.top/gtabvaeixv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ydjk.org.cn/gtjxalabli.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.9152youxi.cn/gtypqhlvwa.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jlsjyb.cn/gtztnzlpdt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.0kj1m.cn/gtlmhafqwg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhijiandao.cn/gtbdrfteib.html

[J09] 时区处理
来源：http://hz.yuanzhike.top/gtesxfztfo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cdnleiting.top/gtxihzahbc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yueranfly.top/gtonrnanfg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.316326.xyz/gtsbwaljau.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj202588.top/gtghhwvzyb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nwbrower.top/gtfzjmedym.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jiagoushi.top/gtzmthcwiq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dianchejie.cn/gtfrvrskaj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhoulong.xyz/gtnuedmubw.html

[J10] 取今天 / 本月第一天
来源：http://hz.shanyushiyangtech.top/gttzpolcbq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.vqdsnc.cn/gtklpdultq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ydjk.org.cn/gtzjpwlbds.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.quarkkingdee.top/gtdjifvbfu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.fzhhl.top/gtnfmvggsk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangtech.top/gtvrkalumy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hnqzz.top/gtdqxgjsjk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinyuanbaomall.cn/gtgckxoltw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yongpay.top/gtdvblzuck.html

================================================================================
来源：http://hz.hnqzz.top/gtjfazylgs.html

K. JSON 与序列化
来源：http://hz.aibaodan.cn/gtprlsqmlt.html

================================================================================
来源：http://hz.snrcjt.cn/gtynwifeuf.html

[K01] 对象转 JSON 字符串
来源：http://hz.guowangkeji.top/gtfbybxzdz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydzc1.top/gtcrkroifc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tian-w.cn/gtfaaqxkie.html

JS:   JSON.stringify(obj)
来源：http://hz.birdmap.top/gtnvdbzkwd.html

TS:   JSON.stringify(obj)
来源：http://hz.ehwqpu.com/gtgrmkzdfo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ybcxt.top/gtqscqpate.html

Go:   json.Marshal(obj)
来源：http://hz.zhaomingkeji.xyz/gtlpiaphza.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xingfuxueyuan.xyz/gtfwhgjecp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.52xcode.cn/gtahjrzppk.html

[K02] JSON 字符串转对象
来源：http://hz.jinghuilouyu.cn/gtwqyjuzhj.html

Py:   json.loads(s)
来源：http://hz.yj20258.top/gtoecokyws.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xuanzx.com/gtvbppcyap.html

JS:   JSON.parse(s)
来源：http://hz.iojbl.cn/gtuqudboes.html

TS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtxaauesay.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jqgufenzy.top/gtanvivjfd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.guowangkeji.top/gtjxqidibr.html

Ruby: JSON.parse(s)
来源：http://hz.zycfv.cn/gtyluheumf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ydjk.org.cn/gtzhnxfikm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhixingplan.top/gtjonlidbc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gtbsahfdmj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinghuilouyu.cn/gtvxsuqrrp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shangyingyoupin.top/gtamedbuay.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxinkj.top/gtlsiypopf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xinyue.icu/gtkjqgeysl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gogol.net.cn/gtqtmyjitb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangshuangyany.cn/gtgvhvomkv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xziqi.cn/gtirnpbxrn.html

[K04] 读取 JSON 文件
来源：http://hz.hfpthk.cn/gtcvsjjgmb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.pengpengdd.cyou/gtarsbjbwn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hysaishi.cn/gtspyyuvba.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cheryme.top/gtbpyielqi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tanke756.top/gtlfgwkwcc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sxryk.cn/gtzkrcvegl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtuhzacuzb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hnxiangtu.top/gtosyybsok.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.havefunace.top/gtshxdrsjd.html

[K05] 深拷贝对象
来源：http://hz.shzxlz.cn/gtgdafbbop.html

Py:   copy.deepcopy(obj)
来源：http://hz.gogol.net.cn/gtkhpbtscw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cashguo.top/gtxfzanquc.html

JS:   structuredClone(obj)
来源：http://hz.guannengcc.top/gtazncytww.html

TS:   structuredClone(obj)
来源：http://hz.ydzc1.top/gtourihyir.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.redwolf501.top/gtmbrmfonh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ydzc1.top/gtnuwyhusw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shangyingyoupin.top/gtddrdfahh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.svipenyu.cn/gtbbdzrjde.html

[K06] 解析 URL 查询串
来源：http://hz.ydzc1.top/gtjhvxctfw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinqigufen.top/gtwobvnpcr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinqigufen.top/gtnnzgpcos.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.kuanghao11.cn/gtstqmwkjx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gtwezprhta.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.316326.xyz/gtiiyuxrxx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dianchejie.cn/gtuzyrrnzb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.svipenyu.cn/gtigcojish.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.guowangkeji.top/gtfmnsmkir.html

[K07] 进制转换
来源：http://hz.ydzc1.top/gtalmzhekl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhoulong.xyz/gteoztkpiz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hysaishi.cn/gtypyrmicb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.birdmap.top/gtsitqvdux.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtjbwyhxhd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtrbjlkbmu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.chenjidiqi.icu/gtfkddhezy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.quarkkingdee.top/gtlbwspzka.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nanxuanxn.top/gtolkotgtc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj202588.top/gtuojopvqc.html

Py:   pickle.dumps(obj)
来源：http://hz.guannengcc.top/gtjgrtvuxt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cqqwz.cn/gtesiwodxm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.nwbrower.top/gtwkxuovsf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.haohaochexian.top/gtyogrubqt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.c1oappe.top/gtfhtfqpva.html

Go:   encoding/gob
来源：http://hz.hnxiangtu.top/gtcbihnylb.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhixingplan.top/gtmnzelvvo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuetiantiany.cn/gtenzihepy.html

================================================================================
来源：http://hz.zdqjudy.top/gtpsyvccpr.html

L. 网络请求
来源：http://hz.shanyushiyangkeji.top/gtwoxgaiqg.html

================================================================================
来源：http://hz.xinyue.icu/gtalccladj.html

[L01] 发送 GET 请求
来源：http://hz.ydjk.org.cn/gthsaplsyc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cdnleiting.top/gtwazcbqgc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.pengpengdd.cyou/gtipimqusq.html

JS:   await fetch(url)
来源：http://hz.chenzaomai.com/gtnuddjmqg.html

TS:   await fetch(url)
来源：http://hz.zhiwuduotai.top/gtarijfnom.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.svipenyu.cn/gtifxevwqo.html

Go:   resp, err := http.Get(url)
来源：http://hz.gogol.net.cn/gtwiqcteyd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinghuilouyu.cn/gtmmoehnmi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cucudq.cn/gttyeuntfp.html

[L02] 发送 POST JSON
来源：http://hz.chenzaomai.com/gtxathfyxy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgufenzy.top/gtmvgiyvaa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hnqzz.top/gtnxjkxbdq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenlongwang.top/gtzeidldxr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gtxnqocioh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xylfe.cn/gtomhbpsdj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ivvv.top/gtbggduhal.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tianlin.xyz/gtcvealjql.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cheryme.top/gtnjtxicds.html

[L03] 设置自定义请求头
来源：http://hz.pycfn.com/gtmycudxhh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xylfe.cn/gtigxuqmxy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.52xcode.cn/gtrubbigem.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangtech.top/gtjgtitefm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.smart0.xyz/gtqsrzvmhg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jqgufenzy.top/gtxnwxfvrf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.haohaochexian.top/gtrzbbuudf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj202588.top/gtajcksksj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yj20258.top/gtyzonvzit.html

[L04] 设置超时
来源：http://hz.yonumen.top/gtyqyjqrzi.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gogol.net.cn/gtdshyyytf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.chenzaomai.com/gtwmjaqshq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenzaomai.com/gttzjsjtwv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hfpthk.cn/gtoximtwjj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinghuilouyu.cn/gtcdwdrtxn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ywan-chungtsiang.top/gtdlcqlhly.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhaomingkeji.xyz/gtaibkkisj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.wangshuangyany.cn/gtemngjlbw.html

[L05] 上传文件（multipart）
来源：http://hz.guannengcc.top/gtsnxzbcih.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tanke756.top/gtajwzgfev.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shzxlz.cn/gtheksgzyh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhixingplan.top/gtolugnbla.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhoulong.xyz/gtofyzhfxx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuetiantiany.cn/gtuuyrcxon.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yuxming.cn/gtmlfpnagu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ppjwa.cn/gtjkjrjaxs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.andypj.xyz/gtpnqhureg.html

[L06] 解析响应为 JSON
来源：http://hz.jinyuanbaomall.cn/gtfadxvgpi.html

Py:   resp.json()
来源：http://hz.meibo888.top/gtqupsgyra.html

PHP:  json_decode($body, true);
来源：http://hz.chenjidiqi.icu/gtcpmcoeeg.html

JS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtymenltyg.html

TS:   await resp.json()
来源：http://hz.fengsongda.top/gtcddttacm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yonumen.top/gtxlsncqgr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gaohongyu789.top/gtvcfyyoam.html

Ruby: JSON.parse(resp.body)
来源：http://hz.kuanghao11.cn/gturrkzvql.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhongyouzk.top/gtvvcjuvww.html

[L07] 处理 HTTP 状态码
来源：http://hz.tianlin.xyz/gtlkdahjho.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yonumen.top/gtfuhszqbn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj202588.top/gtxbvhzatg.html

JS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtxmaanibb.html

TS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtbnrvkgtq.html

Java: resp.statusCode()
来源：http://hz.zhoulong.xyz/gtephpcwyp.html

Go:   resp.StatusCode
来源：http://hz.ehwqpu.com/gtdfekhzny.html

Ruby: resp.code.to_i
来源：http://hz.ywan-chungtsiang.top/gtdkyyegpp.html

C#:   (int)resp.StatusCode
来源：http://hz.ivvv.top/gtrfjdkdqr.html

[L08] 并发请求多个地址
来源：http://hz.aizwys.cn/gtuevubcwr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ppjwa.cn/gtwhcjaplf.html

PHP:  curl_multi_init() 系列
来源：http://hz.mhx1999.top/gtvwyrdhcn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gtlmjuqlgv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gtxwmasalc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenlongwang.top/gtxhqrqbxz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxuanxn.top/gthlevlqbu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cqqwz.cn/gtdcfqhxku.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shanyushiyangkeji.top/gtxoocarbf.html

================================================================================
来源：http://hz.cqqwz.cn/gtmlgdpisq.html

M. 命令行 / 进程 / 环境
来源：http://hz.zycfv.cn/gtmotcizcp.html

================================================================================
来源：http://hz.fengsongda.top/gttrznqjhn.html

[M01] 读取命令行参数
来源：http://hz.cqqwz.cn/gtvhquhceb.html

Py:   sys.argv[1:]
来源：http://hz.xingfuxueyuan.xyz/gtmjfmivwx.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigfzy.top/gtgpvawush.html

JS:   process.argv.slice(2)
来源：http://hz.nwbrower.top/gttoafbfsl.html

TS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtgpwkngrr.html

Java: args 数组（main 方法参数）
来源：http://hz.wangdashe.top/gtjembyqdr.html

Go:   os.Args[1:]
来源：http://hz.jqgufenzy.top/gtilgqoqrk.html

Ruby: ARGV
来源：http://hz.ybcxt.top/gtnxwqabyu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xziqi.cn/gtdjdcaslr.html

[M02] 读取环境变量
来源：http://hz.c1oappe.top/gthntcdvpi.html

Py:   os.environ.get("HOME")
来源：http://hz.9152youxi.cn/gtojribwmq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.aibaodan.cn/gtodpxpcwf.html

JS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtjdykcapm.html

TS:   process.env.HOME
来源：http://hz.hnqzz.top/gtuptjeeue.html

Java: System.getenv("HOME")
来源：http://hz.zhixingplan.top/gtnkjhwamc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.birdmap.top/gtczglhdav.html

Ruby: ENV["HOME"]
来源：http://hz.snrcjt.cn/gtvxtynuji.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.iojbl.cn/gtiiagdgcr.html

[M03] 执行外部命令
来源：http://hz.jqgufenzy.top/gtnmghbtar.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.snrcjt.cn/gtksthkvsc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.havefunace.top/gtybumcdmn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.redwolf501.top/gtdlxpanlh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hysaishi.cn/gtinoqpauh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.iojbl.cn/gtgvkivvtc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zdqjudy.top/gtlqnefydk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jiagoushi.top/gtueqapapc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.9152youxi.cn/gtetpjrdth.html

[M04] 获取当前工作目录
来源：http://hz.yangfankeji.com/gtuubnmppe.html

Py:   os.getcwd()
来源：http://hz.zycfv.cn/gtbbnzwwet.html

PHP:  getcwd();
来源：http://hz.dianchejie.cn/gtyasyqhkw.html

JS:   process.cwd()
来源：http://hz.redwolf501.top/gtqxaasvwb.html

TS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtznlupsyy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cashguo.top/gtdkufolqi.html

Go:   os.Getwd()
来源：http://hz.jinghuilouyu.cn/gtxpplxgzz.html

Ruby: Dir.pwd
来源：http://hz.xuanzx.com/gtqcxcttwk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.birdmap.top/gtbxmlmjip.html

[M05] 设置退出码
来源：http://hz.haohaochexian.top/gtgkjlojmc.html

Py:   sys.exit(1)
来源：http://hz.gaohongyu789.top/gttwxoldga.html

PHP:  exit(1);
来源：http://hz.sweek.top/gtfaztclig.html

JS:   process.exit(1)
来源：http://hz.ydzc1.top/gteqmmwghz.html

TS:   process.exit(1)
来源：http://hz.yongpay.top/gtgpmnsygo.html

Java: System.exit(1)
来源：http://hz.guannengcc.top/gtgawcyylv.html

Go:   os.Exit(1)
来源：http://hz.gotoacloud.top/gtwckfhyqd.html

Ruby: exit 1
来源：http://hz.haohaochexian.top/gtztiifzdy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.svipenyu.cn/gtzzemdoca.html

[M06] 向标准错误输出
来源：http://hz.nwbrower.top/gtkhivmnpm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cucudq.cn/gtbzompwrr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenzaomai.com/gtdzvwictc.html

JS:   console.error("err")
来源：http://hz.shanyushiyangtech.top/gtxawktjvg.html

TS:   console.error("err")
来源：http://hz.xingfuxueyuan.xyz/gtxrohsxrc.html

Java: System.err.println("err")
来源：http://hz.ywan-chungtsiang.top/gtiiuvwoav.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenzaomai.com/gtatpyxsfz.html

Ruby: warn "err"
来源：http://hz.yj20258888.top/gtonypapcb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yonumen.top/gtryhndkde.html

[M07] 判断是否为主入口
来源：http://hz.daxiang520.top/gtjychmwjx.html

Py:   if __name__ == "__main__":
来源：http://hz.zhoulong.xyz/gtbmsspwlw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhengqikj.top/gtrlkkouou.html

JS:   require.main === module
来源：http://hz.feifeiyinyue.top/gtdemrckod.html

TS:   require.main === module
来源：http://hz.guannengcc.top/gtssszteez.html

Java: public static void main(String[] args)
来源：http://hz.shuidangran.top/gtgxlqzvri.html

Go:   func main()
来源：http://hz.xylfe.cn/gttxboqtfm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.quarkkingdee.top/gtertezhwj.html

C#:   static void Main(string[] args)
来源：http://hz.jqgfzy.top/gtxbtvdwvl.html

[M08] 获取系统与运行时信息
来源：http://hz.zhiwuduotai.top/gtrzlmpfza.html

Py:   platform.system();  platform.python_version()
来源：http://hz.9152youxi.cn/gtpclswrde.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hammf.cn/gtkqglggsu.html

JS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gtmsdqnubi.html

TS:   process.platform;  process.version
来源：http://hz.xuetiantiany.cn/gtwyqimebi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hfpthk.cn/gtsfuklizz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.snrcjt.cn/gtewmfzcvf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zycfv.cn/gtlspzfcwr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sufxvd.cn/gtrmyrhsjj.html

================================================================================
来源：http://hz.sweek.top/gtwrwvwiuz.html

N. 数据结构与算法
来源：http://hz.yanxiufei.cn/gtlnilbwtc.html

================================================================================
来源：http://hz.jlsjyb.cn/gtdrkmkgll.html

[N01] 二分查找（有序数组）
来源：http://hz.xinyue.icu/gtknxpfvde.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sweek.top/gtoakvpdik.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinghuilouyu.cn/gtkxthkqjl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.0kj1m.cn/gtmdmxevyx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shanyushiyangkeji.top/gtralpfpbi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.haohaochexian.top/gtsqmiknco.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hongshengwenyu.top/gtwrnhquef.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.mhx1999.top/gtmfbfadid.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xuanzx.com/gtmishjcln.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.redwolf501.top/gtxyfrgxoi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pengpengdd.cyou/gtoderblog.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ivvv.top/gtksejyhqq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gttgoceuwq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jiagoushi.top/gtififacpo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ivvv.top/gtfrwraolx.html

Go:   slices.Sort(arr)
来源：http://hz.mhx1999.top/gtvbreoapa.html

Ruby: arr.sort
来源：http://hz.shanyushiyangkeji.top/gtanrpjgry.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.fengsongda.top/gtvqcoqdkp.html

[N03] 快速排序（分治示例）
来源：http://hz.yuanzhike.top/gtngbtdtwr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shzxlz.cn/gtutgcella.html

PHP:  // 递归实现，或用 usort
来源：http://hz.wangdashe.top/gtqruqormj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenlongwang.top/gtfpegsexn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtfjnncvvn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ehwqpu.com/gtquqewrsz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.havefunace.top/gtipdudcnl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xziqi.cn/gtajlohuwm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.guannengcc.top/gtkoftcuvm.html

[N04] 斐波那契数列
来源：http://hz.yuxming.cn/gtinggejqg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hysaishi.cn/gtdytvnbjv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xziqi.cn/gtlakqirce.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xylfe.cn/gtyappzvym.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtrpuejscg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xingfuxueyuan.xyz/gtbbdsjeld.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sweek.top/gtkbfmyonv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ydzc1.top/gtskbwxmxk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhijiandao.cn/gtctcflpmy.html

[N05] 最大公约数
来源：http://hz.daria6918.cn/gtcjalijnk.html

Py:   math.gcd(a, b)
来源：http://hz.jiagoushi.top/gtqlgdmjiq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhoulong.xyz/gtnbozbnqi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigfzy.top/gtjgjkhjyt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dianchejie.cn/gtoayrjbgx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhengqikj.top/gteltrlppo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xinyue.icu/gtysubzxuy.html

Ruby: a.gcd(b)
来源：http://hz.zycfv.cn/gtkvmlwckt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ehwqpu.com/gtsjwemvbm.html

[N06] 判断回文字符串
来源：http://hz.sysykeji.top/gtisosgdzq.html

Py:   s == s[::-1]
来源：http://hz.jinghuilouyu.cn/gtisvemldy.html

PHP:  $s === strrev($s);
来源：http://hz.zhengqikj.top/gtejxcyuhy.html


<!-- 参考信息 -->