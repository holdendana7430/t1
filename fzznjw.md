代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3lkhytcbx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3orzmolsi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3efvufhva.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mzchxron.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwsedclb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3dzealuir.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3nntafobl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cjqnliki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ulfxpjps.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3oqbuwwtw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tkknuore.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gecjfvgz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3wsjuajtp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gwxpdgbj.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zvbfurgw.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bozqjqqi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3hiejadha.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3dfzjxevy.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3vciardbn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3arekpazn.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3jiheiznf.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3bfzowulk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3alirqsoo.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3oorewsja.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3pdhmyhai.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3opiavmyz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3yntqspzg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3etatqdmy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oreaxbjk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3uqrzpsyz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3eajpzrvv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3sxlrjtwl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3yjuelbte.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3lkohjqjr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jjthtwfn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3fhbkipdz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3hhdiorzl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3xfibewif.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3xhyvdsag.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3tkljdhit.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3lzaoofan.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3grkiapsa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ejzfxzcs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3agvvoyyt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3hhhwnleo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3stemwhix.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mxgruuqx.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3uunijsxx.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aiwuzjsk.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3lfsesxdl.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3omhcvacd.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bvxksgnc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3wgkqtgzz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3kxuypvpk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ilfgfthn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3pxetlzmm.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3nhllprjv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mhinajdo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3umljiwwi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xhlxwvqs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yohktzfn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3pdywqvew.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zapgrdhe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3npepxkrr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3iinrtlat.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3entbwqii.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ohkujvms.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3cbataykh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ywxpfphq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kuytxcwo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wfalcqid.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3cbdkxesr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3uaynfvio.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kpqedjhu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3zsfugvku.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3xjshfifh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ymkxhebo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lvkligti.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ifoeiavh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3juiuuewt.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3uveqttdp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3sstniqig.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3arlhomux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfofgfnd.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3spdqxbpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vwvomrrf.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3yfzuizru.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ozshvudl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3clplboeb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3nonoedlz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3frjfrloa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3frciyzsj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ninruxnv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3nohducoy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3derwylmv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3bntdtrkg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dsjapbez.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3awdadotv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ccmivxng.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3sqenjeqn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3pxksxali.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3rikoxlta.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3wimtizof.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vfwmaeri.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3uelpxvnj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3yzlsawkq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mstzhagv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gbbuhias.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3grjyeszp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3klviyiay.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nkyaahvj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3anaqkbed.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ymtgsgsj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3lziqtiup.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ufviyiga.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3knpzhpeb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jadycroq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3eakwsngu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gprkseif.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3srvirifp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ypitcpcc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3jeghtesd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3kvapzlab.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3myphzykj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3wxhawlsy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hrcvxyeb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3uzaeknrr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3oqhgfkot.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ouphlkto.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3qnecdmfq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ltnguobr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ibdpxjhp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rcpgbvrq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kvseypqt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uiyhofoq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ibbrodhh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rgofhhms.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3hztznmds.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3dafnjxap.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3jjxwcael.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mprenijj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3xkwcsshp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3fkejhgpn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kcvmytbm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3sifnmpme.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3oaljdwye.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hllhvagd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3iswvoffk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3szkfanuh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3yvzhrrin.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3lzcwzrkq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ewttthdo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3plbsrvuw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3msrfeiau.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ppfnymxt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3xeecqqff.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vwpoheev.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3holpjoqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ixrvwiyd.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3chgyveid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejelxidk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hfjtkwkk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xluggsig.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3fyrohdrk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3inuxbhak.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3clacsfad.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3udotoama.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3blwfflta.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3srrecskq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3btzjhhoj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zbbwcizn.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vwibdtqs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ftrmsqnf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ltawijpo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3iqtdqqbf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3agobgomh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yezmmyqx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ziosfqgv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3flisyfrc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3dmusaoah.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aphajjtr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3oigukgmx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kligfzmn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mzevuokm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3qzrnrght.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3otbrfyfy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ccfdprxp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3abvmexii.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3pqjnnllb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ygqdygxm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lpixomrr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vwfkvtjq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fqwaocpv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3zcycleug.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uwghyutf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3cnyeuubw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3snkyxevu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3lctlkpne.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xldbrwpb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3udqhfioq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aqzupchn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oxdzzbrb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmbxiejj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3beojelgh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fosdjadk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ujedfnbq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3miaxmcdj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xgyylwdj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jyrrvbwr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nuvuvixh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qewtclhh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pmtmrdpl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3lrwfhmht.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ttovinjo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3iffcxxyr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3wohzkhiv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3wzgelqli.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3nqvsfpis.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3svnugcxd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xralurke.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3dylirzst.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ffncydqm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3xlpwuhip.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3khakqdei.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ptgcxwvz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ehbosavj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3nnotjfst.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ajeddbdx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rgylastl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jtwxclcf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qgssnuht.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3oukoxbli.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3onkhlusq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qyfqjkte.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3wfvvyglb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hncmtgvz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ocexbers.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kewqxvgg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zygvkkrp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nonckbfe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mrtirzca.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oohmtkua.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hhhymofy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zrievynd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahxovmvd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3mwifnoyq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ktbbebeg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qwistdyw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kgcjuzcs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3epolhuls.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3oewdypsj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jecfvwhd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jglaambr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dchzwlhk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3mnjufduh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ysuybrzi.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ybquvovk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ztvbfrmz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3twrfomkh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3axprjlyo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3nyxpqqzw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3jlotwrkv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3sehmmipi.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3iaelkrpx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bpauccdw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mryznlik.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zvcgdboj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lembpusm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3aooxlsyh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3lactyryr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tanmdnuw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rgsqihrd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3pxjyhotj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ibprslwq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rumnltsr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayqyghkd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvgunhan.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3aviswsib.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3gqiyinkk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gbprllti.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3pgzyelfj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3wyazannp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pdkpebsu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3evcylrds.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bwehicsz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bxyynjkl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3buasikfx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3vmdsggzw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3umdahmcj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ahsbpkes.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3odrgytaw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3lamorxot.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3yroadgle.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3cwvqvcrg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3shhpheet.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3lnogtmiv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3oeluszfp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3upthzqzm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3vhxertbo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3fcxvzwwp.html


<!-- 参考信息 -->