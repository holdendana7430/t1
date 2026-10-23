代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3shcaezik.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3cipvhoaw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3fjhyjuqu.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3rqlgefdp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3vsoypewu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3vydgdyig.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgwewqws.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3woetqwrm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3pcpqkszk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3skwnjoou.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3smlikxuc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3sqmhzphi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnworszc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3kotxkmnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gszgydhj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3keddqufn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3mfwyizbk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3fnfvnayv.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3nsvlzzjq.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wmvfjglp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3melgxxcj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mbvotsbf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3amxssrvk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qojwflcw.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ginwswsg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3bxbvjlwz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3gxelxyht.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3sdcrwedq.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3txgzokhm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hxbpoamv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3sgionuqo.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nsqhdwgu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bvsxnvyj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3nqowtynv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3vwolzxfa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3xtioumgq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3asxoliho.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3koxglaad.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3kaivncpa.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3vvbaxgfg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ykriinly.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3vxjhlkjl.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3prlklntq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ysttmzbm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3jzhixtia.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3qxrutjjj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jdsckmau.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wacxginl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3zvyjfcwd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3aghrvtvq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kzmusujo.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3bxfmdink.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3xhewcmdv.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3retadfxl.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wxmzncnu.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wzwaxypz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ilflypil.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3gcidrxos.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3tnhrxcoq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3lfwxzjmj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3lfcyvhkc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hgpnldog.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ntnmwpex.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tqtlfyfa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vknmkemm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yzjjqoyb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hiilytxf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ogdsrqnx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mxwmfxrr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3pzhnbtmy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3juoksrwj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3vypwbvfd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hjoilhwv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pfhrsrhj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3smrmhhma.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3wmlmmctb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3nsadhrhe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xfrkbtnt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3fyepbejv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3jhqxhamm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wwpogzhk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3eutuzwlp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3wbzqonpa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3epenmncb.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3vzvyjkfr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ygwauwqz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3meccpxhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xwzkdkho.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wglhkdew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olppwhxp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3kyhxrqik.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3qqkaprca.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3pzxgqkjx.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vbgeblwq.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rxqhwjmf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ojnucmsv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3etqmmkui.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3cmuopfbq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3rqpjzohe.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pmgfdpsx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3uhzhkude.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3itrdvqdm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3jwunaxlm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rnxohcqy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zltjlvxd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3xfzaxzzu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3adrthybs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hgqdmise.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3mafbbsrn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3noroqzel.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3elacujuz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3zhzhlapl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ekocbcad.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3hwjhwrql.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3glndpnsc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ghhobvzm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cvsyegun.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3jqdbgmhn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3biwuuved.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3oaefjkvt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3pnbfansn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tofhmctm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3czycuisv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3wiuxoavh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ggxnzbrj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hivgtvvg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3bcaibbub.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3rkhmsjyu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3utxckcbg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3dxmokolm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3erxymtof.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3bbemdfwv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3vqqukpfu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zndxrlzq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3smumykkt.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mmmeptbd.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gktntkjz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bxhydtvl.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gwledrpj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3modfurho.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fsgvdyde.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3utbmqxfr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3npffssim.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3gupbravg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3amfpgakc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3xdmmphvj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3niuzxfha.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3serqgjuy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mpscqxjn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3uhhtetij.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3qjphkbnm.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3zshehhfq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vqitqozv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3wmmvayja.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3acrqgvtd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ngupeyhu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cmecfeja.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vqtevxtj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3cvuxntzi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3yytelriz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nvcevczt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hkxsznjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3meabknkt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gklcwmae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqgrzjnf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gcbyfikn.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3dbxydslf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3dylzepwe.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qsdtggqd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qgwgxmue.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3szthftdq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dvawrifs.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qcrhtecr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lnqzcnmd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hllccdtg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lqzcjhdf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rugzucmg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3svpnjkhl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ailohgnb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3leellcry.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bxtaojkl.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3tidexpla.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xcoafgim.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3middsvfp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fekmhamz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3frntqcsu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nvfwngdk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tdxorvmn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ynkbdadw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xiqtupqm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3egftwdgi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3wjxjmvxq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3qydmlszm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3pljijldw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3rgxhkzst.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lsfzarax.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gzxmzrmh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3cdbgbhbs.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3eohafcfi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3lgnromca.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3mbsamovk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3vwbdrpoi.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yqnmdzqz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gzvmynph.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3koohfqvp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3frxojpnh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dgitfujh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zubxmnhq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3cefjuwrc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3hxnjalfy.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3etsxwwgj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ugslkslj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3umhnzpna.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fufcsehb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lffyrfyy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xdywuwew.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ebqkspgl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ozkfonvn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oaclylga.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3kwntlwib.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3oletxkbg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3hgfrozpf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ycsxdpow.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qjkpzdpx.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3odlmincw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3uamzwobq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3jfcvferf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jpmanznd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3gcszgcnf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qzduclpa.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3xmyrkspl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mkuoyjcn.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3oqapznbe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3tonpajrj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jhsufvrq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ccghmoqs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3mbtolhvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzjurwtx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3jfmcwybr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lssoftkd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3oiokeitd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fgfvgmyw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zkfcvvnd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qtglemwm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wxwqbvqz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gtklndyi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nzwpyfdp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3daajgjoy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3waildvng.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3hzrbphlk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vdeaulac.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3dgwbldvc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mdoeopxm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qhicxmov.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lnakxifu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ygrcajwh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ikqbostz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dcrbfgic.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3dlkhyfub.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kysoqfvo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3gkmkijrj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3iikdibpq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lyzyobcm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3nbnsivzt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3eezgcrsl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3brllzxeq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3wjaejvri.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qpkbvzzk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xluruomu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mcpcbfxz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dbjxaikp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qskfwpiw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jnfmxhjt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3qfgiryvo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qavpwkpd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nlggardt.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ogpjlbcm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sxsbltbu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlbpinks.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ptnaotff.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3pimnaflq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3zokumhnq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zkstbzie.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fidsrrcv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3kyabujpn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3iwfrazgu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3erirkqyo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ixzkufxg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hrrnwdzi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xdmkbanv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3jxpgutza.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3odadvshp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dmvqqkmy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ynyrffhe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3rjinykch.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3flfmfgjx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3lwtdwmoh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3duywbefz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jcixzfup.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fwpepdvo.html


<!-- 参考信息 -->