代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2dlkgiaei.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2fywhhtnt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2mxsldukr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2ewkhudxn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2wiiukhgj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2wpzqhszd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2idjengrl.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2cmohghls.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2kgswfygi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2xlhqucth.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2hnubtasa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2irkjpntn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fwkhrbcc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2qqrxgbnc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2tgmopuku.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hnthtmkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yarnwoak.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2bghzztuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpdwqtez.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2acthdwdt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wiopjrib.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zctnzgle.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2psyhdztk.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2fyvzzkfe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2qgbnctoz.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2viwbrkyz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2gmbuiard.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2tbrszveu.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2xkuxuohu.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2wbbvuaye.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2rcunwnzt.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kbxsgkyj.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yroxtgqy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fnkmrrqo.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2pswvhzzh.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2cpxpgcuc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jwpoamep.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2jtuyjrng.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2cavrvunw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2iwpvdefs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2lreijgkt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2lgnqarex.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ibzynrrq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2tzjlnjdw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2curbrsik.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2mbhnlnqa.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2giqwosca.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hyanmxli.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2dgamhqpp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2pwiiuitf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2jqranmhl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cfawooea.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2pflarrbl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ifvzzcut.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2gpkrzurs.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ffofocoq.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2uwviueda.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2gfgxxgsz.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qtyfygct.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jfkbgpdi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2pgomdzoo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2oiiyzfrt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xjczrebm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2wcwvckwv.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2qphfwxsu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jbftbtdx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2jdbvwlji.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hgbtfnbw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jxfdjbme.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jfgxkgmq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wymdhxvt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jsipnbpq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dutnjmor.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2aekrkyrv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zkrcglqi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2hcevnefm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bhyymipw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ebpnvpmq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lybvivdo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2elwuzewb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ubfsxqkb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uxqxvsbt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2lhwbctjb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2rylwvfzy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ggzhvdbn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2secvvnbb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rixsenvr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2hmdhamzg.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2wayyfvij.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sjidbhql.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xrkzcnmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fbypbtot.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2boawslaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibiuonvf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2wdzytyhq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2qohclabb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2dfyjfwzl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xdblbwee.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2gdhukfqz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2njiogiet.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rwxgyifh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2jsqlxayq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2lvfvqvwl.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zmshxfhe.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tvsgpuih.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2bjcmzesq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tdumheon.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2yntthoqn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2cylrzfmb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2odnpaxvr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2olciuhfb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2gmeluxar.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2eehwtlcr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2wfevsidz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2fyngcihv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2fbbodbhk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2awdkjcbq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2uegixhim.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2puyccrvd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ewwcvyau.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mefthqhj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2lxkmvygi.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2eihfvwle.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2zzibpvfw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gqbxrfok.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2whruxckp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gyjnggyv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2cxbhviey.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2rtffhbcd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2xztxlurg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ayhfouzy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2pkykfszw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2xkzeldam.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2thbrrbfo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2juzntpyu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2zahncfgh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ffbbkhbi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2qezdjqsz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iyfowheu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2qtlgqdjl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dbuofvzs.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cpaleucn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ruveplwh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2sldtxtjj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2iibiucdk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2zzrazwvp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2wgsmvabm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2kktslepm.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zhpyvqzn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2hlpngkhv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ahuvoqma.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zpighupe.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ryeycafb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2jdjpuutx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wlsscjme.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2jkriyxpj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nxzfdnye.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ulpifncv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2fwxahtkj.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2raddldtm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mhitwisg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bzxvyfgc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2wuywckyt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2cjdmkxxe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2qykotuuz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iegfnqpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nylnsazi.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2alykuzke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwwpqdon.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wimauyhn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2knlpsxlt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2skrqakoq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2bluqdxnx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ustukzbz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ywyofuan.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2szbczjnq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ivmhjkgz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2azrjeuco.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fvtwopms.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mzqefcgd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mymryhse.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vpydgcgs.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ojsjfyhf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xullvsbi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ebgoozkr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2isizsrug.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2aamgbjjh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2xwbaksrr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2qxnnjset.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2lsnkwmim.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2oplvpodw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lypptcee.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2rvxxklgt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2xilkapkq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2cbvxrayz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2nlntwflh.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2bsigdwjf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2oilhblso.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2jmqpdqlb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dloxpfwp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dqptocwg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2wohtwyeo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vayxcdoa.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2qkafahgl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2eblnmupo.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2usshuevm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bgintimw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2wvdvlpof.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mbjrmtus.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pgmvafbh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xkapkzvz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tenrwujq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2gkziumrw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2eirzwrlx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2basjzext.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cfbueqmo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ajrwadgg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ifcgdisy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gmfpilye.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fkeykten.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2gcslpygi.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2lluurgfx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tcszhaof.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2xwcpxfhh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2swhxcnep.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2jtciulab.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zqotkhtn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jixhyqvl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zaorwhsz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2qwslysyu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2dusripmy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zerrhdoo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2piofbekp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mkxlgzbn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2daqxjjdl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rbkxjdfl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2yutebpwy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2edteviir.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2cmiirbqs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2bynxukjy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2wotqvvse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2enhifgbo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ifbhlask.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2msgenlbz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nfeipoho.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eapyhdhs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2luzjlujf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2eoimxrdj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xgbbgiiq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gmpeuwbw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2orpgwyes.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2pkqzadbh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ukaqgsaw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2yrbkhnqm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rbemobca.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2bvojptph.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2acfdpoal.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sgtryuzo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2kyrbljvj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cjxtvcct.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vkeaekiu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2decncgso.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2iaqefgfh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2xpfkmhoz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2qjcyhxlz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2brrzfomc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2uvelngkc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2fcdrooov.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2vkmftztr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2eeftccep.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2rrhtsfpn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2zorpksip.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2silewtoa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jwqouzxy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2unjivllt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xmauvoyi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfhmstzx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2cnabqhhs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2omzrrtlz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mccbypcx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2xogtqxmk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jkxuvluj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnamoify.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cduxjdoi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zrgabnid.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2bbeurnyu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2kdwcfugh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jyxdeqoc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2abkstrfb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2anhbrrzj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xgppbiyf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rnwmneya.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qrlshrwz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ffcdarmn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2egjrysgk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2kjyqldak.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yyojqncq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2amcefjrz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wyeehfns.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2vgnywgyj.html


<!-- 参考信息 -->