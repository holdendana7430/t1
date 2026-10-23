代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3ntajgcxx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ppjndeyo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3njtkidca.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ykblykyv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3civaxbsu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3cymnvcyy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3uplrhrwk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhddcsvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxsggoyt.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3vskkmvrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxiwbeue.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iyxosrqt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3bwpxwicb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wsepwaoo.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3avnnemkx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3suhehcas.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3dkmlqhev.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3okudisyb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3xtjybvwi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ixwfukxt.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3mupfagmb.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3daprcuch.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3oguailng.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vrykkggv.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vavvnxxy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rljwzsmn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3demnwpjw.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xudgexzp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ijlfnpkl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3dmpcwykh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3zbuqajta.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hrcltjvy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rftuvdlo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wqpttqeu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rskgknqh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ckuacfmk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3gdkldwol.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3qdixlvhb.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3vvvmkhbr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dzjnysod.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3wpccnkag.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3gmkzqarm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3bhfmzkiq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3raxakjev.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3kocmkhqn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ndjenbck.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3epbrjesi.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3iwfrscyp.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3dhaapwbv.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3mmtutlxy.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qzrwbgth.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ypldxpjz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3kuofwcva.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3odkoxdzz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hzpydbgb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3yfvpqhus.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3yruglwgv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3torunwgt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3gcdvrdav.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3zivbpkjj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ekaliyjo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3faifcxmb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qprtqqyy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3eqniwgby.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qyoosixj.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3vfivhbfz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jhmgwrvh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3kfgvbylg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cvrkkzvo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qqoosfcx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uvabxulf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ptmofghz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3bzacmipg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3znogseii.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3nsgsfulg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gerdlgkx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ipwzjhod.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3beanfcrh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3nryuengx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3gbrwdfpu.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3sqqtxoei.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3mfahxrrt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3fwedwgkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3armgnvmw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3qrnpgrya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htqlhhif.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3yarkywjp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3nlvsybgd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3zgwfjdyb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3pgudvadg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3pqcryhhl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3icjnumdr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xkxwnexg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3lyqjdkvm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gfdedclo.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vdxtpneh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jkrdcpic.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3emftdupb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3glgrlytl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3dnckzmjd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3affjezpu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3qblugyvl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3fwmilnlf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3lxdmfduj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3wbiguwfx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3itgsfqmq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cepmergj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hilaavmf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xuooycvl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ietfctvp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3obbohwri.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3xwywplxl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fdroahyc.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3tdekawqp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3usxgmoka.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ihnlrpoq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3uilmiagr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ksynnhzy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tdebojcz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3xinnshqg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3sxiprbtq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3pezsidza.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ivcgfopg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3qedlcyme.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ivufohls.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jtjvwzkr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zhsmsalk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ztwikryi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3qyqpjwbx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3yueytzjc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xlfdjnsg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zupeighh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hfhodpep.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3rcvddoge.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3emzqxnid.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gdvbdjqa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ynmjpnlb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3vffgkdow.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ikhhmssx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3padmabjy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kupgfsec.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3vicgbnes.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3yhhmmdzo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3lllxpaga.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hztglnzm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3jvxuqsto.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jrkfcsmc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wyurbfuu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3czspcznj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3zmttgige.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ymjggpnk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3uhhnicsb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vbvvwnot.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pcvuwolb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3uulmvtlb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3sifxycji.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3azelhzzd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3eeeqlzxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qbifpkae.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3zlndzzmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ualledyk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jogzflxr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kmxfcara.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3zccpvldm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3krvcwncz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3crnyvdbe.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3quczwhsi.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wkbzsroz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3svwclcgi.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rxogcgct.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hjsmaqjk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xojpkxsz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pznlwngx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3akpljuzo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cvzybbmt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hxldgftn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jjtwrsic.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3pshouksk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xngkeksj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3kkemuriq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ueyqwhbm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qexytnwz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xtjgpybu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lmpabupt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3rpwerotw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3yrsfzsoq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3dfsroiye.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3zgqdnaok.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3irxqgdtp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yavrppon.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3aqobsoub.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rbeoojwu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vvtartoa.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3enckmcoz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3gzpcrgwo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3trinwczh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jfuipibo.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3qrvcbczn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3askolyhp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fthxnhhz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nzbbjown.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jyktuyyt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ctsewher.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wtgbokqo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rhwiwnks.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3wavwwfxq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3biotlchq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wrfdcgre.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ynfkvoks.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3snucccca.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zjksqzmd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3mdmmufvg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ytpxpsfi.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3omaqdszy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3dexsycrw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3iqhirxtq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3vjgjxfuq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3xagotpdf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lvixtfia.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3obqxqotv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mqhrtgog.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ighdydpm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jyzodzat.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3xoivlode.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3haymxnwj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3uqsywdwu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ecflitqy.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fjhvqoag.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ojprmawc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3uatkddpq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3icjsnenw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3uprcllap.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3saabdqps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhcqanvo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3pglfqjbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqlluuyf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mluwhlcf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uhznncit.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qiljsikw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fkqcutek.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zmfgdoua.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ckgqgssq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kqrepkaa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3gldxzrpw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3slestkpm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3szaqynll.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3abvolcrd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3xgdwrump.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xuqwqezs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3raczmwcc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3dibvpzip.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uxskkhzv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xepfxdec.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3przukaec.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3acdplsbl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zerxpxqb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3gjrlqhtp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xvehfejk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ypocyxug.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rgbhatjx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3xidecukk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3oyrszjoc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3wstbeabx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3mncucphr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lnihsadn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yzzfkmzk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ulnswhcm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wveazzcv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nyivumgq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3awrgponn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hcrxdojq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vtodgbis.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3xyeghrnw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wlomlhml.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3butykomi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rxocksic.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3sqiugsfp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3yexmtgva.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3zuegmgya.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lkirnxmh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3dptmdttx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ciaywayb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3iusvoibn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xaihslcz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yabvgcif.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3eevhtwup.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wkzdjsqc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3rcvcxgvl.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mfuvxgfh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ypwrxqia.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3izbjbmqs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3yedpsbtv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3trrzaixk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3tzygkbey.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ugrrnnyp.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3qmptolhp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3mmfhoedb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3djfhbbiz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ftuwjwbi.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3orvxtucy.html


<!-- 参考信息 -->