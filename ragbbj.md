代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3hqcrnctn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3zgritbwt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3kcxkjujk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qicmdmyc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lxzwiwku.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3qnmnpgga.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3kcxajqri.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3wrxsyjdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epehairo.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3dhwghuwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctzxzhdj.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3wxbnwtvx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3taprwlek.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3eyefsryo.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yjacagtb.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lxvyihyx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3iwwrcnix.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3hgmwpvsp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3kqgubyye.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3daacpzaf.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3xhczfcdj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3seocizmp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3vqjkegpb.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3yuafdlwa.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3oabykyjj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fwxnnykk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3sqqrisay.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3kaxcwkne.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3avubotsm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3lljzcvpw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3dkskqxqb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3uwhswaui.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3liwpmnpj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3sphpwvkc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ivcwnafw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3zibsqjwv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3hhjxsooh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3dhhcxpvm.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3befdszzu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3piyullqo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3qrhyjzpc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3izfulozg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3buxphzhb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hrowsrdh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3avjgeepv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3bmtmhqhm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ksftkhfj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3lwspjdun.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3nothtjsm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3kxmcrjtr.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3poydivsz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cpgsojxl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3djgntjgp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3geklqzpi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3nsfmeoxi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3lwjypffw.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3vniwppda.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xrlbyysz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3bwotddyx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3tqhswcpc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pkgjxqer.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3epiwohbu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jfreggwx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jrvbayve.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vrenghhw.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3bbcwppvm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pqpxmavi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3nwvgjevf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kpwuxbiq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bhabfbzr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3piovjpwv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3pumtwgsk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ixsndxjr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iodhbbht.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ykwbiimv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jednjtju.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3scgajlmz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mmzesggu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dcqhnbzg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3esgohgzi.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3yzgkhbsj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3saoupdwr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mebgcdgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mphiukrn.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3nnoneenl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrrghgpd.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ozogpehy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3lfjnmphm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3skicbgms.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3eweumtof.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3nnsmashb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3soxzbpeq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3udxlobap.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3wmvesoja.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rfgcxbgc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ukwvtzqw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jkoimjhf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3epboikxf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3hjtqtxah.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3yyranzne.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ihnpgkqb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3iyolxnde.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3zeuedpai.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3beoyyfcq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3uxnpwkbg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hrzpxkfk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tpoatnue.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bmazjrdm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3glxguszb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3hjztkaku.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3inotkzuo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3nlxxgmhz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vyuzolmh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3cjfyircx.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3bsnuqxpa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3njmoistq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qqtgmylq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fikvvhee.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ggznhpyd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3swtcznty.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3khltxuhz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3shwuiuup.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ampybwuz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3hsdncrza.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3tlcwcvgh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3dkdygldb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3yicsdvax.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3bextvhux.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3delttzau.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3dzfqnory.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kvsoniwf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3egogusfg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cnvhohuf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3wpfkxqjc.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3opnlpevf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wovezwbu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wziqnxqg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3cdrujkip.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3whmibyua.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3aeuuvshw.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rpztralz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3okmzkrtq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rgjbcpbs.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pdtwqxqy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cdfyjvdt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3lvnwulwv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3yuhybgln.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3qzwkqafj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3klwrqfep.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3cqewdlzj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3bdyyltod.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3szfktczr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hkechqih.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jlqndqfq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3bobkelwc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3dpvaouda.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3cokgicnj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vlgneyju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlbunqii.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3nvdjfwis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mudvoqta.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tzmijmyv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bhuzxwrz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ljsmdfex.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tcphfprt.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3pjymapci.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3blsdgthk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3afozcqyl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3nalpjivq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qbcqbjdz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3clancxcn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sprckirr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3wrenpsqq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3iyucjdvd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pagdikwl.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lmiswlnj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kokjigru.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ynikeuwo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jhlkxsib.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ctgxppec.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mtterdmw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ceaxnkke.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jazcguso.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ehoahzqz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3gmsfdzit.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3etvvjeyu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3iyvprpwu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3mwlkzvkj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3inmosbnw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bpozreac.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3sdpybdlc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xrtijvxq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3udadnqhb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3huiugihr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ibhtthgn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3cvzdoooq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3csjazvgt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3bgiqyzcv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cnqxuali.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3panihdlt.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3emtmqohq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3awfbvecx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ebpyyleb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3asddfohw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3abghueen.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3iqrewspb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3pyccjmql.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3pybhzjuc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3vawvvmxw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xhzflhlj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jxnuqetc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lgvhnjtl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3wqvnsmli.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ysfdqerp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yconfgrc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ejlpcekh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ohziehzr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gbktmjwm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yoqefoms.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3unvotqku.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3offggtlm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3fjosxrfd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3lucgiptn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tcvoutqt.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3hjaczmqa.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3eaeyuilz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3hykbpkvi.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kvibivzl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cdogmebm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3bbntnltx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3flmvjniq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qhtiiumq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3fzgcmxho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atlgejgl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3todbstzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yitannqb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3snwvzgkm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zenqlcnv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vtpiplef.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mgohkxjs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3obcvlogv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3phjspjye.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lolzrkxg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3imvpcail.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eblczmkt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3wndyxmxv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jgtnizid.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3uvzuipim.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rnoztjqt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3usmaqqbn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qjkhrkfp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tinnlfaa.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3oaxcbeug.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3lcmbdoux.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3rkkjiftv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3tqjvmdwv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3disudvhm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3nhwrfimq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ihmlpsbk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3sjgehkvr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ztmpjqoh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3qfwnhxit.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3yvmhhgxe.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3axrsdquy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3grfflyif.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qqaryndt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xkjaoiie.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3imgdkdpo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rcfptqxe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3vhgtewig.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ocpxmzzu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eiatqgvy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ycfwfolu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gslpczgt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3rdmgygkv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukfnrkky.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zywjalhm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3obmhsqwo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3atxbwjow.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jfxuaqad.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3yfhiytwe.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3lmrmvpxr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gjriisba.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jzcwemha.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jjnprawn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ggyeepup.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3vaeezojh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3fnjyfywo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lpedceqt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3bpysqtwn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cabnhdkt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3iiqvpykd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3mgfdlshr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ufurrxnr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3nmtvxxtg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3zilawwsh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xqgukavs.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3nwpzzton.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qlivwlsg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3htxhpyle.html


<!-- 参考信息 -->