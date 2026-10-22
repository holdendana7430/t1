代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2wxskeaax.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2ajrixfnq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2kuwyckph.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2vwhqicnu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2crhzijhm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ytlgqgck.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2ularvqfc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2mqqrdyhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzaavktn.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2vgsrdtir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyhknyfw.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bbbzeeek.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ymuyohui.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hgtuhyoz.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ljoywhqf.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2swkqrrad.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2tqhakbiv.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2fqijpndp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ppvmblho.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2qmhubtfp.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2yfxwbubi.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2xscsazng.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2bqmwdemk.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iizzapup.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pttlbaqu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hylzibwt.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2errklexv.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hxhgrrei.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2njecamgr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2gspvbbcq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2yyfsibbr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lvnzthue.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gqyxoewq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2jfwseimo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2bnmpwuey.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2gqzokboj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cgwhrqef.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2uqqvwaco.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2rgaifusg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2tmxqrmbp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2vyhnldef.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2uxhzolxp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2gbblgphg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2txrqwrox.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2tzmbmktu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2raomryoc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2gmcdvbrk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2tcceasfy.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2yivnucde.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2uyervzje.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qyfxgsgx.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yttpdbtf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ywfrqvth.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2dshsotum.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2gjtrvhaq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ydpdgktq.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2jnfwhrfi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ddcavwen.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2tuluppsh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2wkxbzcfl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jbxmdhfc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mbsfkcwh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2yetqwtoe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ildyslqp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rpfvzqnf.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ajpymgfb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xkjvquqz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ncukmnzg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2okqirsar.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zllntuin.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tnhustwi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2jrohirtj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2qidrturc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uyshwhnx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ixgvyuwr.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ocnqcqdb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2kipnboqg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jxgqnzxn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ffdatglm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2qsnpyqoo.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2phiglaje.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2tjmhtbte.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2sxtcqyqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qeeabfqv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2bvfsbdpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sllvzqmk.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2hqcmjiql.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2srvmkvuo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2dfcyixvq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2izupaumx.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cnjybynf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2tvnquqwg.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2dovltgfv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2bbhgsnoy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wfseelzp.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tmbhvygi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ytwjwduv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2gnyqceum.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jlsydsuw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2biegdvlr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ubuxuudf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2elxudvvm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2bvkdwhgy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gnllibnx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2jswopwua.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2majlcfcj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2dspcldwx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gkxolmrs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vxmdubss.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2tboahcbg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2lvpwjwzd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ffvuqlvj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2awmlpicf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2umuowppg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2mvjigqma.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2yuaibkmk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bxojtqus.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qvqbydfv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zxfaaghy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2eqpqelii.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2sgrkspqm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uhhfbvqn.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2zcdjoned.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2naflxfsx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2gaqyypmp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mmbtpvyw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rmyquphk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2uuyzxnrp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bquzvbei.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2vfwgnnqz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zlrlkslx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2dzggfjkv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jlbrghyf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2nkasltjv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jiesipwg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zmwntxuo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2iznaldvd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2guyqgmqe.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2tpuilsyu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2bdatytij.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qshvjamw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2hxleqqwp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2usuhfodl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pgrfmzju.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2sebywooj.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ldtryezc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2koqwmckk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ujcebbkj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2sanifmlu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jbdsvekz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2xuhrwjdk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2sifxywhp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2buydpvpn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xlafwywp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2oxaehsun.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2xnxbpzey.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2uiybupxw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2piocxzqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qseyjupz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2iynxtypw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gljkqnqs.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rewqakba.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2idwktchc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2oxndsivg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2oroksvut.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hthxfhxh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2groyndla.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2isijiakw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2mvkudxrg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xdjfmfny.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jfutufhs.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ejrnzuwc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2evvtdjim.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gdnlibtc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tqmtyoww.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sjoqvjqr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2deyungbh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2oceigbri.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qdphobjc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2cfwoipuj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fvvardea.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2btnlresl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zkcgvogf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wozcdxug.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tapbbrro.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2tzwlfrgs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2shsmipah.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2gbclhsku.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2fbzvzjvo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wwpscziu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2hdmufjwi.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hjdaibtt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2savsemcd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2oincutub.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2kowncjtr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2gswnyopi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2aqhbslve.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2pxsqiwjw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wwffbtzx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2pbzyyxwa.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tjdxcodu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pzlauioo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gidqukxz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2evcuuyic.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2yamivpjn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2mjjhhwiu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2igzjutgj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xkdxetle.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lolhyqdq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rrydsbkj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mfjuyjvx.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lgcingtg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2mxgqlcgb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2wufslcwo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2evopszth.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2yzxkmdiw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2msnuczdh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2pbrfubou.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ouuibglf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ykghejpp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2awzjdspu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2whczhihu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2saacdftn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2wcovwpms.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2fnqoitkc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2afcvfcif.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zertdqat.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tbnypxve.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dqlnrxis.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ujfsprom.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2hweebvyk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2vidjgurc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2uqacgsry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfnlzfqx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2fpdweeke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afuyhdll.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vgddigyw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qsrcmzam.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zfqjgxil.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lysvrnhw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nnfqduvy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kuqwtfev.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rpdbuweo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2qtvnjvbr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2etbcoesi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2mftouoea.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2uafipbyj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kysqnwkg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zoooqjnh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sgzduqos.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2cevbtzqg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xlmfzsvr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hworxmqu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hagozxks.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2dlztnwko.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2qrwktntt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ydlmpeuj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2angseiux.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2kznhbzrt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2etypacvd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2pqqaxclc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2uxagkgpu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2julxehrz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2nahltaqv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qofvoczk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ibeyiyde.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2stetugab.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tzjusydp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bjbpifal.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2gutnpemk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2imjqxueh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vloqhxhu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2biivbuks.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lfettmsi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2cklwjixd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyehazzz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihlckssu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2aapzndlr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2gplzoilb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2yqjgpecm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2pjoybcjl.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2lppnzmzl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xhrdotvf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lurzfwtd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2flcfdsza.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fooirblo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2beaedqlz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2sedoymby.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2nnkwlujv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2aobsidzy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2wwgiolnu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2rroukzos.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ipckpwzd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2nbdamaru.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2yjymzzax.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2zfynqwnk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2sutoyfpr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2meoanoyc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2hxislpwm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rqoqdcri.html


<!-- 参考信息 -->