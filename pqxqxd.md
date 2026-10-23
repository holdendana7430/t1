代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mdlygomu.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3ekbbnkaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bffuhrjq.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3ovpqnrgt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3vdbgxoqi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3dnxnzjhu.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bmoqjtlp.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3kyyznnfr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3uosvngzv.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3emhqhokf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3wuqhwnxj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3kevvdeaa.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3zvlqzzdp.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3eejyhfkl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3uoclftpb.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3fmudqavh.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3nzihapsc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pouoogah.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3kyhhkgpc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xputfwap.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jcbpkokp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ztcrttjc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3sguhjmly.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3vrqrxwew.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ihlqghip.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3tdbonrze.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3dqfckjzb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3wsdiinql.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wwoirpyc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3bammczcq.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3jzmooxsz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xqtcilrp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3pxhgdnif.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lqujdsrl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wjqnpxhb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xrhnadko.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wxtuwemx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3retufqhr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3blzbfppy.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3paybypsy.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3gjwxgqrq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3vwfsoved.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zvwhbjlr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sjxhfapl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3taxmlxwr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3dgawqrqc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gmnhpxhk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ptkcuwhd.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3lbfcqsgp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hvainbzg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3lwztodso.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hjadllok.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3lqonxtbl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3hrkzxtqj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bpuprsjt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ydnrbmnt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jrhrusnt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3jfimhdwz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3osisecah.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3aavxrnao.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3epssmajk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qmmznjpk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rpjgaufx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ujbyktkf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3rdethzya.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jrqkttew.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3nxypkyan.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bwcnosbf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3gackoaoi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ysxoizvv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3aplxcalx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3eoxrzidj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3sngfpfrk.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3safrwotj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3cfbjdauw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ekagvhqh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3rpabqbsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqdgugcx.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3pzbjndct.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3jpqtfomd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3lngccguf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cilamosh.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3osuubsrl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3okfwbcbo.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yvydofva.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3sgslupvg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxfcvtg.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cpykoxdn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ilwwtzel.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ecrafvqk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3krfkqsmq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zjoychiu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ndmvwcgw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3pnzjlesz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3mjyivqxe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xlqdikbd.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3clokbilr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3xzmcincr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3bxgctdzc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bvzlzrra.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gvyxwtnb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3yorkbhfe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pvgzyzhf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3yzspsnqv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jbngtexk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ccfanquk.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3tbphwaiy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qrzpxnck.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3etzjihnf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3pqxekese.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3watmcbdy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3qwfzzjdp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ykcuidxe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3weqbdajm.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3rhlnhboh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ueqcoekt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3yaiwfhpu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dehrnwua.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kwjvtfvy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ekwvfspc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3eifetyil.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ubifyumz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wbnojgdg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hqsvzmny.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3abcygdgu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ejbfwnmd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3huocbgfa.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tuqvomrv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pbpbauhr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3jznpxbly.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3iixulrok.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3yatemqdw.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tqdovzhc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3tosiksdx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3zwaplrzc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3lycbspaw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tjqtwhjm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vzmjnuvb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gggvaqnn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3zqjifnyx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gypwbpvg.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3fhbbgeoq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3xzosgwcx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3pwutilir.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mkgftpxx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hgbwafxe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3kvncwhcp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3zglviezo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nsixdjdn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mapcedgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahfknait.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ddxoyeps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zekukafu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zbvnotxc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3svrrohjs.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3wfvisurx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbshwyuq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3slkruzmp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rhvupdfg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ngffsowm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3cftbsjsh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zsonnifc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nhfsohzb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nqdcgyvx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bnrplyrf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cajpxxpb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wpiaxtbp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3spvswcho.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kdszxqtd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ppqjzuxf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ngxwytfc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3brdezbaa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3fohmcuyy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3fiumpzxe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3uyyxljxq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xpnbpxpj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3bmttkxqu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ntlzjavd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3klmkjmco.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3puyoprwo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3wlnnspri.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vmphjywd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3chuskpbs.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nhvyzipw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fogupicq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3prmnaane.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jilloinw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3iuomsvxy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3wsqjpcfk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3jlrlpngh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3djtxvtfp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ommizxsq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rezhkzog.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rftfzrfe.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mimzxmfb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jiapbnku.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3bmcvyngk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3smziigww.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3zrxhxpcx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wnilvxbk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fpfaqpom.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vucoxxsl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xnrjkobd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dtoqfvsm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3hzdyuoqr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3fdibmnio.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bsjhvixs.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3qgpkicxs.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3qbxnkakl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3mbjwyola.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tedkukhr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gkwhzaso.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wvpgpwyl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3yuojawzm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3dbvgkcvo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tokjmtzq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3csefmjtl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3nvhqsget.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3nfinnlna.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bfegbpjq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3iejqhmms.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3rbshdtgv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3oeonsyti.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bqzekqdd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3wwykeibr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esjaderx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3arpxomax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eaqdkeps.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3cinajecz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ujplxotv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qifeotla.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yvkkkeaj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xugenfqi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3onevclrc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xrptuohe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ukzpclhy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uzzcwark.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3qtmyxhfx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xuyacnxw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3dyvwmrof.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3donspyhs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rxifwecj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hvuzoetz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3oewwugqs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ehgdusgs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3adrtylls.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3hotivyxf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3climgxpr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3svdfoosn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3aeieeyqo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jsmizfwg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3qkxxdfaf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3yitncleb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3seaopfun.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3zavbvwgl.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3rcasmeky.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uojpvtpo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ehpvsmuu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tsybzgrn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xzogtxms.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfcuzmrh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xlbsbdkn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xkttcksz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pmvomnha.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3qnfuqvji.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3btdaihrk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ywougwqf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qtcvxuql.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rocywave.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3idjrhver.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3aidrqlqr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3kbrcidfo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxbaknao.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qrjfdjcv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kapvrcyr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ofsuflxk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uzzcxqmc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3idiigluw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3lmibkafk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3bykiuvud.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uuinmdnv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xgdkunge.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3hvdtfuni.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3msvwcort.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3etbsknnx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3veewvjdf.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3fnzdqzwv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3lrfdxfaw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3glzglgwk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3gpszwibg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3acosmohv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3uapbcdtl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xxqbzyns.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3lvpwyyft.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3proppawz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ptgfrmea.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xrbitmrl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gaqhaono.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3kmdchkbl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mnlfkkyj.html


<!-- 参考信息 -->