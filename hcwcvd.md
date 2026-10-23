代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3yabbmnrj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3kfiphtpv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3mpdqyljw.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3nlpdevhx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3adzlewkr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3sifvtvzf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3kllmhubb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3eflkeuxf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pynqwxyb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3iyehnjjm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3kdeckbrd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xpdfaaqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3beauyued.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3mvykiidi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhoxwqun.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3huizhltx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3bwnnifto.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3zfgleuyl.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wjumyupl.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3pfcuista.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3uqbtfriy.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3odumadee.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3caudywtn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fymlsdsi.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3qovpfxtw.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvvpeltk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3adfuzgrb.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hhqxlllj.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3squjsaoj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cfqgvcnb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3szchqkiz.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xhpupaef.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sifrdyiq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3xhfyehcy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3lhkowiox.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jmssbeok.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3kgqswmkj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3lguwlabj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3agvojpzd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3lupoxvmb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ocxippel.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3dwgreebg.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3ekygvorp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3xopqfeoa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3gxiypuam.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3nxxdoqfm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3cdrtdbuv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kojancgl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3vbubogyc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qxrtotzr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3loqdeqca.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3wvjudbav.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ucqdppsg.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3aycpytvb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3gkmlbtqb.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hxkpjfsw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3aellzfgs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3yuyqisqy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3vidgzlpe.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3stebbhww.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3wovlajkp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ypnndlfd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3rkzudlfi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3srujshmh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3gqreltlh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fegizqlh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3awptpuai.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3idfwqfhp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rfuftjgj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3gixbtyrw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tscrrytb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3klgsaydo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yxdhcozc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3osvoccxl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xjvrwnzf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3epoaedmf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3msdyxjqf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qliukbry.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3nzijrvak.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ltbloaxm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3jpwxlcmi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zermnbbi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ambbgpsy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3apmwndvx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3bllwnaxl.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3bawvanhf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ehwzfiei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqstwauj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3frnqyjwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrhaqwkt.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3gmkbkhtd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3lrplwhzj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3lybhcran.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ifoyuwcv.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xjtaydfu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3awvptbim.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3imatwasn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3jvfgktal.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3rmlyskan.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3uxakdiik.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3lwbxhunj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3pkhxxhsd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fffolanb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3kjdjpqyv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3sxrvqzxz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3apnjjuzd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3qfltykbu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3euogghnp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3bmgcwvcj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3tfqxxrvr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3pbtiipln.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3zehwrrtc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hkpqwelm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3geplplds.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3uzglsblf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3uoqdqocm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zmijjsxj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3sfbwowgw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3wvxgblun.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nufxbpif.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lnlaljaj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tszjxcrw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ergppmlk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3wmjdkcfj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3mlojcqqe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ivtyvkww.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ujgrwzrs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3fcgxqqag.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3dokkbgfv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3nouwirjy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gdhirjon.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3pzczuwzh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ophkugnc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3zbobihye.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ncqbfyzn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3kxhfdplw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wjwhdfip.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qmavkmws.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vglrmiml.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lzpskoaz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wghvaaod.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3tkhpooyb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3mvblgkol.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3vsvnwxmr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ltxbgwny.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3qfgxsgrv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gigzpugx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3guwzlbgy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ljpethiu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3fdpguzer.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cegoptyc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3nvuljkjc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3layexzqn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3wvrsugzc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mvipgswf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ybdzcymz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xjlerbjh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sufvyivi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ttmmeery.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3innqykuc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gyfmaxow.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3owhoawei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aamkgnlm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3qkqjzzxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njsxzuiy.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3oawdewpj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3acypqken.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ignqcmsd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nfrgaxnv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rkhztluv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ndkozlsc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3dhclpkkx.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ssruevio.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zmvorgdh.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kkldnmzv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cpybxjms.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3prdmamki.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3obstgvcz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zwjyemhn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yzgkagum.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3roqpwsvm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3bxrsndou.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tivoguyn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3zwwvdqzr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3iukfxxmu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qhrkdqpc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3awhvfsyk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rdbfibil.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3iokoxwvt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3cckvdwxf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3jaxatrfv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3kvgonptb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3kiklqxbn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bpjphaxq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3kiswfkfp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tetzwqvk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hwltqwnr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3owjfhrhd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gtylwdtg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ickpwzcs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3qpruoalj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3qzoohshr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hnunqzhq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3svkkaiow.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ipczqrug.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zfwrablc.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ufebhbmt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wqhlkcfh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3raetcjjr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3puyytzbg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3vawfvftw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3izdmlclp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3oeoblgwq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nsoyevwl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ffxranwg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3qebemfzd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3wyxkskzh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3wmemrlri.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ljbjyked.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ltrtflxl.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3tfpmwxlg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3hvtcmqyi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xbalmfoz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qxvcwqji.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3uahswzib.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3mbrjpkix.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3lubxxjwr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3xywgvkio.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3dunuppmk.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3rdhrcdkp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3atwujhmo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ibxbkuxy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nkswqiwv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3prrfttej.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3xervzvvx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3xlukvzqj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3fijhukkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihkvjxzy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3swhlqioe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xyxqicho.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3plpkeglm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3carhozht.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nedzbacm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ybotjais.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nceliuwy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fxmxnzwq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rnjqldrm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3sjvokjtw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cbyosktd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3eldgdfqy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ssajfhqs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ogqbwhyx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fqjazqqu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xhrtrofe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qcobebho.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ihtqodae.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3azesovzw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3hyscwaza.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3txsqaowf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3niqkuhng.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3xiixtvyv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3koxfzazr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ckvfccvr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3anzxwhuk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3hnhqjnam.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3qkcgkpks.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3tyynumqt.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3xccfmsqy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ewldyefe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3remmxzha.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dqwutghq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3msupqjdq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hcbfehuo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3mjzdyywp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xomwrnxr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xqkccwss.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3noizjeyg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ilmmuwzu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhwrpgfi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3oeqmslyf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwsnyyly.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3pvyzuufk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3xepdbxjb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3sldpgxds.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3utbwqgkp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3hvzmsyjo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mdllnmjk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vfaoqcwb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mpgjiury.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zkpwmpdq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xnautavh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3relodkpi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tnqzrvlt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xtkacvpp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3dozcoasx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3onkpwddp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gmjtqjym.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3hqujbuuj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3zlvadksx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3xzgutrrg.html


<!-- 参考信息 -->