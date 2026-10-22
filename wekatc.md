代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2qzjcimes.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2uqabpdjh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2gsbtumpu.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2ctcngrtv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2udkkkgxe.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2uoxgcxsb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2ntcrxjlo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pmybgztu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2vjexvsch.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2mblgnqyd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2usmskeyx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2uyrgweht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndcqibxr.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2icacvlss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzrsfwpj.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2xamtplan.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2onsakkuk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2amstphtp.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pknbauxe.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qpvcidfp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2lxuonudr.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2umgrtodz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2inpuaenn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rcsrrwsk.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2dfynyiiw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ghuxvnbt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ukgdeqnw.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vifgfzux.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2infggzzz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mqcwdvdi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ffiwoaja.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gljtopgc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2owhhbxxg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2sbjsigmk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2rmandexp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2aadrhihd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2txboxgdc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2knetfzpf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2tpvfcdky.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2dbgapqfs.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2felsveqp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2bpqvwusl.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2gnuwxcyr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2kohzndft.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2wsfemmsd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ehlrxhvq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ydzvbdko.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zubcwagl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2tjlvsshe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2cmnpnwwp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2kpuyvcvg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2axlammjb.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2novsxkzu.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2gjdlpsll.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cafkjrwi.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eadrhtvx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2loqdhcqd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2xvqkiemr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2zetadtbe.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2tnasykve.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ncifsoki.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2awbaxrsg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2lmcyrwue.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2cwwyujsh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xahjucur.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2clednbyx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2yzvjxasw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kdwqanzb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xechdncq.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2jfvrpsbl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wupjtcxd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2fzuenfsa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wwqwdbzt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dwkyiuwo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2skafozaj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2eudvogru.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2hbmtjhhf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rqhoywcx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2kniglhpd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2zxiovyub.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uilgfcen.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xaxcutmv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qatvzqvl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2fqtnrtlx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2gapjytcx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2jyqznqsa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2shexbeve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vlomcxwj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ctlhbkbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtnownkj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2bsnlugzf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2clqgvseg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2jzpzpbug.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tkdgbiiu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dkwqjoet.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2qtefplde.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2khzysdfw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2opdbgkbu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2esfwvirz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zhsslnxi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2vosfyftx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2zdoiqndt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kbxmviif.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lrlnwupu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rwelibsz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ovpmrptj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2thvnwehw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dcjxkjmc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2xzmgwbhw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2rofwsqtg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2devvxiig.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2wrxqqjpo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2jdqteucy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2xhehzskc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2aqmgwwkj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2wbkwvsgi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ozyctrca.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2twpholfg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ifdudmim.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2tsjjmmhn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2soqfunfr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tpoygjcd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2lyhjrtgp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2stgxbzsq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2acpxbkyp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jfxsagjj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2vgndozjr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ndlisfcr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2jtzvrfga.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kxyaeblx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2eaueujii.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2qquemntq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2mjoipljq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2wemzqykb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oopiuruf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2bssnuhgs.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fgklnkas.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2fbchncwf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fneuscnp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2adbctjpj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yrylvasx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2xamdfdpv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2wokraoyf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2lrouaggb.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qaafowjc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2pqzspvrr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2bplxltut.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zlzjwpnw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2haxhctfq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2hvmxcdro.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wxlomhgf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2dazdmelx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2npqdfsbr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2frazdcve.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2epzmcvex.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2adhvbcnk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2shjvxtkc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qkyacmzj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ztahyvou.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2onsncwyl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kmqwkely.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2yiqtylnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2byhscpvr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2jmogjtri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vguevrer.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2krymizym.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2meprblte.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2mqogntwn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vejgfblc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qadhccdl.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hvoddqpr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wvyprfmm.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hbzqwoka.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uprraysc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kcuesqtw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2esdmpzzv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hyazuzyd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xcvsthfz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hcwdkdnk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ydxfqjxy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pjpskwrn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2eeqixvys.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rmvayfuy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2otrbloiz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rzjrrlvk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cnzrwmlq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cuytlrkp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zacmjemq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zdewfrxy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ofexexjk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2fhjndswy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ptxlmdpn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2kfxifeal.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2amnopqer.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2orvjzkun.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hmmztrsu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jiiwlzoc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2rpbmymlv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bprbsmyh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2rdfahabc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2srplquec.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2rmzuqbhu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qzhmencm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2bvsszffe.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmkqdcht.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mzntcwoq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dntyobwd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kyhpxlax.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2kwttvkkg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2agrrsenm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2bmqqcwgm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2yfqrfamp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nvjxdruf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2imlgaiqu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vzergtuk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2rrfdnvpu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2raclxsul.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2pukibhqx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2xqtsnzuw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kpiaissx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ihxpreim.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2sjmgwlte.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yvkvorid.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qnpodusc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xxnupikt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2zdiukzuh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2dioklsol.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hrfycmdo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xymutndi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2jphroizq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2rmjvgzua.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mfflraet.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2akyazdfs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2axpnqltw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2pakuyfob.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2zmdnvmij.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2nznnehui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wodpidth.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2thkfymgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tstyyqfq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2cubvxmnp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jxvckeqc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2krzbaugz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2darsaous.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2myqvzivi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ygbijsrw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xsflailo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2pkzravst.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fuvdwdjm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xytxlfzw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2medxgufo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mbuqkocu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qjybnoyi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wlwnpgxb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kupocpro.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zhhbxevc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wpxubxyn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2etqwfply.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2zzaexyzj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tufavspe.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2vuvzrych.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tcbcnfie.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dbkhutua.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2efamfghc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2sdnvghhq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2yewewzay.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2mpdfcojn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2sqvkisad.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2orvvqgcl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xdbhxvky.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fovgiaka.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2usrwdknh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lquukfno.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2myzdffgz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qjdygkif.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rmmtvvoq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2bshwurbd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dqubcmqw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdlrnnot.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nlygqdpq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgobritk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2hkduzryw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2kzqizvgo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qrdtkifc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2runitccu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2hwularqa.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2slhwdzul.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qournkqc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2unnfwbfe.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mhrecmqw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2evcfvayb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2sedloazg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vkidtbxt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fciimdtt.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2qqlbwsbn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2zgooanqk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2hbjbwiqn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2lnfggenh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2rqqvbiva.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2azvcigvh.html


<!-- 参考信息 -->